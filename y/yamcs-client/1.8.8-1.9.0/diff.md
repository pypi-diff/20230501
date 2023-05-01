# Comparing `tmp/yamcs-client-1.8.8.tar.gz` & `tmp/yamcs-client-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamcs-client-1.8.8.tar", last modified: Fri Mar 17 09:13:31 2023, max compression
+gzip compressed data, was "yamcs-client-1.9.0.tar", last modified: Mon May  1 12:06:56 2023, max compression
```

## Comparing `yamcs-client-1.8.8.tar` & `yamcs-client-1.9.0.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.726254 yamcs-client-1.8.8/
--rw-r--r--   0 fdi        (503) staff       (20)     7652 2018-08-10 14:47:21.000000 yamcs-client-1.8.8/LICENSE
--rw-r--r--   0 fdi        (503) staff       (20)       34 2020-03-04 12:26:47.000000 yamcs-client-1.8.8/MANIFEST.in
--rw-r--r--   0 fdi        (503) staff       (20)     1510 2023-03-17 09:13:31.726084 yamcs-client-1.8.8/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)      578 2020-06-18 07:14:03.000000 yamcs-client-1.8.8/README.md
--rw-r--r--   0 fdi        (503) staff       (20)       38 2023-03-17 09:13:31.726307 yamcs-client-1.8.8/setup.cfg
--rw-r--r--   0 fdi        (503) staff       (20)     1529 2022-05-30 08:34:06.000000 yamcs-client-1.8.8/setup.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.651310 yamcs-client-1.8.8/src/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.659412 yamcs-client-1.8.8/src/yamcs/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.661768 yamcs-client-1.8.8/src/yamcs/api/
--rw-r--r--   0 fdi        (503) staff       (20)    13641 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/api/annotations_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)     3671 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/api/exception_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)     5141 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/api/httpbody_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    13250 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/api/websocket_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.664331 yamcs-client-1.8.8/src/yamcs/archive/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs-client-1.8.8/src/yamcs/archive/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)    35234 2023-03-09 08:58:34.000000 yamcs-client-1.8.8/src/yamcs/archive/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     8476 2023-03-14 14:48:29.000000 yamcs-client-1.8.8/src/yamcs/archive/model.py
--rw-r--r--   0 fdi        (503) staff       (20)    20172 2023-03-17 08:28:42.000000 yamcs-client-1.8.8/src/yamcs/client.py
--rw-r--r--   0 fdi        (503) staff       (20)       22 2023-03-17 09:10:11.000000 yamcs-client-1.8.8/src/yamcs/clientversion.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.668280 yamcs-client-1.8.8/src/yamcs/core/
--rw-r--r--   0 fdi        (503) staff       (20)       28 2022-04-07 19:17:50.000000 yamcs-client-1.8.8/src/yamcs/core/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     6177 2023-03-15 14:14:18.000000 yamcs-client-1.8.8/src/yamcs/core/auth.py
--rw-r--r--   0 fdi        (503) staff       (20)     4301 2023-03-15 14:11:22.000000 yamcs-client-1.8.8/src/yamcs/core/context.py
--rw-r--r--   0 fdi        (503) staff       (20)      393 2022-04-07 19:17:50.000000 yamcs-client-1.8.8/src/yamcs/core/exceptions.py
--rw-r--r--   0 fdi        (503) staff       (20)     4138 2022-04-07 19:17:50.000000 yamcs-client-1.8.8/src/yamcs/core/futures.py
--rw-r--r--   0 fdi        (503) staff       (20)    10570 2023-03-15 14:13:17.000000 yamcs-client-1.8.8/src/yamcs/core/helpers.py
--rw-r--r--   0 fdi        (503) staff       (20)     1507 2022-04-07 19:17:50.000000 yamcs-client-1.8.8/src/yamcs/core/pagination.py
--rw-r--r--   0 fdi        (503) staff       (20)     7575 2023-03-14 12:40:04.000000 yamcs-client-1.8.8/src/yamcs/core/subscriptions.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.674369 yamcs-client-1.8.8/src/yamcs/filetransfer/
--rw-r--r--   0 fdi        (503) staff       (20)       65 2022-04-07 19:17:50.000000 yamcs-client-1.8.8/src/yamcs/filetransfer/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)    10637 2023-03-14 13:45:48.000000 yamcs-client-1.8.8/src/yamcs/filetransfer/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    15752 2023-03-14 13:44:52.000000 yamcs-client-1.8.8/src/yamcs/filetransfer/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.675503 yamcs-client-1.8.8/src/yamcs/link/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs-client-1.8.8/src/yamcs/link/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     7647 2023-03-14 14:42:37.000000 yamcs-client-1.8.8/src/yamcs/link/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     1853 2022-04-07 19:17:50.000000 yamcs-client-1.8.8/src/yamcs/link/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.676576 yamcs-client-1.8.8/src/yamcs/mdb/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs-client-1.8.8/src/yamcs/mdb/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     6141 2022-04-07 19:17:50.000000 yamcs-client-1.8.8/src/yamcs/mdb/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    12341 2022-05-30 08:31:08.000000 yamcs-client-1.8.8/src/yamcs/mdb/model.py
--rw-r--r--   0 fdi        (503) staff       (20)    11052 2023-03-14 12:40:04.000000 yamcs-client-1.8.8/src/yamcs/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.676909 yamcs-client-1.8.8/src/yamcs/protobuf/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.678129 yamcs-client-1.8.8/src/yamcs/protobuf/alarms/
--rw-r--r--   0 fdi        (503) staff       (20)    29157 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/alarms/alarms_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    39439 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/alarms/alarms_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.680274 yamcs-client-1.8.8/src/yamcs/protobuf/archive/
--rw-r--r--   0 fdi        (503) staff       (20)    30515 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/archive/archive_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    51245 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/archive/index_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    35584 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    19025 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/archive/rocksdb_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.682034 yamcs-client-1.8.8/src/yamcs/protobuf/audit/
--rw-r--r--   0 fdi        (503) staff       (20)    12095 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/audit/audit_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.682395 yamcs-client-1.8.8/src/yamcs/protobuf/buckets/
--rw-r--r--   0 fdi        (503) staff       (20)    34163 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/buckets/buckets_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.684804 yamcs-client-1.8.8/src/yamcs/protobuf/commanding/
--rw-r--r--   0 fdi        (503) staff       (20)    12531 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/commanding/clearance_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    39728 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/commanding/commanding_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    45990 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/commanding/commands_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    40386 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/commanding/queue_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.686089 yamcs-client-1.8.8/src/yamcs/protobuf/cop1/
--rw-r--r--   0 fdi        (503) staff       (20)    35089 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/cop1/cop1_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.687293 yamcs-client-1.8.8/src/yamcs/protobuf/database/
--rw-r--r--   0 fdi        (503) staff       (20)     8365 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/database/database_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.688747 yamcs-client-1.8.8/src/yamcs/protobuf/events/
--rw-r--r--   0 fdi        (503) staff       (20)     9412 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/events/events_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    30854 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/events/events_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.691120 yamcs-client-1.8.8/src/yamcs/protobuf/filetransfer/
--rw-r--r--   0 fdi        (503) staff       (20)    76664 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.693012 yamcs-client-1.8.8/src/yamcs/protobuf/iam/
--rw-r--r--   0 fdi        (503) staff       (20)    73707 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/iam/iam_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)     8383 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/iam/sessions_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.693572 yamcs-client-1.8.8/src/yamcs/protobuf/links/
--rw-r--r--   0 fdi        (503) staff       (20)    34775 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/links/links_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.694000 yamcs-client-1.8.8/src/yamcs/protobuf/mdb/
--rw-r--r--   0 fdi        (503) staff       (20)   227553 2023-03-14 15:00:23.000000 yamcs-client-1.8.8/src/yamcs/protobuf/mdb/mdb_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.695043 yamcs-client-1.8.8/src/yamcs/protobuf/packets/
--rw-r--r--   0 fdi        (503) staff       (20)     4689 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/packets/packets_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    33596 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/packets/packets_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.696936 yamcs-client-1.8.8/src/yamcs/protobuf/processing/
--rw-r--r--   0 fdi        (503) staff       (20)    27862 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/processing/mdb_override_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    81524 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/processing/processing_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.697396 yamcs-client-1.8.8/src/yamcs/protobuf/pvalue/
--rw-r--r--   0 fdi        (503) staff       (20)    30578 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/pvalue/pvalue_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.698003 yamcs-client-1.8.8/src/yamcs/protobuf/replication/
--rw-r--r--   0 fdi        (503) staff       (20)    13152 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/replication/replication_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.698617 yamcs-client-1.8.8/src/yamcs/protobuf/table/
--rw-r--r--   0 fdi        (503) staff       (20)    67041 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/table/table_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.699242 yamcs-client-1.8.8/src/yamcs/protobuf/tco/
--rw-r--r--   0 fdi        (503) staff       (20)    32904 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/tco/tco_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.699868 yamcs-client-1.8.8/src/yamcs/protobuf/time/
--rw-r--r--   0 fdi        (503) staff       (20)    13072 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/time/time_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.700303 yamcs-client-1.8.8/src/yamcs/protobuf/timeline/
--rw-r--r--   0 fdi        (503) staff       (20)   115941 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/timeline/timeline_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.701482 yamcs-client-1.8.8/src/yamcs/protobuf/web/
--rw-r--r--   0 fdi        (503) staff       (20)     8530 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/web/auth_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    50999 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/web/server_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.702012 yamcs-client-1.8.8/src/yamcs/protobuf/yamcsManagement/
--rw-r--r--   0 fdi        (503) staff       (20)   117378 2023-03-14 15:00:36.000000 yamcs-client-1.8.8/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    42560 2023-03-14 14:59:17.000000 yamcs-client-1.8.8/src/yamcs/protobuf/yamcs_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.704168 yamcs-client-1.8.8/src/yamcs/storage/
--rw-r--r--   0 fdi        (503) staff       (20)       55 2022-04-07 19:17:50.000000 yamcs-client-1.8.8/src/yamcs/storage/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     4853 2023-03-15 14:14:43.000000 yamcs-client-1.8.8/src/yamcs/storage/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     6181 2022-10-22 06:39:00.000000 yamcs-client-1.8.8/src/yamcs/storage/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.705614 yamcs-client-1.8.8/src/yamcs/tco/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs-client-1.8.8/src/yamcs/tco/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     4611 2022-05-30 08:31:08.000000 yamcs-client-1.8.8/src/yamcs/tco/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     2747 2022-04-07 19:17:50.000000 yamcs-client-1.8.8/src/yamcs/tco/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.709627 yamcs-client-1.8.8/src/yamcs/timeline/
--rw-r--r--   0 fdi        (503) staff       (20)       57 2022-05-30 08:31:08.000000 yamcs-client-1.8.8/src/yamcs/timeline/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     7355 2022-05-30 08:31:08.000000 yamcs-client-1.8.8/src/yamcs/timeline/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    12333 2023-02-15 13:00:11.000000 yamcs-client-1.8.8/src/yamcs/timeline/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.710503 yamcs-client-1.8.8/src/yamcs/tmtc/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs-client-1.8.8/src/yamcs/tmtc/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)    49752 2023-03-14 14:42:54.000000 yamcs-client-1.8.8/src/yamcs/tmtc/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    31663 2023-03-15 18:42:11.000000 yamcs-client-1.8.8/src/yamcs/tmtc/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-03-17 09:13:31.725596 yamcs-client-1.8.8/src/yamcs_client.egg-info/
--rw-r--r--   0 fdi        (503) staff       (20)     1510 2023-03-17 09:13:31.000000 yamcs-client-1.8.8/src/yamcs_client.egg-info/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)     2916 2023-03-17 09:13:31.000000 yamcs-client-1.8.8/src/yamcs_client.egg-info/SOURCES.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2023-03-17 09:13:31.000000 yamcs-client-1.8.8/src/yamcs_client.egg-info/dependency_links.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2022-04-07 19:46:24.000000 yamcs-client-1.8.8/src/yamcs_client.egg-info/not-zip-safe
--rw-r--r--   0 fdi        (503) staff       (20)       54 2023-03-17 09:13:31.000000 yamcs-client-1.8.8/src/yamcs_client.egg-info/requires.txt
--rw-r--r--   0 fdi        (503) staff       (20)        6 2023-03-17 09:13:31.000000 yamcs-client-1.8.8/src/yamcs_client.egg-info/top_level.txt
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.744094 yamcs-client-1.9.0/
+-rw-r--r--   0 fdi        (503) staff       (20)     7652 2018-08-10 14:47:21.000000 yamcs-client-1.9.0/LICENSE
+-rw-r--r--   0 fdi        (503) staff       (20)       34 2020-03-04 12:26:47.000000 yamcs-client-1.9.0/MANIFEST.in
+-rw-r--r--   0 fdi        (503) staff       (20)     1510 2023-05-01 12:06:56.743944 yamcs-client-1.9.0/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)      578 2020-06-18 07:14:03.000000 yamcs-client-1.9.0/README.md
+-rw-r--r--   0 fdi        (503) staff       (20)       38 2023-05-01 12:06:56.744138 yamcs-client-1.9.0/setup.cfg
+-rw-r--r--   0 fdi        (503) staff       (20)     1529 2022-05-30 08:34:06.000000 yamcs-client-1.9.0/setup.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.650806 yamcs-client-1.9.0/src/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.653252 yamcs-client-1.9.0/src/yamcs/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.663130 yamcs-client-1.9.0/src/yamcs/api/
+-rw-r--r--   0 fdi        (503) staff       (20)    13641 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/api/annotations_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)     3671 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/api/exception_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)     5141 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/api/httpbody_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    13250 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/api/websocket_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.664230 yamcs-client-1.9.0/src/yamcs/archive/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs-client-1.9.0/src/yamcs/archive/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)    37001 2023-04-17 10:07:37.000000 yamcs-client-1.9.0/src/yamcs/archive/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8549 2023-04-16 21:50:06.000000 yamcs-client-1.9.0/src/yamcs/archive/model.py
+-rw-r--r--   0 fdi        (503) staff       (20)    20411 2023-04-17 10:03:18.000000 yamcs-client-1.9.0/src/yamcs/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)       22 2023-05-01 11:34:54.000000 yamcs-client-1.9.0/src/yamcs/clientversion.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.669072 yamcs-client-1.9.0/src/yamcs/core/
+-rw-r--r--   0 fdi        (503) staff       (20)       28 2022-04-07 19:17:50.000000 yamcs-client-1.9.0/src/yamcs/core/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6769 2023-04-17 08:48:02.000000 yamcs-client-1.9.0/src/yamcs/core/auth.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4659 2023-04-17 10:02:53.000000 yamcs-client-1.9.0/src/yamcs/core/context.py
+-rw-r--r--   0 fdi        (503) staff       (20)      393 2022-04-07 19:17:50.000000 yamcs-client-1.9.0/src/yamcs/core/exceptions.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4234 2023-04-16 19:38:09.000000 yamcs-client-1.9.0/src/yamcs/core/futures.py
+-rw-r--r--   0 fdi        (503) staff       (20)    10998 2023-04-16 19:59:06.000000 yamcs-client-1.9.0/src/yamcs/core/helpers.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1611 2023-04-16 20:00:45.000000 yamcs-client-1.9.0/src/yamcs/core/pagination.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7628 2023-04-17 11:03:25.000000 yamcs-client-1.9.0/src/yamcs/core/subscriptions.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.670026 yamcs-client-1.9.0/src/yamcs/filetransfer/
+-rw-r--r--   0 fdi        (503) staff       (20)       65 2022-04-07 19:17:50.000000 yamcs-client-1.9.0/src/yamcs/filetransfer/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)    11638 2023-04-28 11:53:26.000000 yamcs-client-1.9.0/src/yamcs/filetransfer/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    16832 2023-04-17 12:13:52.000000 yamcs-client-1.9.0/src/yamcs/filetransfer/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.670827 yamcs-client-1.9.0/src/yamcs/link/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs-client-1.9.0/src/yamcs/link/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7824 2023-04-16 21:11:08.000000 yamcs-client-1.9.0/src/yamcs/link/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1927 2023-04-16 21:10:35.000000 yamcs-client-1.9.0/src/yamcs/link/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.671551 yamcs-client-1.9.0/src/yamcs/mdb/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs-client-1.9.0/src/yamcs/mdb/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6825 2023-05-01 11:42:55.000000 yamcs-client-1.9.0/src/yamcs/mdb/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    12854 2023-04-17 12:11:33.000000 yamcs-client-1.9.0/src/yamcs/mdb/model.py
+-rw-r--r--   0 fdi        (503) staff       (20)    12193 2023-05-01 11:42:48.000000 yamcs-client-1.9.0/src/yamcs/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.674240 yamcs-client-1.9.0/src/yamcs/protobuf/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.675688 yamcs-client-1.9.0/src/yamcs/protobuf/alarms/
+-rw-r--r--   0 fdi        (503) staff       (20)    29157 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/alarms/alarms_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    39439 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/alarms/alarms_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.678503 yamcs-client-1.9.0/src/yamcs/protobuf/archive/
+-rw-r--r--   0 fdi        (503) staff       (20)    30515 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/archive/archive_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    51245 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/archive/index_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    35584 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    19025 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/archive/rocksdb_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.678879 yamcs-client-1.9.0/src/yamcs/protobuf/audit/
+-rw-r--r--   0 fdi        (503) staff       (20)    12095 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/audit/audit_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.679736 yamcs-client-1.9.0/src/yamcs/protobuf/buckets/
+-rw-r--r--   0 fdi        (503) staff       (20)    34163 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/buckets/buckets_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.682352 yamcs-client-1.9.0/src/yamcs/protobuf/commanding/
+-rw-r--r--   0 fdi        (503) staff       (20)    12531 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/commanding/clearance_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    39217 2023-04-04 09:35:44.000000 yamcs-client-1.9.0/src/yamcs/protobuf/commanding/commanding_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    45463 2023-04-04 09:35:44.000000 yamcs-client-1.9.0/src/yamcs/protobuf/commanding/commands_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    33430 2023-04-04 09:35:44.000000 yamcs-client-1.9.0/src/yamcs/protobuf/commanding/queue_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.683005 yamcs-client-1.9.0/src/yamcs/protobuf/cop1/
+-rw-r--r--   0 fdi        (503) staff       (20)    35089 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/cop1/cop1_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.683742 yamcs-client-1.9.0/src/yamcs/protobuf/database/
+-rw-r--r--   0 fdi        (503) staff       (20)     8365 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/database/database_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.684905 yamcs-client-1.9.0/src/yamcs/protobuf/events/
+-rw-r--r--   0 fdi        (503) staff       (20)     9412 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/events/events_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    30854 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/events/events_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.685684 yamcs-client-1.9.0/src/yamcs/protobuf/filetransfer/
+-rw-r--r--   0 fdi        (503) staff       (20)    76664 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.687368 yamcs-client-1.9.0/src/yamcs/protobuf/iam/
+-rw-r--r--   0 fdi        (503) staff       (20)    73707 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/iam/iam_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8383 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/iam/sessions_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.687967 yamcs-client-1.9.0/src/yamcs/protobuf/links/
+-rw-r--r--   0 fdi        (503) staff       (20)    34775 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/links/links_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.688855 yamcs-client-1.9.0/src/yamcs/protobuf/mdb/
+-rw-r--r--   0 fdi        (503) staff       (20)   235716 2023-04-04 09:35:44.000000 yamcs-client-1.9.0/src/yamcs/protobuf/mdb/mdb_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.690190 yamcs-client-1.9.0/src/yamcs/protobuf/packets/
+-rw-r--r--   0 fdi        (503) staff       (20)     4689 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/packets/packets_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    33596 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/packets/packets_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.691529 yamcs-client-1.9.0/src/yamcs/protobuf/processing/
+-rw-r--r--   0 fdi        (503) staff       (20)    27862 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/processing/mdb_override_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    81524 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/processing/processing_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.692376 yamcs-client-1.9.0/src/yamcs/protobuf/pvalue/
+-rw-r--r--   0 fdi        (503) staff       (20)    30578 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/pvalue/pvalue_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.694939 yamcs-client-1.9.0/src/yamcs/protobuf/replication/
+-rw-r--r--   0 fdi        (503) staff       (20)    13152 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/replication/replication_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.697651 yamcs-client-1.9.0/src/yamcs/protobuf/table/
+-rw-r--r--   0 fdi        (503) staff       (20)    67468 2023-04-04 09:35:44.000000 yamcs-client-1.9.0/src/yamcs/protobuf/table/table_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.699890 yamcs-client-1.9.0/src/yamcs/protobuf/tco/
+-rw-r--r--   0 fdi        (503) staff       (20)    32904 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/tco/tco_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.721181 yamcs-client-1.9.0/src/yamcs/protobuf/time/
+-rw-r--r--   0 fdi        (503) staff       (20)    13072 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/time/time_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.721647 yamcs-client-1.9.0/src/yamcs/protobuf/timeline/
+-rw-r--r--   0 fdi        (503) staff       (20)   115941 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/timeline/timeline_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.724693 yamcs-client-1.9.0/src/yamcs/protobuf/web/
+-rw-r--r--   0 fdi        (503) staff       (20)     8530 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/web/auth_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    50999 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/web/server_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.725300 yamcs-client-1.9.0/src/yamcs/protobuf/yamcsManagement/
+-rw-r--r--   0 fdi        (503) staff       (20)   120703 2023-04-04 09:35:44.000000 yamcs-client-1.9.0/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    42560 2023-03-26 07:22:27.000000 yamcs-client-1.9.0/src/yamcs/protobuf/yamcs_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.731560 yamcs-client-1.9.0/src/yamcs/storage/
+-rw-r--r--   0 fdi        (503) staff       (20)       55 2022-04-07 19:17:50.000000 yamcs-client-1.9.0/src/yamcs/storage/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     5004 2023-04-16 20:17:32.000000 yamcs-client-1.9.0/src/yamcs/storage/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6218 2023-04-17 10:35:43.000000 yamcs-client-1.9.0/src/yamcs/storage/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.733178 yamcs-client-1.9.0/src/yamcs/tco/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs-client-1.9.0/src/yamcs/tco/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4866 2023-04-17 10:18:23.000000 yamcs-client-1.9.0/src/yamcs/tco/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     3029 2023-04-16 20:59:17.000000 yamcs-client-1.9.0/src/yamcs/tco/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.734312 yamcs-client-1.9.0/src/yamcs/timeline/
+-rw-r--r--   0 fdi        (503) staff       (20)       57 2022-05-30 08:31:08.000000 yamcs-client-1.9.0/src/yamcs/timeline/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7449 2023-04-16 19:21:44.000000 yamcs-client-1.9.0/src/yamcs/timeline/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    12658 2023-04-16 19:34:39.000000 yamcs-client-1.9.0/src/yamcs/timeline/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.735214 yamcs-client-1.9.0/src/yamcs/tmtc/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs-client-1.9.0/src/yamcs/tmtc/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)    50069 2023-05-01 11:43:07.000000 yamcs-client-1.9.0/src/yamcs/tmtc/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    33155 2023-04-17 10:35:38.000000 yamcs-client-1.9.0/src/yamcs/tmtc/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2023-05-01 12:06:56.743675 yamcs-client-1.9.0/src/yamcs_client.egg-info/
+-rw-r--r--   0 fdi        (503) staff       (20)     1510 2023-05-01 12:06:56.000000 yamcs-client-1.9.0/src/yamcs_client.egg-info/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)     2916 2023-05-01 12:06:56.000000 yamcs-client-1.9.0/src/yamcs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2023-05-01 12:06:56.000000 yamcs-client-1.9.0/src/yamcs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2022-04-07 19:46:24.000000 yamcs-client-1.9.0/src/yamcs_client.egg-info/not-zip-safe
+-rw-r--r--   0 fdi        (503) staff       (20)       54 2023-05-01 12:06:56.000000 yamcs-client-1.9.0/src/yamcs_client.egg-info/requires.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        6 2023-05-01 12:06:56.000000 yamcs-client-1.9.0/src/yamcs_client.egg-info/top_level.txt
```

### Comparing `yamcs-client-1.8.8/LICENSE` & `yamcs-client-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/PKG-INFO` & `yamcs-client-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-client
-Version: 1.8.8
+Version: 1.9.0
 Summary: Yamcs API client library
 Home-page: https://github.com/yamcs/python-yamcs-client
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `yamcs-client-1.8.8/README.md` & `yamcs-client-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/setup.py` & `yamcs-client-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/api/annotations_pb2.py` & `yamcs-client-1.9.0/src/yamcs/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/api/exception_pb2.py` & `yamcs-client-1.9.0/src/yamcs/api/exception_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/api/httpbody_pb2.py` & `yamcs-client-1.9.0/src/yamcs/api/httpbody_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/api/websocket_pb2.py` & `yamcs-client-1.9.0/src/yamcs/api/websocket_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/archive/client.py` & `yamcs-client-1.9.0/src/yamcs/archive/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,83 +1,99 @@
 import functools
 from datetime import datetime, timedelta, timezone
+from typing import Callable, Iterable, List, Optional, Union
 
 from yamcs.archive.model import (
     IndexGroup,
     ParameterRange,
     ResultSet,
     Sample,
     Stream,
     StreamData,
     Table,
 )
 from yamcs.core import pagination
+from yamcs.core.context import Context
+from yamcs.core.exceptions import YamcsError
 from yamcs.core.futures import WebSocketSubscriptionFuture
 from yamcs.core.helpers import (
     split_protobuf_stream,
     to_isostring,
     to_named_object_ids,
     to_server_time,
 )
 from yamcs.core.subscriptions import WebSocketSubscriptionManager
 from yamcs.model import Event
+from yamcs.protobuf.alarms import alarms_pb2, alarms_service_pb2
 from yamcs.protobuf.archive import (
     archive_pb2,
     index_service_pb2,
     parameter_archive_service_pb2,
 )
 from yamcs.protobuf.commanding import commands_service_pb2
 from yamcs.protobuf.events import events_service_pb2
 from yamcs.protobuf.packets import packets_pb2, packets_service_pb2
 from yamcs.protobuf.pvalue import pvalue_pb2
 from yamcs.protobuf.table import table_pb2
-from yamcs.tmtc.model import CommandHistory, Packet, ParameterData, ParameterValue
+from yamcs.tmtc.model import (
+    Alarm,
+    CommandHistory,
+    EventAlarm,
+    Packet,
+    ParameterAlarm,
+    ParameterData,
+    ParameterValue,
+)
 
 
 def _wrap_callback_parse_stream_data(subscription, on_data, message):
     """
     Wraps an (optional) user callback to parse StreamData
     from a WebSocket data message
     """
     pb = table_pb2.StreamData()
     message.Unpack(pb)
     on_data(StreamData(pb))
 
 
 class ArchiveClient:
-    def __init__(self, ctx, instance):
+    def __init__(self, ctx: Context, instance: str):
         super(ArchiveClient, self).__init__()
         self.ctx = ctx
         self._instance = instance
 
-    def list_packet_names(self):
+    def list_packet_names(self) -> Iterable[str]:
         """
         Returns the existing packet names.
-
-        :rtype: ~collections.abc.Iterable[str]
         """
         # Server does not do pagination on listings of this resource.
         # Return an iterator anyway for similarity with other API methods
         path = f"/archive/{self._instance}/packet-names"
         response = self.ctx.get_proto(path=path)
         message = packets_service_pb2.ListPacketNamesResponse()
         message.ParseFromString(response.content)
         names = getattr(message, "name")
         return iter(names)
 
-    def list_packet_histogram(self, name=None, start=None, stop=None, merge_time=2):
+    def list_packet_histogram(
+        self,
+        name: Optional[str] = None,
+        start: Optional[datetime] = None,
+        stop: Optional[datetime] = None,
+        merge_time: float = 2,
+    ) -> Iterable[IndexGroup]:
         """
         Reads packet-related index records between the specified start and stop
         time.
 
         Each iteration returns a chunk of chronologically-sorted records.
 
-        :param float merge_time: Maximum gap in seconds before two consecutive index
-                                 records are merged together.
-        :rtype: ~collections.abc.Iterable[.IndexGroup]
+        :param merge_time:
+            Maximum gap in seconds before two consecutive index
+            records are merged together.
         """
         params = {}
         if name is not None:
             params["name"] = name
         if start is not None:
             params["start"] = to_isostring(start)
         if stop is not None:
@@ -90,41 +106,43 @@
             path=f"/archive/{self._instance}/packet-index",
             params=params,
             response_class=index_service_pb2.IndexResponse,
             items_key="group",
             item_mapper=IndexGroup,
         )
 
-    def list_processed_parameter_groups(self):
+    def list_processed_parameter_groups(self) -> Iterable[str]:
         """
         Returns the existing parameter groups.
-
-        :rtype: ~collections.abc.Iterable[str]
         """
         # Server does not do pagination on listings of this resource.
         # Return an iterator anyway for similarity with other API methods
         path = f"/archive/{self._instance}/parameter-groups"
         response = self.ctx.get_proto(path=path)
         message = archive_pb2.ParameterGroupInfo()
         message.ParseFromString(response.content)
         groups = getattr(message, "group")
         return iter(groups)
 
     def list_processed_parameter_group_histogram(
-        self, group=None, start=None, stop=None, merge_time=20
-    ):
+        self,
+        group: Optional[str] = None,
+        start: Optional[datetime] = None,
+        stop: Optional[datetime] = None,
+        merge_time: float = 20,
+    ) -> Iterable[IndexGroup]:
         """
         Reads index records related to processed parameter groups between the
         specified start and stop time.
 
         Each iteration returns a chunk of chronologically-sorted records.
 
-        :param float merge_time: Maximum gap in seconds before two consecutive index
-                                 records are merged together.
-        :rtype: ~collections.abc.Iterable[.IndexGroup]
+        :param merge_time:
+            Maximum gap in seconds before two consecutive index
+            records are merged together.
         """
         params = {}
         if group is not None:
             params["group"] = group
         if start is not None:
             params["start"] = to_isostring(start)
         if stop is not None:
@@ -137,39 +155,43 @@
             path=f"/archive/{self._instance}/parameter-index",
             params=params,
             response_class=index_service_pb2.IndexResponse,
             items_key="group",
             item_mapper=IndexGroup,
         )
 
-    def list_event_sources(self):
+    def list_event_sources(self) -> Iterable[str]:
         """
         Returns the existing event sources.
-
-        :rtype: ~collections.abc.Iterable[str]
         """
         # Server does not do pagination on listings of this resource.
         # Return an iterator anyway for similarity with other API methods
         path = f"/archive/{self._instance}/events/sources"
         response = self.ctx.get_proto(path=path)
         message = events_service_pb2.ListEventSourcesResponse()
         message.ParseFromString(response.content)
         sources = getattr(message, "source")
         return iter(sources)
 
-    def list_event_histogram(self, source=None, start=None, stop=None, merge_time=2):
+    def list_event_histogram(
+        self,
+        source: Optional[str] = None,
+        start: Optional[datetime] = None,
+        stop: Optional[datetime] = None,
+        merge_time: float = 2,
+    ) -> Iterable[IndexGroup]:
         """
         Reads event-related index records between the specified start and stop
         time.
 
         Each iteration returns a chunk of chronologically-sorted records.
 
-        :param float merge_time: Maximum gap in seconds before two consecutive index
-                                 records are merged together.
-        :rtype: ~collections.abc.Iterable[.IndexGroup]
+        :param merge_time:
+            Maximum gap in seconds before two consecutive index
+            records are merged together.
         """
         params = {}
         if source is not None:
             params["source"] = source
         if start is not None:
             params["start"] = to_isostring(start)
         if stop is not None:
@@ -182,24 +204,30 @@
             path=f"/archive/{self._instance}/event-index",
             params=params,
             response_class=index_service_pb2.IndexResponse,
             items_key="group",
             item_mapper=IndexGroup,
         )
 
-    def list_command_histogram(self, name=None, start=None, stop=None, merge_time=2):
+    def list_command_histogram(
+        self,
+        name: Optional[str] = None,
+        start: Optional[datetime] = None,
+        stop: Optional[datetime] = None,
+        merge_time: float = 2,
+    ) -> Iterable[IndexGroup]:
         """
         Reads command-related index records between the specified start and stop
         time.
 
         Each iteration returns a chunk of chronologically-sorted records.
 
-        :param float merge_time: Maximum gap in seconds before two consecutive index
-                                 records are merged together.
-        :rtype: ~collections.abc.Iterable[.IndexGroup]
+        :param merge_time:
+            Maximum gap in seconds before two consecutive index
+            records are merged together.
         """
         params = {}
         if name is not None:
             params["name"] = name
         if start is not None:
             params["start"] = to_isostring(start)
         if stop is not None:
@@ -212,22 +240,22 @@
             path=f"/archive/{self._instance}/command-index",
             params=params,
             response_class=index_service_pb2.IndexResponse,
             items_key="group",
             item_mapper=IndexGroup,
         )
 
-    def list_completeness_index(self, start=None, stop=None):
+    def list_completeness_index(
+        self, start: Optional[datetime] = None, stop: Optional[datetime] = None
+    ) -> Iterable[IndexGroup]:
         """
         Reads completeness index records between the specified start and stop
         time.
 
         Each iteration returns a chunk of chronologically-sorted records.
-
-        :rtype: ~collections.abc.Iterable[.IndexGroup]
         """
         params = {}
         if start is not None:
             params["start"] = to_isostring(start)
         if stop is not None:
             params["stop"] = to_isostring(stop)
 
@@ -236,34 +264,98 @@
             path=f"/archive/{self._instance}/completeness-index",
             params=params,
             response_class=index_service_pb2.IndexResponse,
             items_key="group",
             item_mapper=IndexGroup,
         )
 
+    def list_alarms(
+        self,
+        name: Optional[str] = None,
+        start: Optional[datetime] = None,
+        stop: Optional[datetime] = None,
+        page_size: int = 500,
+        descending: bool = False,
+    ) -> Iterable[Alarm]:
+        """
+        Reads alarm information between the specified start and stop time.
+
+        Alarms are sorted by trigger time, name and sequence number.
+
+        :param name:
+            Filter by alarm name
+        :param start:
+            Minimum trigger time (inclusive)
+        :param stop:
+            Maximum trigger time (exclusive)
+        :param page_size:
+            Page size of underlying requests. Higher values imply
+            less overhead, but risk hitting the maximum message size
+            limit.
+        :param descending:
+            If set to ``True`` alarms are fetched in reverse
+            order (most recent first).
+        """
+        params = {
+            "order": "desc" if descending else "asc",
+        }
+        if name is not None:
+            params["name"] = name
+        if page_size is not None:
+            params["limit"] = page_size
+        if start is not None:
+            params["start"] = to_isostring(start)
+        if stop is not None:
+            params["stop"] = to_isostring(stop)
+
+        # TODO change to pagination iterator in time. continuationToken support only
+        # added recently.
+        path = f"/archive/{self._instance}/alarms"
+        response = self.ctx.get_proto(path=path, params=params)
+        message = alarms_service_pb2.ListAlarmsResponse()
+        message.ParseFromString(response.content)
+
+        alarms = []
+        for proto in getattr(message, "alarms"):
+            if proto.type == alarms_pb2.PARAMETER:
+                alarms.append(ParameterAlarm(proto))
+            elif proto.type == alarms_pb2.EVENT:
+                alarms.append(EventAlarm(proto))
+            else:
+                raise YamcsError("Unexpected type " + str(proto.type))
+
+        return iter(alarms)
+
     def list_packets(
-        self, name=None, start=None, stop=None, page_size=500, descending=False
-    ):
+        self,
+        name: Optional[str] = None,
+        start: Optional[datetime] = None,
+        stop: Optional[datetime] = None,
+        page_size: int = 500,
+        descending: bool = False,
+    ) -> Iterable[Packet]:
         """
         Reads packet information between the specified start and stop
         time.
 
         Packets are sorted by generation time and sequence number.
 
-        :param str name: Archived name of the packet
-        :param ~datetime.datetime start: Minimum generation time of the returned
-                                         packets (inclusive)
-        :param ~datetime.datetime stop: Maximum generation time of the returned
-                                        packets (exclusive)
-        :param int page_size: Page size of underlying requests. Higher values imply
-                              less overhead, but risk hitting the maximum message size
-                              limit.
-        :param bool descending: If set to ``True`` packets are fetched in reverse
-                                order (most recent first).
-        :rtype: ~collections.abc.Iterable[.Packet]
+        :param name:
+            Archived name of the packet
+        :param start:
+            Minimum generation time of the returned packets (inclusive)
+        :param stop:
+            Maximum generation time of the returned packets (exclusive)
+        :param page_size:
+            Page size of underlying requests. Higher values imply
+            less overhead, but risk hitting the maximum message size
+            limit.
+        :param descending:
+            If set to ``True`` packets are fetched in reverse
+            order (most recent first).
         """
         params = {
             "order": "desc" if descending else "asc",
         }
         if name is not None:
             params["name"] = name
         if page_size is not None:
@@ -278,42 +370,50 @@
             path=f"/archive/{self._instance}/packets",
             params=params,
             response_class=packets_service_pb2.ListPacketsResponse,
             items_key="packet",
             item_mapper=Packet,
         )
 
-    def get_packet(self, generation_time, sequence_number):
+    def get_packet(self, generation_time: datetime, sequence_number: int) -> Packet:
         """
         Gets a single packet by its identifying key (gentime, seqNum).
 
-        :param ~datetime.datetime generation_time: When the packet was generated
-                                                   (packet time)
-        :param int sequence_number: Sequence number of the packet
-        :rtype: .Packet
+        :param generation_time:
+            When the packet was generated (packet time)
+        :param sequence_number:
+            Sequence number of the packet
         """
         url = f"/archive/{self._instance}/packets/"
         url += f"{to_isostring(generation_time)}/{sequence_number}"
         response = self.ctx.get_proto(url)
         message = packets_pb2.TmPacketData()
         message.ParseFromString(response.content)
         return Packet(message)
 
-    def export_packets(self, name=None, start=None, stop=None, chunk_size=1024):
+    def export_packets(
+        self,
+        name: Optional[str] = None,
+        start: Optional[datetime] = None,
+        stop: Optional[datetime] = None,
+        chunk_size: int = 1024,
+    ) -> Iterable:
         """
         Export raw packets.
 
         Packets are sorted by generation time and sequence number.
 
-        :param str name: Archived name of the packet
-        :param ~datetime.datetime start: Minimum generation time of the returned
-                                         packets (inclusive)
-        :param ~datetime.datetime stop: Maximum generation time of the returned
-                                        packets (exclusive)
-        :rtype: An iterator over received chunks
+        :param name:
+            Archived name of the packet
+        :param start:
+            Minimum generation time of the returned packets (inclusive)
+        :param stop:
+            Maximum generation time of the returned packets (exclusive)
+        :return:
+            An iterator over received chunks
         """
         params = {}
         if name is not None:
             params["name"] = name
         if start is not None:
             params["start"] = to_isostring(start)
         if stop is not None:
@@ -321,42 +421,46 @@
 
         path = f"/archive/{self._instance}:exportPackets"
         response = self.ctx.get_proto(path=path, params=params, stream=True)
         return response.iter_content(chunk_size=chunk_size)
 
     def list_events(
         self,
-        source=None,
-        severity=None,
-        text_filter=None,
-        start=None,
-        stop=None,
-        page_size=500,
-        descending=False,
-    ):
+        source: Optional[str] = None,
+        severity: Optional[str] = None,
+        text_filter: Optional[str] = None,
+        start: Optional[datetime] = None,
+        stop: Optional[datetime] = None,
+        page_size: int = 500,
+        descending: bool = False,
+    ) -> Iterable[Event]:
         """
         Reads events between the specified start and stop time.
 
         Events are sorted by generation time, source, then sequence number.
 
-        :param str source: The source of the returned events.
-        :param str severity: The minimum severity level of the returned events.
-                             One of ``INFO``, ``WATCH``, ``WARNING``, ``DISTRESS``,
-                             ``CRITICAL`` or ``SEVERE``.
-        :param str text_filter: Filter the text message of the returned events
-        :param ~datetime.datetime start: Minimum start date of the returned events
-                                         (inclusive)
-        :param ~datetime.datetime stop: Maximum start date of the returned events
-                                        (exclusive)
-        :param int page_size: Page size of underlying requests. Higher values imply
-                              less overhead, but risk hitting the maximum message size
-                              limit.
-        :param bool descending: If set to ``True`` events are fetched in reverse
-                                order (most recent first).
-        :rtype: ~collections.abc.Iterable[.Event]
+        :param source:
+            The source of the returned events.
+        :param severity:
+            The minimum severity level of the returned events.
+            One of ``INFO``, ``WATCH``, ``WARNING``, ``DISTRESS``,
+            ``CRITICAL`` or ``SEVERE``.
+        :param text_filter:
+            Filter the text message of the returned events
+        :param start:
+            Minimum start date of the returned events (inclusive)
+        :param stop:
+            Maximum start date of the returned events (exclusive)
+        :param page_size:
+            Page size of underlying requests. Higher values imply
+            less overhead, but risk hitting the maximum message size
+            limit.
+        :param descending:
+            If set to ``True`` events are fetched in reverse
+            order (most recent first).
         """
         params = {
             "order": "desc" if descending else "asc",
         }
         if source is not None:
             params["source"] = source
         if page_size is not None:
@@ -377,56 +481,61 @@
             response_class=events_service_pb2.ListEventsResponse,
             items_key="event",
             item_mapper=Event,
         )
 
     def sample_parameter_values(
         self,
-        parameter,
-        start=None,
-        stop=None,
-        sample_count=500,
-        parameter_cache="realtime",
-        source="ParameterArchive",
-    ):
+        parameter: str,
+        start: Optional[datetime] = None,
+        stop: Optional[datetime] = None,
+        sample_count: int = 500,
+        parameter_cache: str = "realtime",
+        source: str = "ParameterArchive",
+    ) -> List[Sample]:
         """
         Returns parameter samples.
 
         The query range is split in sample intervals of equal length. For
         each interval a :class:`.Sample` is returned which describes the
         min, max, count and avg during that interval.
 
         Note that sample times are determined without considering the
         actual parameter values. Two separate queries with equal start/stop
         arguments will always return the same number of samples with the
         same timestamps. This is done to ease merging of multiple sample
         series. You should always be explicit about the ``start`` and ``stop``
         times when relying on this property.
 
-        :param str parameter: Either a fully-qualified XTCE name or an alias in the
-                              format ``NAMESPACE/NAME``.
-        :param ~datetime.datetime start: Minimum generation time of the sampled
-                                         parameter values (inclusive). If not set
-                                         this defaults to one hour ago.
-        :param ~datetime.datetime stop: Maximum generation time of the sampled
-                                        parameter values (exclusive). If not set
-                                        this defaults to the current time.
-        :param int sample_count: The number of returned samples.
-        :param str parameter_cache: Specify the name of the processor who's
-                                    parameter cache is merged with already
-                                    archived values. To disable results from
-                                    the parameter cache, set this to ``None``.
-        :param str source: Specify how to retrieve parameter values. By
-                           default this uses the ``ParameterArchive`` which
-                           is optimized for retrieval. For Yamcs instances
-                           that do not enable the ``ParameterArchive``, you can
-                           still get results by specifying ``replay`` as the
-                           source. Replay requests take longer to return because
-                           the data needs to be reprocessed.
-        :rtype: .Sample[]
+        :param parameter:
+            Either a fully-qualified XTCE name or an alias in the
+            format ``NAMESPACE/NAME``.
+        :param start:
+            Minimum generation time of the sampled
+            parameter values (inclusive). If not set
+            this defaults to one hour ago.
+        :param stop:
+            Maximum generation time of the sampled
+            parameter values (exclusive). If not set
+            this defaults to the current time.
+        :param sample_count:
+            The number of returned samples.
+        :param parameter_cache:
+            Specify the name of the processor who's
+            parameter cache is merged with already
+            archived values. To disable results from
+            the parameter cache, set this to ``None``.
+        :param source:
+            Specify how to retrieve parameter values. By
+            default this uses the ``ParameterArchive`` which
+            is optimized for retrieval. For Yamcs instances
+            that do not enable the ``ParameterArchive``, you can
+            still get results by specifying ``replay`` as the
+            source. Replay requests take longer to return because
+            the data needs to be reprocessed.
         """
         path = f"/archive/{self._instance}/parameters{parameter}/samples"
         now = datetime.now(tz=timezone.utc)
         params = {
             "count": sample_count,
             "source": source,
             "start": to_isostring(now - timedelta(hours=1)),
@@ -446,70 +555,71 @@
         message = pvalue_pb2.TimeSeries()
         message.ParseFromString(response.content)
         samples = getattr(message, "sample")
         return [Sample(s) for s in samples]
 
     def list_parameter_ranges(
         self,
-        parameter,
-        start=None,
-        stop=None,
-        min_gap=None,
-        max_gap=None,
-        min_range=None,
-        max_values=100,
-        parameter_cache="realtime",
-    ):
+        parameter: str,
+        start: Optional[datetime] = None,
+        stop: Optional[datetime] = None,
+        min_gap: Optional[float] = None,
+        max_gap: Optional[float] = None,
+        min_range: Optional[float] = None,
+        max_values: int = 100,
+        parameter_cache: str = "realtime",
+    ) -> List[ParameterRange]:
         """
         Returns parameter ranges between the specified start and stop time.
 
         Each range indicates an interval during which this parameter's
         value was uninterrupted and unchanged.
 
         Ranges are a good fit for retrieving the value of a parameter
         that does not change frequently. For example an on/off indicator
         or some operational status. Querying ranges will then induce
         much less overhead than manually processing the output of
         :meth:`list_parameter_values` would.
 
         The maximum number of returned ranges is limited to 500.
 
-        :param str parameter: Either a fully-qualified XTCE name or an alias in the
-                              format ``NAMESPACE/NAME``.
-        :param start: Minimum generation time of the considered values (inclusive)
-        :type start: Optional[~datetime.datetime]
-        :param stop: Maximum generation time of the considered values (exclusive)
-        :type stop: Optional[~datetime.datetime]
-        :param min_gap: Time in seconds. Any gap (detected based on parameter
-                        expiration) smaller than this will be ignored.
-                        However if the parameter changes value, the ranges
-                        will still be split.
-        :type max_gap: Optional[float]
-        :param max_gap: Time in seconds. If the distance between two
-                        subsequent parameter values is bigger than
-                        this value (but smaller than the parameter
-                        expiration), then an artificial gap is
-                        created. This also applies if there is no
-                        expiration defined for the parameter.
-        :type max_gap: Optional[float]
-        :param min_range: Time in seconds. Minimum duration of returned
-                          ranges. If multiple values occur within the
-                          range, the most frequent can be accessed using
-                          the ``entries`` property.
-        :type min_range: Optional[float]
-        :param max_values: Maximum number of unique values, tallied across the
-                           full requested range. Use this in combination with
-                           ``min_range`` to further optimize for transfer size.
-                           This value is limited to 100 at most.
-        :param str parameter_cache: Specify the name of the processor who's
-                                    parameter cache is merged with already
-                                    archived values. To disable results from
-                                    the parameter cache, set this to ``None``.
-        :type parameter_cache: Optional[str]
-        :rtype: .ParameterRange[]
+        :param parameter:
+            Either a fully-qualified XTCE name or an alias in the
+            format ``NAMESPACE/NAME``.
+        :param start:
+            Minimum generation time of the considered values (inclusive)
+        :param stop:
+            Maximum generation time of the considered values (exclusive)
+        :param min_gap:
+            Time in seconds. Any gap (detected based on parameter
+            expiration) smaller than this will be ignored.
+            However if the parameter changes value, the ranges
+            will still be split.
+        :param max_gap:
+            Time in seconds. If the distance between two
+            subsequent parameter values is bigger than
+            this value (but smaller than the parameter
+            expiration), then an artificial gap is
+            created. This also applies if there is no
+            expiration defined for the parameter.
+        :param min_range:
+            Time in seconds. Minimum duration of returned
+            ranges. If multiple values occur within the
+            range, the most frequent can be accessed using
+            the ``entries`` property.
+        :param max_values:
+            Maximum number of unique values, tallied across the
+            full requested range. Use this in combination with
+            ``min_range`` to further optimize for transfer size.
+            This value is limited to 100 at most.
+        :param parameter_cache:
+            Specify the name of the processor who's
+            parameter cache is merged with already
+            archived values. To disable results from
+            the parameter cache, set this to ``None``.
         """
         path = f"/archive/{self._instance}/parameters{parameter}/ranges"
         params = {}
         if start is not None:
             params["start"] = to_isostring(start)
         if stop is not None:
             params["stop"] = to_isostring(stop)
@@ -531,56 +641,60 @@
         message = pvalue_pb2.Ranges()
         message.ParseFromString(response.content)
         ranges = getattr(message, "range")
         return [ParameterRange(r) for r in ranges]
 
     def list_parameter_values(
         self,
-        parameter,
-        start=None,
-        stop=None,
-        page_size=500,
-        descending=False,
-        parameter_cache="realtime",
-        source="ParameterArchive",
-    ):
+        parameter: str,
+        start: Optional[datetime] = None,
+        stop: Optional[datetime] = None,
+        page_size: int = 500,
+        descending: bool = False,
+        parameter_cache: str = "realtime",
+        source: str = "ParameterArchive",
+    ) -> Iterable[ParameterValue]:
         """
         Reads parameter values between the specified start and stop time.
 
         .. note::
 
             This method will send out multiple requests when more than
             ``page_size`` values are queried. For large queries, consider
             using :meth:`stream_parameter_values` instead, it uses server-streaming
             based on a single request, and supports downloading the values of
             multiple parameter at the same time.
 
-        :param str parameter: Either a fully-qualified XTCE name or an alias in the
-                              format ``NAMESPACE/NAME``.
-        :param ~datetime.datetime start: Minimum generation time of the returned
-                                         values (inclusive)
-        :param ~datetime.datetime stop: Maximum generation time of the returned
-                                        values (exclusive)
-        :param int page_size: Page size of underlying requests. Higher values imply
-                              less overhead, but risk hitting the maximum message size
-                              limit.
-        :param bool descending: If set to ``True`` values are fetched in reverse
-                                order (most recent first).
-        :param str parameter_cache: Specify the name of the processor who's
-                                    parameter cache is merged with already
-                                    archived values. To disable results from
-                                    the parameter cache, set this to ``None``.
-        :param str source: Specify how to retrieve parameter values. By
-                           default this uses the ``ParameterArchive`` which
-                           is optimized for retrieval. For Yamcs instances
-                           that do not enable the ``ParameterArchive``, you can
-                           still get results by specifying ``replay`` as the
-                           source. Replay requests take longer to return because
-                           the data needs to be reprocessed.
-        :rtype: ~collections.abc.Iterable[.ParameterValue]
+        :param parameter:
+            Either a fully-qualified XTCE name or an alias in the
+            format ``NAMESPACE/NAME``.
+        :param start:
+            Minimum generation time of the returned values (inclusive)
+        :param stop:
+            Maximum generation time of the returned values (exclusive)
+        :param page_size:
+            Page size of underlying requests. Higher values imply
+            less overhead, but risk hitting the maximum message size
+            limit.
+        :param descending:
+            If set to ``True`` values are fetched in reverse
+            order (most recent first).
+        :param parameter_cache:
+            Specify the name of the processor who's
+            parameter cache is merged with already
+            archived values. To disable results from
+            the parameter cache, set this to ``None``.
+        :param source:
+            Specify how to retrieve parameter values. By
+            default this uses the ``ParameterArchive`` which
+            is optimized for retrieval. For Yamcs instances
+            that do not enable the ``ParameterArchive``, you can
+            still get results by specifying ``replay`` as the
+            source. Replay requests take longer to return because
+            the data needs to be reprocessed.
         """
         params = {
             "source": source,
             "order": "desc" if descending else "asc",
         }
         if page_size is not None:
             params["limit"] = page_size
@@ -600,40 +714,40 @@
             params=params,
             response_class=archive_pb2.ListParameterHistoryResponse,
             items_key="parameter",
             item_mapper=ParameterValue,
         )
 
     def stream_parameter_values(
-        self, parameters, start=None, stop=None, tm_links=None, chunk_size=32 * 1024
-    ):
+        self,
+        parameters: Union[str, List[str]],
+        start: Optional[datetime] = None,
+        stop: Optional[datetime] = None,
+        tm_links: Optional[Union[str, List[str]]] = None,
+        chunk_size: int = 32 * 1024,
+    ) -> Iterable[ParameterData]:
         """
         Reads parameter values between the specified start and stop time.
 
         Value updates are emitted for each unique generation time within
         the queried range. If one of the parameters does not have a value
         for a specific generation time, it is not included in the update.
 
-        :param parameters: Parameter(s) to be queried.
-        :type parameters: Union[str, str[]]
+        :param parameters:
+            Parameter(s) to be queried.
+        :param start:
+            Minimum generation time of the returned values (inclusive)
+        :param stop:
+            Maximum generation time of the returned values (exclusive)
+        :param tm_links:
+            If set, include only values that were received through
+            a specific link.
 
-        :param ~datetime.datetime start: Minimum generation time of the returned
-                                         values (inclusive)
-
-        :param ~datetime.datetime stop: Maximum generation time of the returned
-                                        values (exclusive)
-
-        :param tm_links: If set, include only values that were received through
-                         a specific link.
-
-                         .. versionadded:: 1.8.4
-                            Compatible with Yamcs 5.7.4 onwards
-        :type tm_links: Union[str, str[]]
-
-        :rtype: ~collections.abc.Iterable[.ParameterData]
+            .. versionadded:: 1.8.4
+               Compatible with Yamcs 5.7.4 onwards
         """
         options = archive_pb2.StreamParameterValuesRequest()
         options.ids.extend(to_named_object_ids(parameters))
         if start is not None:
             options.start.MergeFrom(to_server_time(start))
         if stop is not None:
             options.stop.MergeFrom(to_server_time(stop))
@@ -653,37 +767,42 @@
             ):
                 yield ParameterData(message)
 
         return generate()
 
     def list_command_history(
         self,
-        command=None,
-        queue=None,
-        start=None,
-        stop=None,
-        page_size=500,
-        descending=False,
-    ):
+        command: Optional[str] = None,
+        queue: Optional[str] = None,
+        start: Optional[datetime] = None,
+        stop: Optional[datetime] = None,
+        page_size: int = 500,
+        descending: bool = False,
+    ) -> Iterable[CommandHistory]:
         """
         Reads command history entries between the specified start and stop time.
 
-        :param str command: Either a fully-qualified XTCE name or an alias in the
-                            format ``NAMESPACE/NAME``.
-        :param str queue: Name of the queue that the command was assigned to.
-        :param ~datetime.datetime start: Minimum generation time of the returned
-                                         command history entries (inclusive)
-        :param ~datetime.datetime stop: Maximum generation time of the returned
-                                        command history entries (exclusive)
-        :param int page_size: Page size of underlying requests. Higher values imply
-                              less overhead, but risk hitting the maximum message size
-                              limit.
-        :param bool descending: If set to ``True`` results are fetched in reverse
-                                order (most recent first).
-        :rtype: ~collections.abc.Iterable[.CommandHistory]
+        :param command:
+            Either a fully-qualified XTCE name or an alias in the
+            format ``NAMESPACE/NAME``.
+        :param queue:
+            Name of the queue that the command was assigned to.
+        :param start:
+            Minimum generation time of the returned
+            command history entries (inclusive)
+        :param stop:
+            Maximum generation time of the returned
+            command history entries (exclusive)
+        :param page_size:
+            Page size of underlying requests. Higher values imply
+            less overhead, but risk hitting the maximum message size
+            limit.
+        :param descending:
+            If set to ``True`` results are fetched in reverse
+            order (most recent first).
         """
         params = {
             "order": "desc" if descending else "asc",
         }
         if queue:
             params["queue"] = queue
         if page_size is not None:
@@ -703,50 +822,57 @@
             path=path,
             params=params,
             response_class=commands_service_pb2.ListCommandsResponse,
             items_key="entry",
             item_mapper=CommandHistory,
         )
 
-    def list_tables(self):
+    def list_tables(self) -> Iterable[Table]:
         """
         Returns the existing tables.
 
         Tables are returned in lexicographical order.
-
-        :rtype: ~collections.abc.Iterable[.Table]
         """
         # Server does not do pagination on listings of this resource.
         # Return an iterator anyway for similarity with other API methods
         path = f"/archive/{self._instance}/tables"
         response = self.ctx.get_proto(path=path)
         message = table_pb2.ListTablesResponse()
         message.ParseFromString(response.content)
         tables = getattr(message, "tables")
         return iter([Table(table) for table in tables])
 
-    def get_table(self, table):
+    def get_table(self, table: str) -> Table:
         """
         Gets a single table.
 
-        :param str table: The name of the table.
-        :rtype: .Table
+        :param table:
+            The name of the table.
         """
         path = f"/archive/{self._instance}/tables/{table}"
         response = self.ctx.get_proto(path=path)
         message = table_pb2.TableInfo()
         message.ParseFromString(response.content)
         return Table(message)
 
-    def dump_table(self, table, chunk_size=32 * 1024):
+    def dump_table(
+        self, table: str, query: Optional[str] = None, chunk_size: int = 32 * 1024
+    ):
         path = f"/archive/{self._instance}/tables/{table}:readRows"
-        response = self.ctx.post_proto(path=path, stream=True)
+        if query:
+            req = table_pb2.ReadRowsRequest()
+            req.query = query
+            response = self.ctx.post_proto(
+                path=path, stream=True, data=req.SerializeToString()
+            )
+        else:
+            response = self.ctx.post_proto(path=path, stream=True)
         return response.iter_content(chunk_size=chunk_size)
 
-    def load_table(self, table, data, chunk_size=32 * 1024):
+    def load_table(self, table: str, data, chunk_size: int = 32 * 1024) -> int:
         def read_in_chunks(file_object, chunk_size):
             chunk = file_object.read(chunk_size)
             while chunk:
                 yield chunk
                 chunk = file_object.read(chunk_size)
 
         path = f"/archive/{self._instance}/tables/{table}:writeRows"
@@ -755,109 +881,118 @@
             response = self.ctx.post_proto(path=path, data=generator)
         else:
             response = self.ctx.post_proto(path=path, data=data)
         message = table_pb2.WriteRowsResponse()
         message.ParseFromString(response.content)
         return message.count
 
-    def rebuild_histogram(self, table, start=None, stop=None):
+    def rebuild_histogram(
+        self,
+        table: str,
+        start: Optional[datetime] = None,
+        stop: Optional[datetime] = None,
+    ):
         """
         Rebuilds the histogram for a table. This may be necessary
         for example after bulk loading data.
 
         The rebuild may be constrained by using the
         ``start`` and ``stop`` parameters. When
         specified all partitions overlapping this range
         are reconsidered.
 
         .. note::
             Histogram rebuilds run synchronously: this
             method will await the outcome.
 
-        :param str table: The name of the table
-        :param start: Start time
-        :type start: Optional[~datetime.datetime]
-        :param stop: Stop time
-        :type stop: Optional[~datetime.datetime]
+        :param table:
+            The name of the table
+        :param start:
+            Start time
+        :param stop:
+            Stop time
         """
         req = table_pb2.RebuildHistogramRequest()
         if start:
             req.start.MergeFrom(to_server_time(start))
         if stop:
             req.stop.MergeFrom(to_server_time(stop))
         url = f"/archive/{self._instance}/tables/{table}:rebuildHistogram"
         self.ctx.post_proto(url, data=req.SerializeToString())
 
-    def rebuild_parameter_archive(self, start, stop):
+    def rebuild_parameter_archive(self, start: datetime, stop: datetime):
         """
         Rebuilds the Parameter Archive.
 
         The rebuild must be constrained by using the
         ``start`` and ``stop`` parameters. This values
         are only hints to the Parameter Archive, which
         will extend the requested range based on archive
         segmentation.
 
         .. note::
             Rebuilds run as an asynchronous operation: this
             method will not await the outcome.
 
-        :param start: Start time
-        :type start: ~datetime.datetime
-        :param stop: Stop time
-        :type stop: ~datetime.datetime
+        :param start:
+            Start time
+        :param stop:
+            Stop time
         """
         req = parameter_archive_service_pb2.RebuildRangeRequest()
         req.start.MergeFrom(to_server_time(start))
         req.stop.MergeFrom(to_server_time(stop))
         url = f"/archive/{self._instance}/parameterArchive:rebuild"
         self.ctx.post_proto(url, data=req.SerializeToString())
 
-    def list_streams(self):
+    def list_streams(self) -> Iterable[Stream]:
         """
         Returns the existing streams.
 
         Streams are returned in lexicographical order.
-
-        :rtype: ~collections.abc.Iterable[.Stream]
         """
         # Server does not do pagination on listings of this resource.
         # Return an iterator anyway for similarity with other API methods
         path = f"/archive/{self._instance}/streams"
         response = self.ctx.get_proto(path=path)
         message = table_pb2.ListStreamsResponse()
         message.ParseFromString(response.content)
         streams = getattr(message, "streams")
         return iter([Stream(stream) for stream in streams])
 
-    def get_stream(self, stream):
+    def get_stream(self, stream: str) -> Stream:
         """
         Gets a single stream.
 
-        :param str stream: The name of the stream.
-        :rtype: .Stream
+        :param stream:
+            The name of the stream.
         """
         path = f"/archive/{self._instance}/streams/{stream}"
         response = self.ctx.get_proto(path=path)
         message = table_pb2.StreamInfo()
         message.ParseFromString(response.content)
         return Stream(message)
 
-    def create_stream_subscription(self, stream, on_data, timeout=60):
+    def create_stream_subscription(
+        self, stream: str, on_data: Callable[[StreamData], None], timeout: float = 60
+    ) -> WebSocketSubscriptionFuture:
         """
         Create a new stream subscription.
 
-        :param str stream: The name of the stream.
-        :param on_data: Function that gets called with  :class:`.StreamData`
-                        updates.
-        :param float timeout: The amount of seconds to wait for the request
-                              to complete.
-        :return: Future that can be used to manage the background websocket
-                 subscription
-        :rtype: .WebSocketSubscriptionFuture
+        :param stream:
+            The name of the stream.
+        :param on_data:
+            Function that gets called with  :class:`.StreamData`
+            updates.
+        :param timeout:
+            The amount of seconds to wait for the request
+            to complete.
+        :return:
+            Future that can be used to manage the background websocket
+            subscription.
         """
         options = table_pb2.SubscribeStreamRequest()
         options.instance = self._instance
         options.stream = stream
 
         manager = WebSocketSubscriptionManager(
             self.ctx, topic="stream", options=options
@@ -873,21 +1008,22 @@
         manager.open(wrapped_callback)
 
         # Wait until a reply or exception is received
         subscription.reply(timeout=timeout)
 
         return subscription
 
-    def execute_sql(self, statement):
+    def execute_sql(self, statement: str) -> ResultSet:
         """
         Executes a single SQL statement.
 
-        :param statement: SQL string
-        :return: A result set for consuming rows
-        :rtype: .ResultSet
+        :param statement:
+            SQL string
+        :return:
+            A result set for consuming rows
         """
         path = f"/archive/{self._instance}:executeStreamingSql"
         req = table_pb2.ExecuteSqlRequest()
         req.statement = statement
 
         response = self.ctx.post_proto(
             path=path, data=req.SerializeToString(), stream=True
```

### Comparing `yamcs-client-1.8.8/src/yamcs/archive/model.py` & `yamcs-client-1.9.0/src/yamcs/archive/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,70 @@
+import datetime
+from typing import Any, List, Optional
+
 from google.protobuf.internal.decoder import _DecodeVarint32
 from yamcs.core.helpers import parse_server_time, parse_server_timestring, parse_value
 from yamcs.protobuf.table import table_pb2
 
 
 class Table:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Table name."""
         return self._proto.name
 
     def __str__(self):
         return self.name
 
 
 class Stream:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Stream name."""
         return self._proto.name
 
     def __str__(self):
         return self.name
 
 
 class StreamData:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def stream(self):
+    def stream(self) -> str:
         """Stream name."""
         return self._proto.stream
 
     @property
-    def columns(self):
+    def columns(self) -> List['ColumnData']:
         """Tuple columns."""
         return [ColumnData(c) for c in self._proto.column]
 
     def __str__(self):
         return f"{self.stream} ({len(self.columns)} columns)"
 
 
 class ColumnData:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Column name."""
         return self._proto.name
 
     @property
-    def value(self):
+    def value(self) -> Any:
         """Value for this column."""
         return parse_value(self._proto.value)
 
     def __str__(self):
         return f"{self.name}: {self.value}"
 
 
@@ -100,31 +103,27 @@
                 if self._columns_proto is None:
                     self._columns_proto = message.columns
                 for row_proto in message.rows:
                     values = [parse_value(v) for v in row_proto.values]
                     yield values
 
     @property
-    def columns(self):
+    def columns(self) -> Optional[List[str]]:
         """
         Column names. This returns ``None`` as long as no row has
         been consumed yet.
-
-        :type: str[]
         """
         if self._columns_proto is not None:
             return [c.name for c in self._columns_proto]
         return None
 
     @property
-    def column_types(self):
+    def column_types(self) -> Optional[List[str]]:
         """
         Column types.
-
-        :type: str[]
         """
         if self._columns_proto is not None:
             return [c.type for c in self._columns_proto]
         return None
 
 
 class IndexGroup:
@@ -133,32 +132,30 @@
     type of underlying objects.
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """
         Name associated with this group. The meaning is defined
         by the objects represented by this index. For example:
 
         * In an index of events, index records are grouped by ``source``.
         * In an index of packets, index records are grouped by ``packet name``.
         """
         if self._proto.HasField("id"):
             return self._proto.id.name
         return None
 
     @property
-    def records(self):
+    def records(self) -> List['IndexRecord']:
         """
         Index records within this group
-
-        :type: List[:class:`.IndexRecord`]
         """
         return [IndexRecord(rec) for rec in self._proto.entry]
 
     def __str__(self):
         return f"{self.name} ({len(self.records)} records)"
 
 
@@ -169,33 +166,29 @@
     ``merge_time``.
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def start(self):
+    def start(self) -> datetime.datetime:
         """
         Start time of the record
-
-        :type: :class:`~datetime.datetime`
         """
         return parse_server_timestring(self._proto.start)
 
     @property
-    def stop(self):
+    def stop(self) -> datetime.datetime:
         """
         Stop time of the record
-
-        :type: :class:`~datetime.datetime`
         """
         return parse_server_timestring(self._proto.stop)
 
     @property
-    def count(self):
+    def count(self) -> int:
         """
         Number of underlying objects this index record represents
         """
         return self._proto.count
 
     def __str__(self):
         return f"{self.start} - {self.stop} (n={self.count})"
@@ -207,45 +200,43 @@
     values.
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def time(self):
+    def time(self) -> datetime.datetime:
         """
         Sample time.
-
-        :type: :class:`~datetime.datetime`
         """
         return parse_server_time(self._proto.time)
 
     @property
-    def avg(self):
+    def avg(self) -> Optional[float]:
         """Average value."""
         if self._proto.HasField("avg"):
             return self._proto.avg
         return None
 
     @property
-    def min(self):
+    def min(self) -> Optional[float]:
         """Minimum value."""
         if self._proto.HasField("min"):
             return self._proto.min
         return None
 
     @property
-    def max(self):
+    def max(self) -> Optional[float]:
         """Maximum value."""
         if self._proto.HasField("max"):
             return self._proto.max
         return None
 
     @property
-    def parameter_count(self):
+    def parameter_count(self) -> int:
         """The number of parameter values this sample represents."""
         return self._proto.n
 
     def __str__(self):
         return f"{self.time} {self.avg}"
 
 
@@ -255,20 +246,20 @@
     number of appearances within a ParameterRange.
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def eng_value(self):
+    def eng_value(self) -> Any:
         """The engineering (calibrated) value."""
         return parse_value(self._proto.engValue)
 
     @property
-    def parameter_count(self):
+    def parameter_count(self) -> int:
         """The number of received parameter values during this range."""
         return self._proto.count
 
     def __str__(self):
         return f"{self.eng_value} {self.parameter_count}x"
 
 
@@ -278,33 +269,29 @@
     value was uninterrupted and unchanged.
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def start(self):
+    def start(self) -> datetime.datetime:
         """
         Start time of this range (inclusive).
-
-        :type: :class:`~datetime.datetime`
         """
         return parse_server_timestring(self._proto.timeStart)
 
     @property
-    def stop(self):
+    def stop(self) -> datetime.datetime:
         """
         Stop time of this range (exclusive).
-
-        :type: :class:`~datetime.datetime`
         """
         return parse_server_timestring(self._proto.timeStop)
 
     @property
-    def eng_value(self):
+    def eng_value(self) -> Optional[Any]:
         """
         The engineering (calibrated) value within this range.
 
         If the request was made using ``min_range`` option,
         this will be the most-frequent value only. Retrieve
         the complete distribution using the ``entries``
         attribute.
@@ -318,27 +305,25 @@
 
         if result:
             return parse_value(result)
         else:
             return None
 
     @property
-    def parameter_count(self):
+    def parameter_count(self) -> int:
         """
         The total number of parameter values within this range.
         """
         return self._proto.count
 
     @property
-    def entries(self):
+    def entries(self) -> List[ParameterRangeEntry]:
         """
         Value distribution within this range.
 
         Unless the request was made using ``min_range`` option,
         there should be only one entry only.
-
-        :type: List[:class:`ParameterRangeEntry`]
         """
         return [ParameterRangeEntry(proto) for proto in self._proto.engValues]
 
     def __str__(self):
         return f"{self.start} - {self.stop}: {self.eng_value}"
```

### Comparing `yamcs-client-1.8.8/src/yamcs/client.py` & `yamcs-client-1.9.0/src/yamcs/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import datetime
 import functools
+from typing import Any, Callable, Iterable, List, Mapping, Optional
 
 from google.protobuf import timestamp_pb2
 from yamcs.archive.client import ArchiveClient
 from yamcs.core.context import Context
 from yamcs.core.futures import WebSocketSubscriptionFuture
 from yamcs.core.helpers import do_get, parse_server_time, to_server_time
 from yamcs.core.subscriptions import WebSocketSubscriptionManager
@@ -77,20 +79,16 @@
 
     A subscription object stores the last time info.
     """
 
     def __init__(self, manager):
         super(TimeSubscription, self).__init__(manager)
 
-        self.time = None
-        """
-        The last time info.
-
-        :type: :class:`~datetime.datetime`
-        """
+        self.time: Optional[datetime.datetime] = None
+        """The last time info."""
 
     def _process(self, time):
         self.time = time
 
 
 class LinkSubscription(WebSocketSubscriptionFuture):
     """
@@ -102,30 +100,28 @@
 
     def __init__(self, manager):
         super(LinkSubscription, self).__init__(manager)
 
         self._cache = {}
         """Link cache keyed by name."""
 
-    def get_link(self, name):
+    def get_link(self, name: str) -> Link:
         """
         Returns the latest link state.
 
-        :param str name: Identifying name of the data link
-        :rtype: .Link
+        :param name:
+            Identifying name of the data link
         """
         if name in self._cache:
             return self._cache[name]
         return None
 
-    def list_links(self):
+    def list_links(self) -> List[Link]:
         """
         Returns a snapshot of all instance links.
-
-        :rtype: .Link[]
         """
         return [self._cache[k] for k in self._cache]
 
     def _process(self, link_event):
         link = link_event.link
         if link_event.event_type == "UNREGISTERED":
             del self._cache[link.name]
@@ -134,348 +130,372 @@
 
 
 class YamcsClient:
     """
     Client for accessing core Yamcs resources.
     """
 
-    def __init__(self, address, **kwargs):
+    def __init__(self, address: str, **kwargs):
         """
-        :param str address: The address of Yamcs in the format 'hostname:port'
-        :param Optional[bool] tls: Whether TLS encryption is expected
-        :param tls_verify: Whether server certificate verification is
-                           enabled (only applicable if ``tls=True``).
-                           As an alternative to a boolean value, this option
-                           may be set to a path containing the appropriate
-                           TLS CA certificate bundle.
-        :type tls_verify: Optional[Union[bool, str]]
-        :param Optional[.Credentials] credentials: Credentials for when the server is
-                                                   secured
-        :param Optional[str] user_agent: Optionally override the default user agent
+        :param address:
+            The address of Yamcs in the format 'hostname:port'
+        :param bool tls:
+            Whether TLS encryption is expected
+        :param tls_verify:
+            Whether server certificate verification is
+            enabled (only applicable if ``tls=True``).
+            As an alternative to a boolean value, this option
+            may be set to a path containing the appropriate
+            TLS CA certificate bundle.
+        :type tls_verify:
+            Optional[Union[bool, str]]
+        :param Optional[.Credentials] credentials:
+            Credentials for when the server is secured
+        :param Optional[str] user_agent:
+            Optionally override the default user agent
         """
         self.ctx = Context(address, **kwargs)
 
-    def get_time(self, instance):
+    def get_time(self, instance) -> datetime.datetime:
         """
         Return the current mission time for the specified instance.
-
-        :rtype: ~datetime.datetime
         """
         url = f"/instances/{instance}"
         response = self.ctx.get_proto(url)
         message = yamcsManagement_pb2.YamcsInstance()
         message.ParseFromString(response.content)
         if message.HasField("missionTime"):
             return parse_server_time(message.missionTime)
         return None
 
-    def get_server_info(self):
+    def get_server_info(self) -> ServerInfo:
         """
         Return general server info.
-
-        :rtype: .ServerInfo
         """
         response = self.ctx.get_proto(path="")
         message = server_service_pb2.GetServerInfoResponse()
         message.ParseFromString(response.content)
         return ServerInfo(message)
 
-    def get_auth_info(self):
+    def get_auth_info(self) -> AuthInfo:
         """
         Returns general authentication information. This operation
         does not require authenticating and is useful to test
         if a server requires authentication or not.
-
-        :rtype: .AuthInfo
         """
         response = do_get(
             self.ctx.session,
             self.ctx.auth_root,  # Full URL, so don't use get_proto
             headers={"Accept": "application/protobuf"},
         )
         message = auth_pb2.AuthInfo()
         message.ParseFromString(response.content)
         return AuthInfo(message)
 
-    def get_user_info(self):
+    def get_user_info(self) -> UserInfo:
         """
         Get information on the authenticated user.
-
-        :rtype: .UserInfo
         """
         response = self.ctx.get_proto(path="/user")
         message = iam_pb2.UserInfo()
         message.ParseFromString(response.content)
         return UserInfo(message)
 
-    def get_mdb(self, instance):
+    def get_mdb(self, instance: str) -> MDBClient:
         """
         Return an object for working with the MDB of the specified instance.
 
-        :param str instance: A Yamcs instance name.
-        :rtype: .MDBClient
+        :param instance:
+            A Yamcs instance name.
         """
         return MDBClient(self.ctx, instance)
 
-    def get_archive(self, instance):
+    def get_archive(self, instance: str) -> ArchiveClient:
         """
         Return an object for working with the Archive of the specified instance.
 
-        :param str instance: A Yamcs instance name.
-        :rtype: .ArchiveClient
+        :param instance:
+            A Yamcs instance name.
         """
         return ArchiveClient(self.ctx, instance)
 
-    def get_file_transfer_client(self, instance):
+    def get_file_transfer_client(self, instance: str) -> FileTransferClient:
         """
         Return an object for working with file transfers on a specified instance.
 
-        :param str instance: A Yamcs instance name.
-        :rtype: .FileTransferClient
+        :param instance:
+            A Yamcs instance name.
         """
         return FileTransferClient(self.ctx, instance)
 
-    def get_tco_client(self, instance, service):
+    def get_tco_client(self, instance: str, service: str) -> TCOClient:
         """
         Return an object for Time Correlation API calls on a specified service.
 
-        :param str instance: A Yamcs instance name.
-        :param str service: Target service name.
-        :rtype: .TCOClient
+        :param instance:
+            A Yamcs instance name.
+        :param service:
+            Target service name.
         """
         return TCOClient(self.ctx, instance, service)
 
-    def get_storage_client(self, instance="_global"):
+    def get_storage_client(self, instance: str = "_global") -> StorageClient:
         """
         Return an object for working with object storage
 
-        :param str instance: The storage instance.
-        :rtype: .StorageClient
+        :param instance:
+            The storage instance.
         """
         return StorageClient(self.ctx, instance)
 
-    def get_timeline_client(self, instance):
+    def get_timeline_client(self, instance: str) -> TimelineClient:
         """
         Return an object for working with Yamcs timeline items
 
-        :param str instance: A Yamcs instance name.
-        :rtype: .TimelineClient
+        :param instance:
+            A Yamcs instance name.
         """
         return TimelineClient(self.ctx, instance)
 
-    def create_instance(self, name, template, args=None, labels=None):
+    def create_instance(
+        self,
+        name: str,
+        template: str,
+        args: Optional[Mapping[str, Any]] = None,
+        labels: Optional[Mapping[str, str]] = None,
+    ):
         """
         Create a new instance based on an existing template. This method blocks
         until the instance is fully started.
 
-        :param str instance: A Yamcs instance name.
-        :param str template: The name of an existing template.
+        :param instance:
+            A Yamcs instance name.
+        :param template:
+            The name of an existing template.
         """
         req = yamcsManagement_pb2.CreateInstanceRequest()
         req.name = name
         req.template = template
         if args:
             for k in args:
                 req.templateArgs[k] = args[k]
         if labels:
             for k in labels:
                 req.labels[k] = labels[k]
         url = "/instances"
         self.ctx.post_proto(url, data=req.SerializeToString())
 
-    def list_instance_templates(self):
+    def list_instance_templates(self) -> Iterable[InstanceTemplate]:
         """
         List the available instance templates.
         """
         response = self.ctx.get_proto(path="/instance-templates")
         message = yamcsManagement_pb2.ListInstanceTemplatesResponse()
         message.ParseFromString(response.content)
         templates = getattr(message, "templates")
         return iter([InstanceTemplate(template) for template in templates])
 
-    def list_services(self, instance):
+    def list_services(self, instance: str) -> Iterable[Service]:
         """
         List the services for an instance.
 
-        :param str instance: A Yamcs instance name.
-        :rtype: ~collections.abc.Iterable[~yamcs.model.Service]
+        :param instance:
+            A Yamcs instance name.
         """
         # Server does not do pagination on listings of this resource.
         # Return an iterator anyway for similarity with other API methods
         url = f"/services/{instance}"
         response = self.ctx.get_proto(path=url)
         message = yamcsManagement_pb2.ListServicesResponse()
         message.ParseFromString(response.content)
         services = getattr(message, "services")
         return iter([Service(service) for service in services])
 
-    def start_service(self, instance, service):
+    def start_service(self, instance: str, service: str):
         """
         Starts a single service.
 
-        :param str instance: A Yamcs instance name.
-        :param str service: The name of the service.
+        :param instance:
+            A Yamcs instance name.
+        :param service:
+            The name of the service.
         """
         url = f"/services/{instance}/{service}:start"
         self.ctx.post_proto(url)
 
-    def stop_service(self, instance, service):
+    def stop_service(self, instance: str, service: str):
         """
         Stops a single service.
 
-        :param str instance: A Yamcs instance name.
-        :param str service: The name of the service.
+        :param instance:
+            A Yamcs instance name.
+        :param service:
+            The name of the service.
         """
         url = f"/services/{instance}/{service}:stop"
         self.ctx.post_proto(url)
 
-    def list_processors(self, instance=None):
+    def list_processors(self, instance: Optional[str] = None) -> Iterable[Processor]:
         """
         Lists the processors.
 
         Processors are returned in lexicographical order.
 
-        :param Optional[str] instance: A Yamcs instance name.
-        :rtype: ~collections.abc.Iterable[.Processor]
+        :param instance:
+            A Yamcs instance name.
         """
         # Server does not do pagination on listings of this resource.
         # Return an iterator anyway for similarity with other API methods
         url = "/processors"
         if instance:
             url += "?instance=" + instance
         response = self.ctx.get_proto(path=url)
         message = processing_pb2.ListProcessorsResponse()
         message.ParseFromString(response.content)
         processors = getattr(message, "processors")
         return iter([Processor(processor) for processor in processors])
 
-    def get_processor(self, instance, processor):
+    def get_processor(self, instance: str, processor: str) -> ProcessorClient:
         """
         Return an object for working with a specific Yamcs processor.
 
-        :param str instance: A Yamcs instance name.
-        :param str processor: A processor name within that instance.
-        :rtype: .ProcessorClient
+        :param instance:
+            A Yamcs instance name.
+        :param processor:
+            A processor name within that instance.
         """
         return ProcessorClient(self.ctx, instance, processor)
 
-    def get_link(self, instance, link):
+    def delete_processor(self, instance: str, processor: str):
+        """
+        Delete a processor.
+
+        :param instance:
+            A Yamcs instance name.
+        :param processor:
+            A processor name within that instance.
+        """
+        url = f"/processors/{instance}/{processor}"
+        self.ctx.delete_proto(url)
+
+    def get_link(self, instance: str, link: str) -> LinkClient:
         """
         Return an object for working with a specific Yamcs link.
 
-        :param str instance: A Yamcs instance name.
-        :param str link: A link name within that instance.
-        :rtype: .LinkClient
+        :param instance:
+            A Yamcs instance name.
+        :param link:
+            A link name within that instance.
         """
         return LinkClient(self.ctx, instance, link)
 
-    def list_instances(self):
+    def list_instances(self) -> Iterable[Instance]:
         """
         Lists the instances.
 
         Instances are returned in lexicographical order.
-
-        :rtype: ~collections.abc.Iterable[.Instance]
         """
         # Server does not do pagination on listings of this resource.
         # Return an iterator anyway for similarity with other API methods
         response = self.ctx.get_proto(path="/instances")
         message = yamcsManagement_pb2.ListInstancesResponse()
         message.ParseFromString(response.content)
         instances = getattr(message, "instances")
         return iter([Instance(instance) for instance in instances])
 
-    def start_instance(self, instance):
+    def start_instance(self, instance: str):
         """
         Starts a single instance.
 
-        :param str instance: A Yamcs instance name.
+        :param instance:
+            A Yamcs instance name.
         """
         url = f"/instances/{instance}:start"
         self.ctx.post_proto(url)
 
-    def stop_instance(self, instance):
+    def stop_instance(self, instance: str):
         """
         Stops a single instance.
 
-        :param str instance: A Yamcs instance name.
+        :param instance:
+            A Yamcs instance name.
         """
         url = f"/instances/{instance}:stop"
         self.ctx.post_proto(url)
 
-    def restart_instance(self, instance):
+    def restart_instance(self, instance: str):
         """
         Restarts a single instance.
 
-        :param str instance: A Yamcs instance name.
+        :param instance:
+            A Yamcs instance name.
         """
         url = f"/instances/{instance}:restart"
         self.ctx.post_proto(url)
 
-    def list_links(self, instance):
+    def list_links(self, instance: str) -> Iterable[Link]:
         """
         Lists the data links visible to this client.
 
         Data links are returned in random order.
 
-        :param str instance: A Yamcs instance name.
-        :rtype: ~collections.abc.Iterable[.Link]
+        :param instance:
+            A Yamcs instance name.
         """
         # Server does not do pagination on listings of this resource.
         # Return an iterator anyway for similarity with other API methods
         response = self.ctx.get_proto(path="/links/" + instance)
         message = links_pb2.ListLinksResponse()
         message.ParseFromString(response.content)
         links = getattr(message, "links")
         return iter([Link(link) for link in links])
 
     def send_event(
         self,
-        instance,
-        message,
-        event_type=None,
-        time=None,
-        severity="info",
-        source=None,
-        sequence_number=None,
-        extra=None,
+        instance: str,
+        message: str,
+        event_type: Optional[str] = None,
+        time: Optional[datetime.datetime] = None,
+        severity: Optional[str] = "info",
+        source: Optional[str] = None,
+        sequence_number: Optional[int] = None,
+        extra: Optional[Mapping[str, str]] = None,
     ):
         """
         Post a new event.
 
-        :param str instance: A Yamcs instance name.
-        :param str message: Event message.
-        :param Optional[str] event_type: Type of event.
-
-        :param severity: The severity level of the event. One of ``info``,
-                         ``watch``, ``warning``, ``distress``, ``critical``
-                         or ``severe``. Defaults to ``info``.
-        :type severity: Optional[str]
-
-        :param time: Time of the event. If unspecified, defaults to mission time.
-        :type time: Optional[~datetime.datetime]
-
-        :param source: Source of the event. Useful for grouping events in the
-                       archive. When unset this defaults to ``User``.
-        :type source: Optional[str]
-
-        :param event_type: Event type.
-        :type event_type: Optional[str]
-
-        :param sequence_number: Sequence number of this event. This is used to
-                                determine unicity of events at the same time and
-                                coming from the same source. If not set Yamcs
-                                will automatically assign a sequential number as
-                                if every submitted event is unique.
-        :type sequence_number: Optional[int]
-
-        :param dict extra: Extra event properties.
+        :param instance:
+            A Yamcs instance name.
+        :param message:
+            Event message.
+        :param event_type:
+            Type of event.
+
+        :param severity:
+            The severity level of the event. One of ``info``,
+            ``watch``, ``warning``, ``distress``, ``critical``
+            or ``severe``. Defaults to ``info``.
+        :param time:
+            Time of the event. If unspecified, defaults to mission time.
+        :param source:
+            Source of the event. Useful for grouping events in the
+            archive. When unset this defaults to ``User``.
+        :param event_type:
+            Event type.
+        :param sequence_number:
+            Sequence number of this event. This is used to
+            determine unicity of events at the same time and
+            coming from the same source. If not set Yamcs
+            will automatically assign a sequential number as
+            if every submitted event is unique.
+        :param extra:
+            Extra event properties.
 
-                           .. versionadded:: 1.8.4
-                              Compatible with Yamcs 5.7.3 onwards
+            .. versionadded:: 1.8.4
+               Compatible with Yamcs 5.7.3 onwards
         """
         req = events_service_pb2.CreateEventRequest()
         req.message = message
         req.severity = severity
         if event_type:
             req.type = event_type
         if time:
@@ -487,34 +507,35 @@
         if extra:
             for key in extra:
                 req.extra[key] = extra[key]
 
         url = f"/archive/{instance}/events"
         self.ctx.post_proto(url, data=req.SerializeToString())
 
-    def create_link_subscription(self, instance, on_data=None, timeout=60):
+    def create_link_subscription(
+        self,
+        instance: str,
+        on_data: Optional[Callable[[LinkEvent], None]] = None,
+        timeout: float = 60,
+    ) -> LinkSubscription:
         """
         Create a new subscription for receiving data link updates of an instance.
 
         This method returns a future, then returns immediately. Stop the
         subscription by canceling the future.
 
-        :param str instance: A Yamcs instance name.
-
-        :param on_data: Function that gets called with
-                        :class:`.LinkEvent` updates.
-        :type on_data: Optional[Callable[.LinkEvent])
-
-        :param timeout: The amount of seconds to wait for the request to
-                        complete.
-        :type timeout: Optional[float]
-
-        :return: Future that can be used to manage the background websocket
-                 subscription.
-        :rtype: .LinkSubscription
+        :param instance:
+            A Yamcs instance name.
+        :param on_data:
+            Function that gets called with :class:`.LinkEvent` updates.
+        :param timeout:
+            The amount of seconds to wait for the request to complete.
+        :return:
+            Future that can be used to manage the background websocket
+            subscription.
         """
         options = links_pb2.SubscribeLinksRequest()
         options.instance = instance
         manager = WebSocketSubscriptionManager(self.ctx, topic="links", options=options)
 
         # Represent subscription as a future
         subscription = LinkSubscription(manager)
@@ -526,35 +547,37 @@
         manager.open(wrapped_callback)
 
         # Wait until a reply or exception is received
         subscription.reply(timeout=timeout)
 
         return subscription
 
-    def create_time_subscription(self, instance, on_data=None, timeout=60):
+    def create_time_subscription(
+        self,
+        instance: str,
+        on_data: Optional[Callable[[datetime.datetime], None]] = None,
+        timeout: float = 60,
+    ) -> TimeSubscription:
         """
         Create a new subscription for receiving time updates of an instance.
         Time updates are emitted at 1Hz.
 
         This method returns a future, then returns immediately. Stop the
         subscription by canceling the future.
 
-        :param str instance: A Yamcs instance name
-
-        :param on_data: Function that gets called with
-                        :class:`~datetime.datetime` updates.
-        :type on_data: Optional[Callable[~datetime.datetime])
-
-        :param timeout: The amount of seconds to wait for the request to
-                        complete.
-        :type timeout: Optional[float]
-
-        :return: Future that can be used to manage the background websocket
-                 subscription.
-        :rtype: .TimeSubscription
+        :param instance:
+            A Yamcs instance name
+        :param on_data:
+            Function that gets called with :class:`~datetime.datetime` updates.
+        :param timeout:
+            The amount of seconds to wait for the request to complete.
+
+        :return:
+            Future that can be used to manage the background websocket
+            subscription.
         """
         options = time_service_pb2.SubscribeTimeRequest()
         options.instance = instance
         manager = WebSocketSubscriptionManager(self.ctx, topic="time", options=options)
 
         # Represent subscription as a future
         subscription = TimeSubscription(manager)
@@ -566,33 +589,32 @@
         manager.open(wrapped_callback)
 
         # Wait until a reply or exception is received
         subscription.reply(timeout=timeout)
 
         return subscription
 
-    def create_event_subscription(self, instance, on_data, timeout=60):
+    def create_event_subscription(
+        self, instance: str, on_data: Callable[[Event], None], timeout: float = 60
+    ) -> WebSocketSubscriptionFuture:
         """
         Create a new subscription for receiving events of an instance.
 
         This method returns a future, then returns immediately. Stop the
         subscription by canceling the future.
 
-        :param str instance: A Yamcs instance name
-
-        :param on_data: Function that gets called on each :class:`.Event`.
-        :type on_data: Optional[Callable[.Event])
-
-        :param timeout: The amount of seconds to wait for the request to
-                        complete.
-        :type timeout: Optional[float]
-
-        :return: Future that can be used to manage the background websocket
-                 subscription.
-        :rtype: .WebSocketSubscriptionFuture
+        :param instance:
+            A Yamcs instance name
+        :param on_data:
+            Function that gets called on each :class:`.Event`.
+        :param timeout:
+            The amount of seconds to wait for the request to complete.
+        :return:
+            Future that can be used to manage the background websocket
+            subscription.
         """
         options = events_service_pb2.SubscribeEventsRequest()
         options.instance = instance
         manager = WebSocketSubscriptionManager(
             self.ctx, topic="events", options=options
         )
```

### Comparing `yamcs-client-1.8.8/src/yamcs/core/auth.py` & `yamcs-client-1.9.0/src/yamcs/core/auth.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import base64
 from datetime import datetime, timedelta, timezone
+from typing import Callable, Optional
 
+import requests
 from requests.auth import HTTPBasicAuth
 from yamcs.core.exceptions import Unauthorized, YamcsError
 from yamcs.core.helpers import do_post
 
 
 def _convert_user_credentials(
-    session, token_url, username=None, password=None, refresh_token=None
-):
+    session: requests.Session,
+    token_url: str,
+    username: Optional[str] = None,
+    password: Optional[str] = None,
+    refresh_token: Optional[str] = None,
+) -> "Credentials":
     """
     Converts username/password credentials to token credentials by
     using Yamcs as the authentication server.
     """
     if username and password:
         data = {"grant_type": "password", "username": username, "password": password}
     elif refresh_token:
@@ -32,16 +38,20 @@
             expiry=expiry,
         )
     else:
         raise YamcsError(f"{response.status_code} Server Error")
 
 
 def _convert_service_account_credentials(
-    session, token_url, client_id, client_secret, become
-):
+    session: requests.Session,
+    token_url: str,
+    client_id: str,
+    client_secret: str,
+    become: str,
+) -> "Credentials":
     """
     Converts service account credentials to impersonated token credentials.
     """
     data = {"grant_type": "client_credentials", "become": become}
 
     response = do_post(
         session,
@@ -71,22 +81,22 @@
 
     * Username/password credentials (fields ``username`` and ``password``)
     * Bearer tokens (fields ``access_token`` and optionally ``refresh_token``)
     """
 
     def __init__(
         self,
-        username=None,
-        password=None,
-        access_token=None,
-        refresh_token=None,
-        expiry=None,
-        client_id=None,
-        client_secret=None,
-        become=None,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        access_token: Optional[str] = None,
+        refresh_token: Optional[str] = None,
+        expiry: Optional[datetime] = None,
+        client_id: Optional[str] = None,
+        client_secret: Optional[str] = None,
+        become: Optional[str] = None,
     ):
         self.username = username
         """Username (only needed when using username/password credentials)."""
 
         self.password = password
         """Clear-text password (consider TLS!)."""
 
@@ -109,15 +119,20 @@
         """
         Name of the user to impersonate. Only service accounts with
         impersonation authority can use this feature.
         """
 
         self._on_token_update = None
 
-    def login(self, session, auth_url, on_token_update):
+    def login(
+        self,
+        session: requests.Session,
+        auth_url: str,
+        on_token_update: Optional[Callable[["Credentials"], None]],
+    ) -> "Credentials":
         self._on_token_update = on_token_update
         token_url = auth_url + "/token"
         if self.username:  # Convert u/p to bearer
             creds = _convert_user_credentials(
                 session, token_url, username=self.username, password=self.password
             )
         elif self.become:  # Impersonate from service account
@@ -131,18 +146,18 @@
         else:
             creds = self
 
         if on_token_update:
             on_token_update(creds)
         return creds
 
-    def is_expired(self):
+    def is_expired(self) -> bool:
         return self.expiry and datetime.now(tz=timezone.utc) >= self.expiry
 
-    def refresh(self, session, auth_url):
+    def refresh(self, session: requests.Session, auth_url: str):
         if self.become:
             new_creds = _convert_service_account_credentials(
                 session,
                 auth_url + "/token",
                 client_id=self.client_id,
                 client_secret=self.client_secret,
                 become=self.become,
@@ -156,36 +171,36 @@
 
         self.access_token = new_creds.access_token
         self.refresh_token = new_creds.refresh_token
         self.expiry = new_creds.expiry
         if self._on_token_update:
             self._on_token_update(self)
 
-    def before_request(self, session, auth_url):
+    def before_request(self, session: requests.Session, auth_url: str):
         if self.is_expired():
             self.refresh(session, auth_url)
 
         if self.access_token:
             session.headers.update({"Authorization": "Bearer " + self.access_token})
 
 
 class BasicAuthCredentials(Credentials):
     """
     Data holder for Basic Auth credentials. This includes a username and a password
     which are passed in the HTTP Authorization header on each request.
     """
 
-    def __init__(self, username, password):
+    def __init__(self, username: str, password: str):
         super().__init__(username=username, password=password)
 
-    def is_expired(self):
+    def is_expired(self) -> bool:
         return False
 
     def refresh(self):
         pass
 
     def login(self, *args, **kwargs):
         return self
 
-    def before_request(self, session, auth_url):
+    def before_request(self, session: requests.Session, auth_url: str):
         usernamePass = base64.b64encode((self.username + ":" + self.password).encode())
         session.headers.update({"Authorization": "Basic " + usernamePass.decode()})
```

### Comparing `yamcs-client-1.8.8/src/yamcs/core/context.py` & `yamcs-client-1.9.0/src/yamcs/core/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+from typing import Callable, Optional, Union
+
 import requests
 import urllib3
 from google.protobuf.message import DecodeError
 from yamcs import clientversion
 from yamcs.api import exception_pb2
+from yamcs.core.auth import Credentials
 from yamcs.core.exceptions import NotFound, Unauthorized, YamcsError
 from yamcs.core.helpers import do_request
 
 
 class Context:
-
     credentials = None
 
     def __init__(
         self,
-        address,
-        tls=False,
-        credentials=None,
-        user_agent=None,
-        on_token_update=None,
-        tls_verify=True,
+        address: str,
+        tls: bool = False,
+        credentials: Optional[Credentials] = None,
+        user_agent: Optional[str] = None,
+        on_token_update: Optional[Callable[[Credentials], None]] = None,
+        tls_verify: Union[bool, str] = True,
     ):
         if address.endswith("/"):
             self.address = address[:-1]
         else:
             self.address = address
 
         if tls:
@@ -53,48 +55,48 @@
                 self.session, self.auth_root, on_token_update
             )
 
         if not user_agent:
             user_agent = "python-yamcs-client v" + clientversion.__version__
         self.session.headers.update({"User-Agent": user_agent})
 
-    def get_proto(self, path, **kwargs):
+    def get_proto(self, path: str, **kwargs) -> requests.Request:
         headers = kwargs.pop("headers", {})
         headers["Accept"] = "application/protobuf"
         kwargs.update({"headers": headers})
         return self.request("get", path, **kwargs)
 
-    def put_proto(self, path, **kwargs):
+    def put_proto(self, path: str, **kwargs) -> requests.Request:
         headers = kwargs.pop("headers", {})
         headers["Content-Type"] = "application/protobuf"
         headers["Accept"] = "application/protobuf"
         kwargs.update({"headers": headers})
         return self.request("put", path, **kwargs)
 
-    def patch_proto(self, path, **kwargs):
+    def patch_proto(self, path: str, **kwargs) -> requests.Request:
         headers = kwargs.pop("headers", {})
         headers["Content-Type"] = "application/protobuf"
         headers["Accept"] = "application/protobuf"
         kwargs.update({"headers": headers})
         return self.request("patch", path, **kwargs)
 
-    def post_proto(self, path, **kwargs):
+    def post_proto(self, path: str, **kwargs) -> requests.Request:
         headers = kwargs.pop("headers", {})
         headers["Content-Type"] = "application/protobuf"
         headers["Accept"] = "application/protobuf"
         kwargs.update({"headers": headers})
         return self.request("post", path, **kwargs)
 
-    def delete_proto(self, path, **kwargs):
+    def delete_proto(self, path: str, **kwargs) -> requests.Request:
         headers = kwargs.pop("headers", {})
         headers["Accept"] = "application/protobuf"
         kwargs.update({"headers": headers})
         return self.request("delete", path, **kwargs)
 
-    def request(self, method, path, **kwargs):
+    def request(self, method: str, path: str, **kwargs) -> requests.Request:
         path = f"{self.api_root}{path}"
 
         if self.credentials:
             self.credentials.before_request(self.session, self.auth_root)
 
         response = do_request(self.session, method, path, **kwargs)
         if 200 <= response.status_code < 300:
```

### Comparing `yamcs-client-1.8.8/src/yamcs/core/futures.py` & `yamcs-client-1.9.0/src/yamcs/core/futures.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import threading
 from concurrent.futures import Future
 
 from yamcs.core.exceptions import TimeoutError, YamcsError
+from yamcs.core.subscriptions import WebSocketSubscriptionManager
 
 
 class WebSocketSubscriptionFuture(Future):
     """
     Future for capturing the asynchronous execution of a WebSocket subscription.
     """
 
-    def __init__(self, manager):
+    def __init__(self, manager: WebSocketSubscriptionManager):
         super(WebSocketSubscriptionFuture, self).__init__()
         self.ctx = manager.ctx
         self._manager = manager
         self._manager.add_response_callback(self._on_response_callback)
         self._manager.add_close_callback(self._on_close_callback)
 
         # Yamcs send either a 'reply' message or an 'exception' message on
```

### Comparing `yamcs-client-1.8.8/src/yamcs/core/helpers.py` & `yamcs-client-1.9.0/src/yamcs/core/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import logging
 import os
 from collections import OrderedDict
 from datetime import datetime, timezone
+from typing import Any, List, Union
 from urllib.parse import urlparse
 
 import requests
 import urllib3
 from google.protobuf import timestamp_pb2
 from google.protobuf.internal.decoder import _DecodeVarint32
 from yamcs.core.exceptions import ConnectionFailure, YamcsError
 from yamcs.protobuf import yamcs_pb2
 
 logger = logging.getLogger("yamcs-client")
 
 
-def to_isostring(dt):
+def to_isostring(dt: datetime) -> str:
     """
     Converts the given datetime to an ISO String for use as URL parameter.
     """
     pb = to_server_time(dt)
     return pb.ToJsonString()
 
 
-def to_server_time(dt):
+def to_server_time(dt: datetime) -> timestamp_pb2.Timestamp:
     """
     Converts the given ``datetime.datetime`` to a
     ``google.protobuf.timestamp_pb2.Timestamp``.
     """
     if dt.tzinfo is None:
         # TODO - this is a temporary error.
         # Old versions of this client interpreted naive times as UTC,
@@ -40,15 +41,15 @@
         )
 
     pb = timestamp_pb2.Timestamp()
     pb.FromDatetime(dt)
     return pb
 
 
-def parse_server_timestring(isostring):
+def parse_server_timestring(isostring: str) -> datetime:
     """
     Converts an ISO string to a timezone-aware ``datetime.datetime``.
     The timezone uses the system-default. This can be overriden to UTC
     by setting the environment variable ``PYTHON_YAMCS_CLIENT_UTC``.
     """
     if not isostring:
         return None
@@ -56,28 +57,28 @@
     utctime = naive.replace(tzinfo=timezone.utc)
 
     if os.environ.get("PYTHON_YAMCS_CLIENT_UTC") not in (None, "0"):
         return utctime
     return utctime.astimezone(tz=None)
 
 
-def parse_server_time(pb):
+def parse_server_time(pb: timestamp_pb2.Timestamp) -> datetime:
     """
     Converts a Protobuf timestamp message to a timezone-aware ``datetime.datetime``.
     The timezone uses the system-default. This can be overriden to UTC by setting
     the environment variable ``PYTHON_YAMCS_CLIENT_UTC``.
     """
     utctime = pb.ToDatetime().replace(tzinfo=timezone.utc)
 
     if os.environ.get("PYTHON_YAMCS_CLIENT_UTC") not in (None, "0"):
         return utctime
     return utctime.astimezone(tz=None)
 
 
-def parse_value(proto):
+def parse_value(proto: yamcs_pb2.Value) -> Any:
     """
     Converts a Protobuf `Value` from the API into a python native value
     """
     if proto.type == yamcs_pb2.Value.FLOAT:
         return proto.floatValue
     elif proto.type == yamcs_pb2.Value.DOUBLE:
         return proto.doubleValue
@@ -110,28 +111,28 @@
     elif proto.type == yamcs_pb2.Value.NONE:
         return None
     else:
         logger.warning("Unrecognized value type for update %s", proto)
         return None
 
 
-def adapt_name_for_rest(name):
+def adapt_name_for_rest(name: str) -> str:
     """
     Modifies a user-provided name for use in API calls.
     Basically we want an alias like 'MDB:OPS Name/SIMULATOR_BatteryVoltage2'
     to be prepended with a slash.
     """
     if name.startswith("/"):
         return name
     elif "/" not in name:
         raise ValueError("Provided name is not a fully-qualified XTCE name.")
     return "/" + name
 
 
-def to_named_object_id(parameter):
+def to_named_object_id(parameter: str) -> yamcs_pb2.NamedObjectId:
     """
     Builds a NamedObjectId. This is a bit more complex than it really
     should be. In Python (for convenience) we allow the user to simply address
     entries by their alias via the NAMESPACE/NAME convention. Yamcs is not
     aware of this convention so we decompose it into distinct namespace and
     name fields.
     """
@@ -147,43 +148,46 @@
                 "in the format NAMESPACE/NAME"
             )
         named_object_id.namespace = parts[0]
         named_object_id.name = parts[1]
     return named_object_id
 
 
-def to_named_object_ids(parameters):
+def to_named_object_ids(parameters: Union[str, List[str]]) -> yamcs_pb2.NamedObjectList:
     """Builds a list of NamedObjectId."""
     if isinstance(parameters, str):
         return [to_named_object_id(parameters)]
     return [to_named_object_id(parameter) for parameter in parameters]
 
 
-def do_get(session, path, **kwargs):
+def do_get(session: requests.Session, path: str, **kwargs) -> requests.Request:
     """
     Performs an HTTP GET request while reraising connection-type exceptions
     to something produced by this library.
     """
     return do_request(session, "get", path, **kwargs)
 
 
-def do_post(session, path, **kwargs):
+def do_post(session: requests.Session, path: str, **kwargs) -> requests.Request:
     """
     Performs an HTTP POST request while reraising connection-type exceptions
     to something produced by this library.
     """
     return do_request(session, "post", path, **kwargs)
 
 
-def do_request(session, method, path, **kwargs):
+def do_request(
+    session: requests.Session, method: str, path: str, **kwargs
+) -> requests.Request:
     """
     Performs an HTTP request while reraising connection-type exceptions
     to something produced by this library.
     """
     try:
+        session.request
         return session.request(method, path, **kwargs)
     except requests.exceptions.SSLError as ssl_error:
         url_parts = urlparse(path)
         base_url = f"{url_parts.scheme}://{url_parts.netloc}"
         msg = f"Connection to {base_url} failed: {ssl_error}"
         raise ConnectionFailure(msg) from None
     except requests.exceptions.ConnectionError as e:
```

### Comparing `yamcs-client-1.8.8/src/yamcs/core/pagination.py` & `yamcs-client-1.9.0/src/yamcs/core/pagination.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,19 @@
+from yamcs.core.context import Context
+
+
 class Iterator:
     def __init__(
-        self, ctx, path, params, response_class, items_key="items", item_mapper=None
+        self,
+        ctx: Context,
+        path: str,
+        params,
+        response_class,
+        items_key="items",
+        item_mapper=None,
     ):
         self.ctx = ctx
         self.path = path
         self.params = params
         self.response_class = response_class
         self.items_key = items_key
         self.item_mapper = item_mapper
```

### Comparing `yamcs-client-1.8.8/src/yamcs/core/subscriptions.py` & `yamcs-client-1.9.0/src/yamcs/core/subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
 import ssl
 import threading
 
 import websocket
 from yamcs.api import websocket_pb2
+from yamcs.core.context import Context
 from yamcs.core.exceptions import ConnectionFailure
 
 logger = logging.getLogger("yamcs-client")
 
 
 class WebSocketSubscriptionManager:
-    def __init__(self, ctx, topic, options=None):
+    def __init__(self, ctx: Context, topic: str, options=None):
         self.ctx = ctx
         self._topic = topic
         self._options = options
 
         self._websocket = None
         self._callback = None
         self._response_callbacks = []
```

### Comparing `yamcs-client-1.8.8/src/yamcs/filetransfer/client.py` & `yamcs-client-1.9.0/src/yamcs/filetransfer/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import functools
 import json
+from typing import Any, Callable, Iterable, List, Mapping, Optional
 
+from yamcs.core.context import Context
 from yamcs.core.futures import WebSocketSubscriptionFuture
 from yamcs.core.subscriptions import WebSocketSubscriptionManager
 from yamcs.filetransfer.model import RemoteFileListing, Service, Transfer
 from yamcs.protobuf.filetransfer import filetransfer_pb2
 
 
 def _wrap_callback_parse_transfer_data(subscription, on_data, message):
@@ -35,56 +37,50 @@
     """
     Local object providing access to transfer updates.
 
     A subscription object stores the last transfer info for
     each transfer.
     """
 
-    def __init__(self, manager, service_client):
+    def __init__(self, manager, service_client: "FileTransferClient"):
         super(TransferSubscription, self).__init__(manager)
         self.service_client = service_client
         self._cache = {}
         """Transfer cache keyed by id."""
 
-    def get_transfer(self, id):
+    def get_transfer(self, id: str) -> Optional[Transfer]:
         """
         Returns the latest transfer state.
 
-        :param str id: Transfer identifier
-        :rtype: .Transfer
+        :param id:
+            Transfer identifier
         """
         if id in self._cache:
             return self._cache[id]
         return None
 
-    def list_transfers(self):
+    def list_transfers(self) -> List[Transfer]:
         """
         Returns a snapshot of all transfer info.
-
-        :rtype: .Transfer[]
         """
         return [self._cache[k] for k in self._cache]
 
-    def list_ongoing(self):
+    def list_ongoing(self) -> List[Transfer]:
         """
         Returns all ongoing transfers.
-
-        :rtype: .Transfer[]
         """
         return [t for t in self.list_transfers() if not t.is_complete()]
 
-    def list_completed(self):
+    def list_completed(self) -> List[Transfer]:
         """
         Returns all completed transfers (successful or not).
-
-        :rtype: .Transfer[]
         """
         return [t for t in self.list_transfers() if t.is_complete()]
 
-    def _process(self, proto):
+    def _process(self, proto) -> Transfer:
         if proto.id in self._cache:
             transfer = self._cache[proto.id]
             transfer._proto = proto
         else:
             transfer = Transfer(proto, service_client=self.service_client)
             self._cache[transfer.id] = transfer
 
@@ -95,95 +91,97 @@
     """
     Local object providing access to filelist updates.
 
     A subscription object stores the last filelist info for
     each remotepath and destination.
     """
 
-    def __init__(self, manager, service_client):
+    def __init__(self, manager, service_client: "FileTransferClient"):
         super(FileListSubscription, self).__init__(manager)
         self.service_client = service_client
         self._cache = {}
         """Filelist cache keyed by (destination, remotePath)"""
 
-    def get_filelist(self, remote_path, destination):
+    def get_filelist(
+        self, remote_path: str, destination: str
+    ) -> Optional[RemoteFileListing]:
         """
         Get the latest cached filelist for the given remote path and destination
-        :param remote_path: path on the remote destination
-        :param destination: remote entity name
-        :rtype .RemoteFileListing
+
+        :param remote_path:
+            path on the remote destination
+        :param destination:
+            remote entity name
         """
         return self._cache.get((remote_path, destination))
 
-    def _process(self, filelist):
-        filelist = RemoteFileListing(filelist)
+    def _process(self, proto) -> RemoteFileListing:
+        filelist = RemoteFileListing(proto)
         self._cache[(filelist.destination, filelist.remote_path)] = filelist
         return filelist
 
 
 class FileTransferClient:
     """
     Client for working with file transfers (e.g. CFDP) managed by Yamcs.
     """
 
-    def __init__(self, ctx, instance):
+    def __init__(self, ctx: Context, instance: str):
         super(FileTransferClient, self).__init__()
         self.ctx = ctx
         self._instance = instance
         self._default_service = None
 
-    def list_services(self):
+    def list_services(self) -> Iterable[Service]:
         """
         List the services.
-
-        :rtype: ~collections.abc.Iterable[~yamcs.filetransfer.model.Service]
         """
         # Server does not do pagination on listings of this resource.
         # Return an iterator anyway for similarity with other API methods
         response = self.ctx.get_proto(path=f"/filetransfer/{self._instance}/services")
         message = filetransfer_pb2.ListFileTransferServicesResponse()
         message.ParseFromString(response.content)
         services = getattr(message, "services")
         result = []
         for proto in services:
             service_client = ServiceClient(self.ctx, proto)
             result.append(Service(proto, service_client))
         return iter(result)
 
-    def get_service(self, name):
+    def get_service(self, name: str) -> Service:
         """
         Get a specific File Transfer service.
 
-        :param str name: The service name.
-        :rtype: ~yamcs.filetransfer.model.Service
+        :param name:
+            The service name.
         """
         # TODO should have an actual server-side operation for this
         for service in self.list_services():
             if service.name == name:
                 return service
 
 
 class ServiceClient:
-    def __init__(self, ctx, proto):
+    def __init__(self, ctx: Context, proto):
         self.ctx = ctx
         self._instance = proto.instance
         self._service = proto.name
 
     def upload(
         self,
-        bucket_name,
-        object_name,
-        remote_path,
-        source_entity,
-        destination_entity,
-        overwrite,
-        parents,
-        reliable,
-        options,
-    ):
+        bucket_name: str,
+        object_name: str,
+        remote_path: str,
+        source_entity: str,
+        destination_entity: str,
+        overwrite: bool,
+        parents: bool,
+        reliable: bool,
+        options: Mapping[str, Any],
+    ) -> Transfer:
         req = filetransfer_pb2.CreateTransferRequest()
         req.direction = filetransfer_pb2.TransferDirection.UPLOAD
         req.bucket = bucket_name
         req.objectName = object_name
         req.remotePath = remote_path
         if source_entity:
             req.source = source_entity
@@ -196,32 +194,38 @@
             "createPath": parents,
             "reliable": reliable,
         }
         req.options.update(old_options)
         if options:
             req.options.update(options)
 
+        # Keep these for a while, for interacting with Yamcs
+        # versions that do not support the new 'options' field.
+        req.uploadOptions.overwrite = req.options["overwrite"]
+        req.uploadOptions.createPath = req.options["createPath"]
+        req.uploadOptions.reliable = req.options["reliable"]
+
         url = f"/filetransfer/{self._instance}/{self._service}/transfers"
         response = self.ctx.post_proto(url, data=req.SerializeToString())
         message = filetransfer_pb2.TransferInfo()
         message.ParseFromString(response.content)
         return Transfer(message, self)
 
     def download(
         self,
-        bucket_name,
-        remote_path,
-        object_name,
-        source_entity,
-        destination_entity,
-        overwrite,
-        parents,
-        reliable,
-        options,
-    ):
+        bucket_name: str,
+        remote_path: str,
+        object_name: str,
+        source_entity: str,
+        destination_entity: str,
+        overwrite: bool,
+        parents: bool,
+        reliable: bool,
+        options: Mapping[str, Any],
+    ) -> Transfer:
         req = filetransfer_pb2.CreateTransferRequest()
         req.direction = filetransfer_pb2.TransferDirection.DOWNLOAD
         req.bucket = bucket_name
         req.remotePath = remote_path
         if object_name:
             req.objectName = object_name
         if source_entity:
@@ -241,53 +245,67 @@
 
         url = f"/filetransfer/{self._instance}/{self._service}/transfers"
         response = self.ctx.post_proto(url, data=req.SerializeToString())
         message = filetransfer_pb2.TransferInfo()
         message.ParseFromString(response.content)
         return Transfer(message, self)
 
-    def fetch_filelist(self, remote_path, source_entity, destination_entity, options):
+    def fetch_filelist(
+        self,
+        remote_path: str,
+        source_entity: str,
+        destination_entity: str,
+        options: Mapping[str, Any],
+    ):
         req = filetransfer_pb2.ListFilesRequest()
         req.remotePath = remote_path
         if source_entity:
             req.source = source_entity
         if destination_entity:
             req.destination = destination_entity
         if options:
             req.options.update(options)
         url = f"/filetransfer/{self._instance}/{self._service}/files:sync"
         self.ctx.post_proto(url, data=req.SerializeToString())
 
-    def get_filelist(self, remote_path, source_entity, destination_entity, options):
+    def get_filelist(
+        self,
+        remote_path: str,
+        source_entity: str,
+        destination_entity: str,
+        options: Mapping[str, Any],
+    ) -> RemoteFileListing:
         params = {"remotePath": remote_path}
         if source_entity:
             params["source"] = source_entity
         if destination_entity:
             params["destination"] = destination_entity
         if options:
             params["options"] = json.dumps(options)
         url = f"/filetransfer/{self._instance}/{self._service}/files"
         response = self.ctx.get_proto(url, params=params)
         message = filetransfer_pb2.ListFilesResponse()
         message.ParseFromString(response.content)
         return RemoteFileListing(message)
 
-    def pause_transfer(self, id):
+    def pause_transfer(self, id: str):
         url = f"/filetransfer/{self._instance}/{self._service}/transfers/{id}:pause"
         self.ctx.post_proto(url)
 
-    def resume_transfer(self, id):
+    def resume_transfer(self, id: str):
         url = f"/filetransfer/{self._instance}/{self._service}/transfers/{id}:resume"
         self.ctx.post_proto(url)
 
-    def cancel_transfer(self, id):
+    def cancel_transfer(self, id: str):
         url = f"/filetransfer/{self._instance}/{self._service}/transfers/{id}:cancel"
         self.ctx.post_proto(url)
 
-    def create_transfer_subscription(self, on_data=None, timeout=60):
+    def create_transfer_subscription(
+        self, on_data: Optional[Callable[[Transfer], None]] = None, timeout: float = 60
+    ) -> TransferSubscription:
         options = filetransfer_pb2.SubscribeTransfersRequest()
         options.instance = self._instance
         options.serviceName = self._service
 
         manager = WebSocketSubscriptionManager(
             self.ctx, topic="file-transfers", options=options
         )
@@ -302,15 +320,19 @@
         manager.open(wrapped_callback)
 
         # Wait until a reply or exception is received
         subscription.reply(timeout=timeout)
 
         return subscription
 
-    def create_filelist_subscription(self, on_data=None, timeout=60):
+    def create_filelist_subscription(
+        self,
+        on_data: Optional[Callable[[RemoteFileListing], None]] = None,
+        timeout: float = 60,
+    ) -> FileListSubscription:
         options = filetransfer_pb2.SubscribeTransfersRequest()
         options.instance = self._instance
         options.serviceName = self._service
 
         manager = WebSocketSubscriptionManager(
             self.ctx, topic="remote-file-list", options=options
         )
```

### Comparing `yamcs-client-1.8.8/src/yamcs/filetransfer/model.py` & `yamcs-client-1.9.0/src/yamcs/filetransfer/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,98 +1,104 @@
+import datetime
 import threading
 from enum import Enum
+from typing import Any, Callable, List, Mapping, Optional
 
 from yamcs.core.helpers import parse_server_time
 from yamcs.protobuf.filetransfer import filetransfer_pb2
 
 
 class Service:
     def __init__(self, proto, service_client):
         self._proto = proto
         self._service_client = service_client
         self._local_entities = [EntityInfo(entity) for entity in proto.localEntities]
         self._remote_entities = [EntityInfo(entity) for entity in proto.remoteEntities]
         self._capabilities = FileTransferCapabilities(proto.capabilities)
-        self._transfer_options = [FileTransferOption(option) for option in
-                                  proto.transferOptions]
+        self._transfer_options = [
+            FileTransferOption(option) for option in proto.transferOptions
+        ]
 
     @property
-    def instance(self):
+    def instance(self) -> str:
         """Instance of the service"""
         return self._proto.instance
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Name of this service."""
         return self._proto.name
 
     @property
-    def local_entities(self):
+    def local_entities(self) -> List["EntityInfo"]:
         """List of local entities"""
         return self._local_entities
 
     @property
-    def remote_entities(self):
+    def remote_entities(self) -> List["EntityInfo"]:
         """List of remote entities"""
         return self._remote_entities
 
     @property
-    def capabilities(self):
+    def capabilities(self) -> "FileTransferCapabilities":
         """Transfer capabilities"""
         return self._capabilities
 
     @property
-    def transfer_options(self):
+    def transfer_options(self) -> List["FileTransferOption"]:
         """List of possible transfer options"""
         return self._transfer_options
 
     def upload(
         self,
-        bucket_name,
-        object_name,
-        remote_path,
-        source_entity=None,
-        destination_entity=None,
-        overwrite=True,
-        parents=True,
-        reliable=False,
-        options=None,
-    ):
+        bucket_name: str,
+        object_name: str,
+        remote_path: str,
+        source_entity: Optional[str] = None,
+        destination_entity: Optional[str] = None,
+        overwrite: bool = True,
+        parents: bool = True,
+        reliable: bool = False,
+        options: Optional[Mapping[str, Any]] = None,
+    ) -> "Transfer":
         """
         Uploads a file located in a bucket to a remote destination path.
 
         .. warning::
-            Prefer the use of 'options' instead of the parameters
-            overwrite, parents and reliable (deprecated parameters)
+            Prefer the use of ``options`` instead of the deprecated params
+            ``overwrite``, ``parents`` and ``reliable``.
 
-        :param str bucket_name: Name of the bucket containing the source object.
-        :param str object_name: Name of the source object.
-        :param str remote_path: Remote destination.
-        :param str source_entity: Use a specific source entity.
-                                  (useful in case of multiples)
-        :param str destination_entity: Use a specific destination entity.
-                                       (useful in case of multiples)
-        :param bool overwrite:
+        :param bucket_name:
+            Name of the bucket containing the source object.
+        :param object_name:
+            Name of the source object.
+        :param remote_path:
+            Remote destination.
+        :param source_entity:
+            Use a specific source entity. (useful in case of multiples)
+        :param destination_entity:
+            Use a specific destination entity. (useful in case of multiples)
+        :param overwrite:
             Replace file if it already exists.
 
             .. deprecated:: 1.8.6
-                Use options instead (option name: overwrite)
-        :param bool parents:
+                Use ``options`` instead (option name: ``overwrite``)
+        :param parents:
             Create the remote path if it does not yet exist.
 
             .. deprecated:: 1.8.6
-                Use options instead (option name: createPath)
-        :param bool reliable:
+                Use ``options`` instead (option name: ``createPath``)
+        :param reliable:
             Enable reliable transfers.
 
             .. deprecated:: 1.8.6
-                Use options instead (option name: reliable)
-        :param options: file transfer options dict (may overwrite "overwrite", "parents"
-                        or "reliable" parameters if set in these options).
-        :rtype: .Transfer
+                Use ``options`` instead (option name: ``reliable``)
+        :param options:
+            file transfer options dict (may overwrite "overwrite", "parents"
+            or "reliable" parameters if set in these options).
         """
         return self._service_client.upload(
             bucket_name=bucket_name,
             object_name=object_name,
             remote_path=remote_path,
             source_entity=source_entity,
             destination_entity=destination_entity,
@@ -100,259 +106,287 @@
             parents=parents,
             reliable=reliable,
             options=options,
         )
 
     def download(
         self,
-        bucket_name,
-        remote_path,
-        object_name=None,
-        source_entity=None,
-        destination_entity=None,
-        overwrite=True,
-        parents=True,
-        reliable=False,
-        options=None,
-    ):
+        bucket_name: str,
+        remote_path: str,
+        object_name: Optional[str] = None,
+        source_entity: Optional[str] = None,
+        destination_entity: Optional[str] = None,
+        overwrite: bool = True,
+        parents: bool = True,
+        reliable: bool = False,
+        options: Optional[Mapping[str, Any]] = None,
+    ) -> "Transfer":
         """
         Downloads a file from the source to a bucket.
 
         .. warning::
-            Prefer the use of 'options' instead of the parameters
-            overwrite, parents and reliable (deprecated parameters)
+            Prefer the use of ``options`` instead of the deprecated
+            params ``overwrite``, ``parents`` and ``reliable``.
 
-        :param str bucket_name: Name of the bucket to receive the file.
-        :param str object_name: Name of the file received in the bucket.
-        :param str remote_path: Name of the file to be downloaded from the source.
-        :param str source_entity: Use a specific source entity.
-                                  (useful in case of multiples)
-        :param str destination_entity: Use a specific destination entity.
-                                       (useful in case of multiples)
-        :param bool overwrite:
+        :param bucket_name:
+            Name of the bucket to receive the file.
+        :param object_name:
+            Name of the file received in the bucket.
+        :param remote_path:
+            Name of the file to be downloaded from the source.
+        :param source_entity:
+            Use a specific source entity. (useful in case of multiples)
+        :param destination_entity:
+            Use a specific destination entity. (useful in case of multiples)
+        :param overwrite:
             Replace file if it already exists.
 
             .. deprecated:: 1.8.6
-                Use options instead (option name: overwrite)
-        :param bool parents:
+                Use ``options`` instead (option name: ``overwrite``)
+        :param parents:
             Create the remote path if it does not yet exist.
 
             .. deprecated:: 1.8.6
-                Use options instead (option name: createPath)
-        :param bool reliable:
+                Use ``options`` instead (option name: ``createPath``)
+        :param reliable:
             Enable reliable transfers.
 
             .. deprecated:: 1.8.6
-                Use options instead (option name: reliable)
-        :param options: file transfer options dict (may overwrite "overwrite", "parents"
-                        or "reliable" parameters if set in these options).
-        :rtype: .Transfer
+                Use ``options`` instead (option name: ``reliable``)
+        :param options:
+            File transfer options dict (may overwrite ``overwrite``, ``parents``
+            or ``reliable`` parameters if set in these options).
         """
         return self._service_client.download(
             bucket_name=bucket_name,
             remote_path=remote_path,
             object_name=object_name,
             source_entity=source_entity,
             destination_entity=destination_entity,
             overwrite=overwrite,
             parents=parents,
             reliable=reliable,
             options=options,
         )
 
-    def fetch_filelist(self, remote_path, source_entity=None,
-                       destination_entity=None, options=None):
+    def fetch_filelist(
+        self,
+        remote_path: str,
+        source_entity: Optional[str] = None,
+        destination_entity: Optional[str] = None,
+        options: Optional[Mapping[str, Any]] = None,
+    ):
         """
         Sends a request to fetch the directory listing from the remote (destination).
 
-        :param remote_path: path on the remote destination to get the file list
-        :param source_entity: source entity requesting the file list
-        :param destination_entity: destination entity from which the file list is needed
-        :param options: option dictionary
-        :return: None
+        :param remote_path:
+            path on the remote destination to get the file list
+        :param source_entity:
+            source entity requesting the file list
+        :param destination_entity:
+            destination entity from which the file list is needed
+        :param options:
+            option dictionary
         """
-        return self._service_client.fetch_filelist(
+        self._service_client.fetch_filelist(
             remote_path=remote_path,
             source_entity=source_entity,
             destination_entity=destination_entity,
             options=options,
         )
 
-    def get_filelist(self, remote_path, source_entity=None, destination_entity=None,
-                     options=None):
+    def get_filelist(
+        self,
+        remote_path: str,
+        source_entity: Optional[str] = None,
+        destination_entity: Optional[str] = None,
+        options: Optional[Mapping[str, Any]] = None,
+    ) -> "RemoteFileListing":
         """
         Returns the latest directory listing for the given destination.
 
-        :param remote_path: path on the remote destination to get the file list
-        :param source_entity: source entity requesting the file list
-        :param destination_entity: destination entity from which the file list is needed
-        :param options: option dictionary
-        :return: .RemoteFileListing
+        :param remote_path:
+            path on the remote destination to get the file list
+        :param source_entity:
+            source entity requesting the file list
+        :param destination_entity:
+            destination entity from which the file list is needed
+        :param options:
+            option dictionary
         """
         return self._service_client.get_filelist(
             remote_path=remote_path,
             source_entity=source_entity,
             destination_entity=destination_entity,
             options=options,
         )
 
-    def pause_transfer(self, id):
+    def pause_transfer(self, id: str):
         """
         Pauses a transfer
         """
         self._service_client.pause_transfer(id)
 
-    def resume_transfer(self, id):
+    def resume_transfer(self, id: str):
         """
         Resume a transfer
         """
         self._service_client.resume_transfer(id)
 
-    def cancel_transfer(self, id):
+    def cancel_transfer(self, id: str):
         """
         Cancel a transfer
         """
         self._service_client.cancel_transfer(id)
 
-    def create_transfer_subscription(self, on_data=None, timeout=60):
+    def create_transfer_subscription(
+        self,
+        on_data: Optional[Callable[["Transfer"], None]] = None,
+        timeout: float = 60,
+    ):
         """
         Create a new transfer subscription.
 
-        :param on_data: (Optional) Function that gets called with
-                        :class:`.TransferInfo` updates.
-        :param timeout: The amount of seconds to wait for the request to
-                        complete.
-        :type timeout: float
-        :return: Future that can be used to manage the background websocket
-                 subscription
-        :rtype: .TransferSubscription
+        :param on_data:
+            Function that gets called with :class:`.Transfer` updates.
+        :param timeout:
+            The amount of seconds to wait for the request to complete.
+        :return:
+            Future that can be used to manage the background websocket
+            subscription
+        :rtype: yamcs.filetransfer.client.TransferSubscription
         """
         return self._service_client.create_transfer_subscription(
             on_data=on_data, timeout=timeout
         )
 
-    def create_filelist_subscription(self, on_data=None, timeout=60):
+    def create_filelist_subscription(
+        self,
+        on_data: Optional[Callable[["RemoteFileListing"], None]] = None,
+        timeout: float = 60,
+    ):
         """
         Create a new filelist subscription.
 
-        :param on_data: (Optional) Function that gets called with
-                        :class:`.TransferInfo` updates.
-        :param timeout: The amount of seconds to wait for the request to
-                        complete.
-        :type timeout: float
-        :return: Future that can be used to manage the background websocket
-                 subscription
-        :rtype: .FileListSubscription
+        :param on_data:
+            Function that gets called with :class:`.Transfer` updates.
+        :param timeout:
+            The amount of seconds to wait for the request to complete.
+        :return:
+            Future that can be used to manage the background websocket
+            subscription
+        :rtype: yamcs.filetransfer.client.FileListSubscription
         """
         return self._service_client.create_filelist_subscription(
             on_data=on_data, timeout=timeout
         )
 
     def __str__(self):
         return self.name
 
 
 class EntityInfo:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Name of the entity"""
         return self._proto.name
 
     @property
-    def id(self):
+    def id(self) -> str:
         """Entity ID"""
         return self._proto.id
 
 
 class FileTransferCapabilities:
     def __init__(self, proto):
         self._proto = proto
 
     def __str__(self):
         return str(self._proto)
 
     @property
-    def upload(self):
+    def upload(self) -> bool:
         return self._proto.upload
 
     @property
-    def download(self):
+    def download(self) -> bool:
         return self._proto.download
 
     @property
-    def reliability(self):
+    def reliability(self) -> bool:
         """Deprecated, use FileTransferOption"""
         return self._proto.reliability
 
     @property
-    def remote_path(self):
+    def remote_path(self) -> bool:
         return self._proto.remotePath
 
     @property
-    def filelist(self):
+    def filelist(self) -> bool:
         return self._proto.fileList
 
     @property
-    def has_transfer_type(self):
+    def has_transfer_type(self) -> bool:
         return self._proto.has_transfer_type
 
 
 class FileTransferOption:
-
     class Type(Enum):
         BOOLEAN = 0
         DOUBLE = 1
         STRING = 2
 
     def __init__(self, proto):
         self._proto = proto
         if proto == filetransfer_pb2.FileTransferOption.Type.BOOLEAN:
             self._type = FileTransferOption.Type.BOOLEAN
         elif proto == filetransfer_pb2.FileTransferOption.Type.DOUBLE:
             self._type = FileTransferOption.Type.DOUBLE
         else:
             self._type = FileTransferOption.Type.STRING
-        self._values = [{"value": item.value, "verbose_name": item.verboseName} for
-                        item in proto.values]
+        self._values = [
+            {"value": item.value, "verbose_name": item.verboseName}
+            for item in proto.values
+        ]
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Name of the option"""
         return self._proto.name
 
     @property
-    def type(self):
+    def type(self) -> str:
         """Type of the option"""
         return self._type
 
     @property
-    def description(self):
+    def description(self) -> str:
         """Description for the option"""
         return self._proto.description
 
     @property
-    def associated_text(self):
+    def associated_text(self) -> str:
         """Text associated with the option"""
         return self._proto.associatedText
 
     @property
-    def default(self):
+    def default(self) -> Any:
         """Default value for the option"""
         return self._proto.default
 
     @property
     def values(self):
         """List of possible values for the option"""
         return self._values
 
     @property
-    def allow_custom_option(self):
+    def allow_custom_option(self) -> bool:
         """Whether using different values from the pre-set ones is allowed"""
         return self._proto.allowCustomOption
 
     def __str__(self):
         return str(self._proto)
 
 
@@ -362,75 +396,77 @@
     """
 
     def __init__(self, proto, service_client):
         self._proto = proto
         self._service_client = service_client
 
     @property
-    def id(self):
+    def id(self) -> str:
         """Yamcs-local transfer identifier."""
         return self._proto.id
 
     @property
-    def bucket(self):
+    def bucket(self) -> str:
         return self._proto.bucket
 
     @property
-    def object_name(self):
+    def object_name(self) -> str:
         return self._proto.objectName
 
     @property
-    def remote_path(self):
+    def remote_path(self) -> str:
         return self._proto.remotePath
 
     @property
-    def time(self):
+    def time(self) -> Optional[datetime.datetime]:
         """Time when the transfer was started."""
         if self._proto.HasField("startTime"):
             return parse_server_time(self._proto.startTime)
         return None
 
     @property
-    def reliable(self):
+    def reliable(self) -> bool:
         """True if this is a Class 2 CFDP transfer."""
         return self._proto.reliable
 
     @property
-    def state(self):
+    def state(self) -> Optional[str]:
         """Current transfer state."""
         if self._proto.HasField("state"):
             return filetransfer_pb2.TransferState.Name(self._proto.state)
         return None
 
     @property
-    def size(self):
+    def size(self) -> int:
         """Total bytes to transfer."""
         return self._proto.totalSize
 
     @property
-    def transferred_size(self):
+    def transferred_size(self) -> int:
         """Total bytes already transferred."""
         return self._proto.sizeTransferred
 
-    def is_complete(self):
+    def is_complete(self) -> bool:
         """
         Returns whether this transfer is complete. A transfer
         can be completed, yet still failed.
         """
         return self.state == "FAILED" or self.state == "COMPLETED"
 
-    def is_success(self):
+    def is_success(self) -> bool:
         """
         Returns true if this transfer was completed successfully.
         """
         return self.state == "COMPLETED"
 
     @property
-    def error(self):
-        """Error message in case the transfer failed."""
+    def error(self) -> Optional[str]:
+        """
+        Error message in case the transfer failed.
+        """
         if self.state == "FAILED" and self._proto.HasField("failureReason"):
             return self._proto.failureReason
         return None
 
     def pause(self):
         """
         Pause this transfer
@@ -445,19 +481,20 @@
 
     def cancel(self):
         """
         Cancel this transfer
         """
         self._service_client.cancel_transfer(self.id)
 
-    def await_complete(self, timeout=None):
+    def await_complete(self, timeout: Optional[float] = None):
         """
         Wait for the transfer to be completed.
 
-        :param float timeout: The amount of seconds to wait.
+        :param timeout:
+            The amount of seconds to wait.
         """
         completed = threading.Event()
 
         def callback(updated_transfer):
             if updated_transfer.id == self.id:
                 self._proto = updated_transfer._proto
                 if self.is_complete():
@@ -476,58 +513,60 @@
             subscription.cancel()
 
 
 class RemoteFileListing:
     """
     Represents a list of files from a remote.
     """
+
     def __init__(self, proto):
         self._proto = proto
         self._files = [RemoteFile(file) for file in proto.files]
 
     @property
-    def files(self):
+    def files(self) -> List["RemoteFile"]:
         """List of files"""
         return self._files
 
     @property
-    def destination(self):
+    def destination(self) -> str:
         """Remote destination of the file list"""
         return self._proto.destination
 
     @property
-    def remote_path(self):
+    def remote_path(self) -> str:
         """Remote directory of the file list"""
         return self._proto.remotePath
 
     @property
-    def list_time(self):
+    def list_time(self) -> datetime.datetime:
         """Time the file list was made"""
         return parse_server_time(self._proto.listTime)
 
 
 class RemoteFile:
     """
     Represents a file on a remote entity.
     """
+
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Name of the file"""
         return self._proto.name
 
     @property
-    def is_directory(self):
+    def is_directory(self) -> bool:
         """Whether the file is a directory"""
         return self._proto.isDirectory
 
     @property
-    def size(self):
+    def size(self) -> int:
         """File size in bytes"""
         return self._proto.size
 
     @property
-    def modified(self):
+    def modified(self) -> datetime.datetime:
         """Latest modification time of the file"""
         return parse_server_time(self._proto.modified)
```

### Comparing `yamcs-client-1.8.8/src/yamcs/link/client.py` & `yamcs-client-1.9.0/src/yamcs/link/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import functools
+from typing import Callable, Mapping, Optional
 
+from yamcs.core.context import Context
 from yamcs.core.futures import WebSocketSubscriptionFuture
 from yamcs.core.subscriptions import WebSocketSubscriptionManager
 from yamcs.link.model import Cop1Config, Cop1Status
 from yamcs.model import Link
 from yamcs.protobuf.cop1 import cop1_pb2
 from yamcs.protobuf.links import links_pb2
 
@@ -26,70 +28,66 @@
     Local object providing access to COP1 status updates.
     """
 
     def __init__(self, manager):
         super(Cop1Subscription, self).__init__(manager)
         self._status = None
 
-    def get_status(self):
+    def get_status(self) -> Cop1Status:
         """
         Returns the latest known COP1 status.
-
-        :rtype: .Cop1Status
         """
         return self._status
 
     @property
-    def cop1_active(self):
+    def cop1_active(self) -> bool:
         if self._status:
             return self._status.cop1_active
         return None
 
     @property
-    def state(self):
+    def state(self) -> str:
         if self._status:
             return self._status.state
         return None
 
     @property
-    def bypass_all(self):
+    def bypass_all(self) -> bool:
         if self._status:
             return self._status.bypass_all
         return None
 
     @property
-    def v_s(self):
+    def v_s(self) -> int:
         if self._status:
             return self._status.v_s
         return None
 
     @property
-    def nn_r(self):
+    def nn_r(self) -> int:
         if self._status:
             return self._status.nn_r
         return None
 
     def _process(self, update):
         self._status = update
 
 
 class LinkClient:
     """Client object that groups operations for a specific link."""
 
-    def __init__(self, ctx, instance, link):
+    def __init__(self, ctx: Context, instance: str, link: str):
         super(LinkClient, self).__init__()
         self.ctx = ctx
         self._instance = instance
         self._link = link
 
-    def get_info(self):
+    def get_info(self) -> Link:
         """
         Get info on this link.
-
-        :rtype: .Link
         """
         response = self.ctx.get_proto(f"/links/{self._instance}/{self._link}")
         message = links_pb2.LinkInfo()
         message.ParseFromString(response.content)
         return Link(message)
 
     def enable_link(self):
@@ -104,49 +102,48 @@
         """
         Disables this link.
         """
         req = links_pb2.DisableLinkRequest()
         url = f"/links/{self._instance}/{self._link}:disable"
         self.ctx.post_proto(url, data=req.SerializeToString())
 
-    def run_action(self, action, message=None):
+    def run_action(self, action: str, message: Optional[Mapping] = None):
         """
         Runs the given action for this link
-        :param str action: action identifier
-        :param dict message: action message
+
+        :param action:
+            action identifier
+        :param message:
+            action message
         """
         req = links_pb2.RunActionRequest()
         if message:
             req.message.update(message)
 
         url = f"/links/{self._instance}/{self._link}/actions/{action}"
         self.ctx.post_proto(url, data=req.message.SerializeToString())
 
-    def get_cop1_config(self):
+    def get_cop1_config(self) -> Cop1Config:
         """
         Gets the COP1 configuration for a data link.
-
-        :rtype: .Cop1Config
         """
         response = self.ctx.get_proto(f"/cop1/{self._instance}/{self._link}/config")
         message = cop1_pb2.Cop1Config()
         message.ParseFromString(response.content)
         return Cop1Config(message)
 
     def update_cop1_config(
         self,
-        window_width=None,
-        timeout_type=None,
-        tx_limit=None,
-        t1=None,
-    ):
+        window_width: Optional[int] = None,
+        timeout_type: Optional[str] = None,
+        tx_limit: Optional[int] = None,
+        t1: Optional[float] = None,
+    ) -> Cop1Config:
         """
         Sets the COP1 configuration for a data link.
-
-        :rtype: .Cop1Config
         """
         req = cop1_pb2.Cop1Config()
         if window_width is not None:
             req.windowWidth = window_width
         if timeout_type is not None:
             req.timeoutType = cop1_pb2.TimeoutType.Value(timeout_type)
         if tx_limit is not None:
@@ -157,35 +154,43 @@
         url = f"/cop1/{self._instance}/{self._link}/config"
         response = self.ctx.patch_proto(url, data=req.SerializeToString())
 
         message = cop1_pb2.Cop1Config()
         message.ParseFromString(response.content)
         return Cop1Config(message)
 
-    def disable_cop1(self, bypass_all=True):
+    def disable_cop1(self, bypass_all: bool = True):
         """
         Disable COP1 for a data link.
 
-        :param bool bypass_all: All frames have bypass activated
-                                (i.e. they will be BD frames)
+        :param bypass_all:
+            All frames have bypass activated (i.e. they will be BD frames)
         """
         req = cop1_pb2.DisableRequest()
         req.setBypassAll = bypass_all
         url = f"/cop1/{self._instance}/{self._link}:disable"
         self.ctx.post_proto(url, data=req.SerializeToString())
 
-    def initialize_cop1(self, type, clcw_wait_timeout=None, v_r=None):
+    def initialize_cop1(
+        self,
+        type: str,
+        clcw_wait_timeout: Optional[int] = None,
+        v_r: Optional[int] = None,
+    ):
         """
         Initialize COP1.
 
-        :param str type: One of ``WITH_CLCW_CHECK``, ``WITHOUT_CLCW_CHECK``,
-                         ``UNLOCK`` or ``SET_VR``
-        :param int clcw_wait_timeout: timeout in seconds used for the reception of
-                                      CLCW. Required if type is ``WITH_CLCW_CHECK``
-        :param int v_r: value of v(R) if type is set to ``SET_VR``
+        :param type:
+            One of ``WITH_CLCW_CHECK``, ``WITHOUT_CLCW_CHECK``,
+            ``UNLOCK`` or ``SET_VR``
+        :param clcw_wait_timeout:
+            timeout in seconds used for the reception of
+            CLCW. Required if type is ``WITH_CLCW_CHECK``
+        :param v_r:
+            value of v(R) if type is set to ``SET_VR``
         """
         req = cop1_pb2.InitializeRequest()
         req.type = cop1_pb2.InitializationType.Value(type)
 
         if clcw_wait_timeout is not None:
             req.clcwCheckInitializeTimeout = int(1000 * clcw_wait_timeout)
         if v_r is not None:
@@ -198,40 +203,39 @@
         """
         Resume COP1.
         """
         req = cop1_pb2.ResumeRequest()
         url = f"/cop1/{self._instance}/{self._link}:resume"
         self.ctx.post_proto(url, data=req.SerializeToString())
 
-    def get_cop1_status(self):
+    def get_cop1_status(self) -> Cop1Status:
         """
         Retrieve the COP1 status.
-
-        :rtype: .Cop1Status
         """
         response = self.ctx.get_proto(f"/cop1/{self._instance}/{self._link}/status")
         message = cop1_pb2.Cop1Status()
         message.ParseFromString(response.content)
         return Cop1Status(message)
 
-    def create_cop1_subscription(self, on_data, timeout=60):
+    def create_cop1_subscription(
+        self, on_data: Callable[[Cop1Status], None], timeout: float = 60
+    ) -> Cop1Subscription:
         """
         Create a new subscription for receiving status of the COP1 link.
 
         This method returns a future, then returns immediately. Stop the
         subscription by canceling the future.
 
-        :param on_data: Function that gets called on each :class:`.Cop1Status`.
-        :type on_data: Optional[Callable[.Cop1Status])
-        :param timeout: The amount of seconds to wait for the request to
-                        complete.
-        :type timeout: Optional[float]
-        :return: Future that can be used to manage the background websocket
-                 subscription.
-        :rtype: .Cop1Subscription
+        :param on_data:
+            Function that gets called on each :class:`.Cop1Status`.
+        :param timeout:
+            The amount of seconds to wait for the request to complete.
+        :return:
+            Future that can be used to manage the background websocket
+            subscription.
         """
         options = cop1_pb2.SubscribeStatusRequest()
         options.instance = self._instance
         options.link = self._link
 
         manager = WebSocketSubscriptionManager(self.ctx, topic="cop1", options=options)
```

### Comparing `yamcs-client-1.8.8/src/yamcs/link/model.py` & `yamcs-client-1.9.0/src/yamcs/link/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,37 +6,37 @@
     COP1 status
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def cop1_active(self):
+    def cop1_active(self) -> bool:
         return self._proto.cop1Active
 
     @property
-    def state(self):
+    def state(self) -> str:
         if self._proto.HasField("state"):
             return cop1_pb2.Cop1State.Name(self._proto.state)
         return None
 
     @property
-    def bypass_all(self):
+    def bypass_all(self) -> bool:
         if self._proto.HasField("setBypassAll"):
             return self._proto.setBypassAll
         return None
 
     @property
-    def v_s(self):
+    def v_s(self) -> int:
         if self._proto.HasField("vS"):
             return self._proto.vS
         return None
 
     @property
-    def nn_r(self):
+    def nn_r(self) -> int:
         if self._proto.HasField("nnR"):
             return self._proto.nnR
         return None
 
     def __str__(self):
         line = f"COP1_ACTIVE: {self.cop1_active}"
         if self.cop1_active:
@@ -50,33 +50,33 @@
     COP1 configuration
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def vc_id(self):
+    def vc_id(self) -> int:
         """
         Virtual Channel ID.
         """
         return self._proto.vcId
 
     @property
-    def window_width(self):
+    def window_width(self) -> int:
         return self._proto.windowWidth
 
     @property
-    def timeout_type(self):
+    def timeout_type(self) -> str:
         return cop1_pb2.TimeoutType.Name(self._proto.timeoutType)
 
     @property
-    def tx_limit(self):
+    def tx_limit(self) -> int:
         return self._proto.txLimit
 
     @property
-    def t1(self):
+    def t1(self) -> float:
         return self._proto.t1 / 1000.0
 
     def __str__(self):
         res = f"VC_ID: {self.vc_id}, win: {self.window_width}"
         res += f", timeout_type: {self.timeout_type}"
         return res + f", tx_limit: {self.tx_limit}, t1: {self.t1}"
```

### Comparing `yamcs-client-1.8.8/src/yamcs/mdb/client.py` & `yamcs-client-1.9.0/src/yamcs/mdb/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+import urllib.parse
+from typing import Iterable, Optional
+
 from yamcs.core import pagination
+from yamcs.core.context import Context
 from yamcs.core.helpers import adapt_name_for_rest
 from yamcs.mdb.model import Algorithm, Command, Container, Parameter, SpaceSystem
 from yamcs.protobuf.mdb import mdb_pb2
 
 
 class MDBClient:
-    def __init__(self, ctx, instance):
+    def __init__(self, ctx: Context, instance: str):
         super(MDBClient, self).__init__()
         self.ctx = ctx
         self._instance = instance
 
-    def list_space_systems(self, page_size=None):
+    def list_space_systems(
+        self, page_size: Optional[int] = None
+    ) -> Iterable[SpaceSystem]:
         """
         Lists the space systems visible to this client.
 
         Space systems are returned in lexicographical order.
-
-        :rtype: :class:`.SpaceSystem` iterator
         """
         params = {}
 
         if page_size is not None:
             params["limit"] = page_size
 
         return pagination.Iterator(
@@ -28,34 +32,53 @@
             path=f"/mdb/{self._instance}/space-systems",
             params=params,
             response_class=mdb_pb2.ListSpaceSystemsResponse,
             items_key="spaceSystems",
             item_mapper=SpaceSystem,
         )
 
-    def get_space_system(self, name):
+    def get_space_system(self, name: str) -> SpaceSystem:
         """
         Gets a single space system by its unique name.
 
-        :param str name: A fully-qualified XTCE name
-        :rtype: .SpaceSystem
+        :param name:
+            A fully-qualified XTCE name. Use ``/`` for root.
         """
-        url = f"/mdb/{self._instance}/space-systems{name}"
+        encoded_name = urllib.parse.quote_plus(name)
+        url = f"/mdb/{self._instance}/space-systems/{encoded_name}"
         response = self.ctx.get_proto(url)
         message = mdb_pb2.SpaceSystemInfo()
         message.ParseFromString(response.content)
         return SpaceSystem(message)
 
-    def list_parameters(self, parameter_type=None, page_size=None):
-        """Lists the parameters visible to this client.
+    def export_space_system(self, name: str) -> str:
+        """
+        Exports an XTCE description of a space system (XML format).
+
+        .. versionadded:: 1.9.0
+           Compatible with Yamcs 5.8.0 onwards
+
+        :param name:
+            A fully-qualified XTCE name. Use ``/`` for root.
+        """
+        encoded_name = urllib.parse.quote_plus(name)
+        url = f"/mdb/{self._instance}/space-systems/{encoded_name}:exportXTCE"
+        response = self.ctx.get_proto(url)
+        return response.text
+
+    def list_parameters(
+        self, parameter_type: Optional[str] = None, page_size: Optional[int] = None
+    ) -> Iterable[Parameter]:
+        """
+        Lists the parameters visible to this client.
 
         Parameters are returned in lexicographical order.
 
-        :param str parameter_type: The type of parameter
-        :rtype: :class:`.Parameter` iterator
+        :param parameter_type:
+            The type of parameter
         """
         params = {"details": True}
 
         if parameter_type is not None:
             params["type"] = parameter_type
         if page_size is not None:
             params["limit"] = page_size
@@ -65,36 +88,34 @@
             path=f"/mdb/{self._instance}/parameters",
             params=params,
             response_class=mdb_pb2.ListParametersResponse,
             items_key="parameters",
             item_mapper=Parameter,
         )
 
-    def get_parameter(self, name):
+    def get_parameter(self, name: str) -> Parameter:
         """
         Gets a single parameter by its name.
 
-        :param str name: Either a fully-qualified XTCE name or an alias in the
-                         format ``NAMESPACE/NAME``.
-        :rtype: .Parameter
+        :param name:
+            Either a fully-qualified XTCE name or an alias in the
+            format ``NAMESPACE/NAME``.
         """
         name = adapt_name_for_rest(name)
         url = f"/mdb/{self._instance}/parameters{name}"
         response = self.ctx.get_proto(url)
         message = mdb_pb2.ParameterInfo()
         message.ParseFromString(response.content)
         return Parameter(message)
 
-    def list_containers(self, page_size=None):
+    def list_containers(self, page_size: Optional[int] = None) -> Iterable[Container]:
         """
         Lists the containers visible to this client.
 
         Containers are returned in lexicographical order.
-
-        :rtype: :class:`.Container` iterator
         """
         params = {}
 
         if page_size is not None:
             params["limit"] = page_size
 
         return pagination.Iterator(
@@ -102,36 +123,34 @@
             path=f"/mdb/{self._instance}/containers",
             params=params,
             response_class=mdb_pb2.ListContainersResponse,
             items_key="containers",
             item_mapper=Container,
         )
 
-    def get_container(self, name):
+    def get_container(self, name: str) -> Container:
         """
         Gets a single container by its unique name.
 
-        :param str name: Either a fully-qualified XTCE name or an alias in the
-                         format ``NAMESPACE/NAME``.
-        :rtype: .Container
+        :param name:
+            Either a fully-qualified XTCE name or an alias in the
+            format ``NAMESPACE/NAME``.
         """
         name = adapt_name_for_rest(name)
         url = f"/mdb/{self._instance}/containers{name}"
         response = self.ctx.get_proto(url)
         message = mdb_pb2.ContainerInfo()
         message.ParseFromString(response.content)
         return Container(message)
 
-    def list_commands(self, page_size=None):
+    def list_commands(self, page_size: Optional[int] = None) -> Iterable[Command]:
         """
         Lists the commands visible to this client.
 
         Commands are returned in lexicographical order.
-
-        :rtype: :class:`.Command` iterator
         """
         params = {}
 
         if page_size is not None:
             params["limit"] = page_size
 
         return pagination.Iterator(
@@ -139,36 +158,34 @@
             path=f"/mdb/{self._instance}/commands",
             params=params,
             response_class=mdb_pb2.ListCommandsResponse,
             items_key="commands",
             item_mapper=Command,
         )
 
-    def get_command(self, name):
+    def get_command(self, name: str) -> Command:
         """
         Gets a single command by its unique name.
 
-        :param str name: Either a fully-qualified XTCE name or an alias in the
-                         format ``NAMESPACE/NAME``.
-        :rtype: .Command
+        :param name:
+            Either a fully-qualified XTCE name or an alias in the
+            format ``NAMESPACE/NAME``.
         """
         name = adapt_name_for_rest(name)
         url = f"/mdb/{self._instance}/commands{name}"
         response = self.ctx.get_proto(url)
         message = mdb_pb2.CommandInfo()
         message.ParseFromString(response.content)
         return Command(message)
 
-    def list_algorithms(self, page_size=None):
+    def list_algorithms(self, page_size: Optional[int] = None) -> Iterable[Algorithm]:
         """
         Lists the algorithms visible to this client.
 
         Algorithms are returned in lexicographical order.
-
-        :rtype: :class:`.Algorithm` iterator
         """
         params = {}
 
         if page_size is not None:
             params["limit"] = page_size
 
         return pagination.Iterator(
@@ -176,21 +193,21 @@
             path=f"/mdb/{self._instance}/algorithms",
             params=params,
             response_class=mdb_pb2.ListAlgorithmsResponse,
             items_key="algorithms",
             item_mapper=Algorithm,
         )
 
-    def get_algorithm(self, name):
+    def get_algorithm(self, name: str) -> Algorithm:
         """
         Gets a single algorithm by its unique name.
 
-        :param str name: Either a fully-qualified XTCE name or an alias in the
-                         format ``NAMESPACE/NAME``.
-        :rtype: .Algorithm
+        :param name:
+            Either a fully-qualified XTCE name or an alias in the
+            format ``NAMESPACE/NAME``.
         """
         name = adapt_name_for_rest(name)
         url = f"/mdb/{self._instance}/algorithms{name}"
         response = self.ctx.get_proto(url)
         message = mdb_pb2.AlgorithmInfo()
         message.ParseFromString(response.content)
         return Algorithm(message)
```

### Comparing `yamcs-client-1.8.8/src/yamcs/mdb/model.py` & `yamcs-client-1.9.0/src/yamcs/mdb/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,204 +1,208 @@
+from typing import List, Optional, Tuple
+
 from yamcs.protobuf.mdb import mdb_pb2
 
 
 class Algorithm:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Short name"""
         return self._proto.name
 
     @property
-    def qualified_name(self):
+    def qualified_name(self) -> str:
         """Full name (incl. space system)"""
         return self._proto.qualifiedName
 
     @property
-    def aliases(self):
+    def aliases(self) -> List[Tuple[str, str]]:
         """List of (namespace, name) pairs, as 2-tuples"""
-        return {alias.namespace: alias.name for alias in self._proto.alias}.items()
+        return list(
+            {alias.namespace: alias.name for alias in self._proto.alias}.items()
+        )
 
     @property
-    def description(self):
+    def description(self) -> Optional[str]:
         """Short description."""
         if self._proto.HasField("shortDescription"):
             return self._proto.shortDescription
         return None
 
     @property
-    def long_description(self):
+    def long_description(self) -> Optional[str]:
         """Long description."""
         if self._proto.HasField("longDescription"):
             return self._proto.longDescription
         return None
 
     def __str__(self):
         return self.qualified_name
 
 
 class Command:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Short name"""
         return self._proto.name
 
     @property
-    def qualified_name(self):
+    def qualified_name(self) -> str:
         """Full name (incl. space system)"""
         return self._proto.qualifiedName
 
     @property
-    def aliases(self):
+    def aliases(self) -> List[Tuple[str, str]]:
         """List of (namespace, name) pairs, as 2-tuples"""
-        return {alias.namespace: alias.name for alias in self._proto.alias}.items()
+        return list(
+            {alias.namespace: alias.name for alias in self._proto.alias}.items()
+        )
 
     @property
-    def description(self):
+    def description(self) -> Optional[str]:
         """Short description."""
         if self._proto.HasField("shortDescription"):
             return self._proto.shortDescription
         return None
 
     @property
-    def long_description(self):
+    def long_description(self) -> Optional[str]:
         """Long description."""
         if self._proto.HasField("longDescription"):
             return self._proto.longDescription
         return None
 
     @property
-    def base_command(self):
+    def base_command(self) -> Optional["Command"]:
         if self._proto.HasField("baseCommand"):
             return Command(self._proto.baseCommand)
         return None
 
     @property
-    def abstract(self):
+    def abstract(self) -> bool:
         """
         Whether this is an abstract command. Abstract commands are
         intended for inheritance and cannot be issued directly.
         """
         return self._proto.abstract
 
     @property
-    def significance(self):
+    def significance(self) -> Optional["Significance"]:
         if self._proto.HasField("significance"):
             return Significance(self._proto.significance)
         return None
 
     def __str__(self):
         return self.qualified_name
 
 
 class Significance:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def consequence_level(self):
+    def consequence_level(self) -> str:
         """
         One of ``NONE``, ``WATCH``, ``WARNING``, ``DISTRESS``, ``CRITICAL``
         or ``SEVERE``.
         """
         if self._proto.HasField("consequenceLevel"):
             return mdb_pb2.SignificanceInfo.SignificanceLevelType.Name(
                 self._proto.consequenceLevel
             )
         return None
 
     @property
-    def reason(self):
+    def reason(self) -> Optional[str]:
         """Message attached to this significance."""
         if self._proto.HasField("reasonForWarning"):
             return self._proto.reasonForWarning
         return None
 
     def __str__(self):
         return f"[{self.consequence_level}] {self.reason}"
 
 
 class Container:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Short name"""
         return self._proto.name
 
     @property
-    def qualified_name(self):
+    def qualified_name(self) -> str:
         """Full name (incl. space system)"""
         return self._proto.qualifiedName
 
     @property
-    def aliases(self):
+    def aliases(self) -> List[Tuple[str, str]]:
         """List of (namespace, name) pairs, as 2-tuples"""
-        return {alias.namespace: alias.name for alias in self._proto.alias}.items()
+        return list(
+            {alias.namespace: alias.name for alias in self._proto.alias}.items()
+        )
 
     @property
-    def description(self):
+    def description(self) -> Optional[str]:
         """Short description."""
         if self._proto.HasField("shortDescription"):
             return self._proto.shortDescription
         return None
 
     @property
-    def long_description(self):
+    def long_description(self) -> Optional[str]:
         """Long description."""
         if self._proto.HasField("longDescription"):
             return self._proto.longDescription
         return None
 
     def __str__(self):
         return self.qualified_name
 
 
 class ArrayType:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Short name of this type."""
         return self._proto.type.engType
 
     @property
-    def array_type(self):
+    def array_type(self) -> Optional["ArrayType"]:
         """
         In case the elements of an array of this type are also of type `array`, this
         returns type info of the elements' array type.
 
         .. note::
             This is an uncommon use case. Multi-dimensional arrays are more prevalent.
-
-        :type: :class:`.ArrayType`
         """
         if self._proto.type.HasField("arrayInfo"):
             return ArrayType(self._proto.type.arrayInfo)
         return None
 
     @property
-    def members(self):
+    def members(self) -> List["Member"]:
         """
         In case the elements of this array are of type `aggregate`, this returns
         an ordered list of its direct sub-members.
-
-        :type: List[:class:`.Member`]
         """
         return [Member(member) for member in self._proto.type.member]
 
     @property
-    def dimensions(self):
+    def dimensions(self) -> int:
         """The number of dimensions in case of a multi-dimensional array."""
         if self._proto.HasField("dimensions"):
             return self._proto.dimensions
 
     def __str__(self):
         return self.name
 
@@ -212,105 +216,97 @@
     a parameter of type `aggregate`.
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Short name"""
         return self._proto.name
 
     @property
-    def type(self):
-        """
-        Engineering type.
-
-        :type: str
-        """
+    def type(self) -> str:
+        """Engineering type."""
         if self._proto.HasField("type"):
             return self._proto.type.engType
         return None
 
     @property
-    def array_type(self):
+    def array_type(self) -> Optional[ArrayType]:
         """
         In case this member is of type `array`, this returns array-specific
         type info.
-
-        :type: :class:`.ArrayType`
         """
         if self._proto.type.HasField("arrayInfo"):
             return ArrayType(self._proto.type.arrayInfo)
         return None
 
     @property
-    def members(self):
+    def members(self) -> List["Member"]:
         """
         In case this member is of type `aggregate`, this returns an ordered list
         of its direct sub-members.
-
-        :type: List[:class:`.Member`]
         """
         return [Member(member) for member in self._proto.type.member]
 
     def __str__(self):
         return self.name
 
 
 class EnumValue:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def value(self):
+    def value(self) -> int:
         """Numeric value"""
         return self._proto.value
 
     @property
-    def label(self):
+    def label(self) -> str:
         """String value"""
         return self._proto.label
 
     @property
-    def description(self):
+    def description(self) -> Optional[str]:
         """State description"""
         if self._proto.HasField("description"):
             return self.__proto.description
         return None
 
     def __str__(self):
         return self.label
 
 
 class DataEncoding:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def type(self):
+    def type(self) -> str:
         """Raw type"""
         if self._proto.HasField("type"):
             return mdb_pb2.DataEncodingInfo.Type.Name(self._proto.type)
         return None
 
     @property
-    def little_endian(self):
+    def little_endian(self) -> bool:
         """True if little-endian"""
         return self._proto.littleEndian
 
     @property
-    def bitlength(self):
+    def bitlength(self) -> int:
         """The size in bits"""
         if self._proto.HasField("sizeInBits"):
             return self._proto.sizeInBits
         return None
 
     @property
-    def encoding(self):
+    def encoding(self) -> Optional[str]:
         """Encoding detail"""
         if self._proto.HasField("encoding"):
             return self._proto.encoding
         return None
 
     def __str__(self):
         return self.type
@@ -324,111 +320,99 @@
         a value. It is not the value itself.
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Short name"""
         return self._proto.name
 
     @property
-    def qualified_name(self):
+    def qualified_name(self) -> str:
         """Full name (incl. space system)"""
         return self._proto.qualifiedName
 
     @property
-    def aliases(self):
+    def aliases(self) -> List[Tuple[str, str]]:
         """List of (namespace, name) pairs, as 2-tuples"""
-        return {alias.namespace: alias.name for alias in self._proto.alias}.items()
+        return list(
+            {alias.namespace: alias.name for alias in self._proto.alias}.items()
+        )
 
     @property
-    def description(self):
+    def description(self) -> Optional[str]:
         """Short description."""
         if self._proto.HasField("shortDescription"):
             return self._proto.shortDescription
         return None
 
     @property
-    def long_description(self):
+    def long_description(self) -> Optional[str]:
         """Long description."""
         if self._proto.HasField("longDescription"):
             return self._proto.longDescription
         return None
 
     @property
-    def data_source(self):
+    def data_source(self) -> str:
         """
         Specifies how this parameter originated (example: ``TELEMETERED``)
-
-        :type: str
         """
         if self._proto.HasField("dataSource"):
             return mdb_pb2.DataSourceType.Name(self._proto.dataSource)
         return None
 
     @property
-    def type(self):
+    def type(self) -> str:
         """
         Engineering type.
-
-        :type: str
         """
         if self._proto.type.HasField("engType"):
             return self._proto.type.engType
         return None
 
     @property
-    def array_type(self):
+    def array_type(self) -> Optional[ArrayType]:
         """
         In case this parameter is of type `array`, this returns array-specific
         type info.
-
-        :type: :class:`.ArrayType`
         """
         if self._proto.type.HasField("arrayInfo"):
             return ArrayType(self._proto.type.arrayInfo)
         return None
 
     @property
-    def members(self):
+    def members(self) -> List[Member]:
         """
         In case this parameter is of type `aggregate`, this returns an ordered list
         of its direct members.
-
-        :type: List[:class:`.Member`]
         """
         return [Member(member) for member in self._proto.type.member]
 
     @property
-    def units(self):
+    def units(self) -> List[str]:
         """
         Engineering unit(s)
-
-        :type: List[str]
         """
         return [info.unit for info in self._proto.type.unitSet]
 
     @property
-    def enum_values(self):
+    def enum_values(self) -> List[EnumValue]:
         """
         In case this parameter is of type `enumeration`, this returns an ordered list
         of possible values.
-
-        :type: List[:class:`.EnumValue`]
         """
         return [EnumValue(enumValue) for enumValue in self._proto.type.enumValue]
 
     @property
-    def data_encoding(self):
+    def data_encoding(self) -> Optional[DataEncoding]:
         """
         Information on the raw encoding of this parameter, if applicable.
-
-        :type: :class:`.DataEncoding`
         """
         if self._proto.type.HasField("dataEncoding"):
             return DataEncoding(self._proto.type.dataEncoding)
         return None
 
     def __str__(self):
         return self.qualified_name
@@ -445,37 +429,39 @@
         the data streams going into and out of a device.
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Short name"""
         return self._proto.name
 
     @property
-    def qualified_name(self):
+    def qualified_name(self) -> str:
         """Full name (incl. space system)"""
         return self._proto.qualifiedName
 
     @property
-    def aliases(self):
+    def aliases(self) -> List[Tuple[str, str]]:
         """List of (namespace, name) pairs, as 2-tuples"""
-        return {alias.namespace: alias.name for alias in self._proto.alias}.items()
+        return list(
+            {alias.namespace: alias.name for alias in self._proto.alias}.items()
+        )
 
     @property
-    def description(self):
+    def description(self) -> Optional[str]:
         """Short description."""
         if self._proto.HasField("shortDescription"):
             return self._proto.shortDescription
         return None
 
     @property
-    def long_description(self):
+    def long_description(self) -> Optional[str]:
         """Long description."""
         if self._proto.HasField("longDescription"):
             return self._proto.longDescription
         return None
 
     def __str__(self):
         return self.qualified_name
```

### Comparing `yamcs-client-1.8.8/src/yamcs/model.py` & `yamcs-client-1.9.0/src/yamcs/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import datetime
+from typing import Any, Dict, List, Optional
+
 from yamcs.core.helpers import parse_server_time
 from yamcs.protobuf.events import events_pb2
 from yamcs.protobuf.links import links_pb2
 from yamcs.protobuf.yamcsManagement import yamcsManagement_pb2
 
 
 class AuthInfo:
@@ -9,38 +12,38 @@
     Authentication information
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def require_authentication(self):
+    def require_authentication(self) -> bool:
         return self._proto.requireAuthentication
 
 
 class ServerInfo:
     """
     General server properties.
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def id(self):
+    def id(self) -> str:
         """The Server ID."""
         return self._proto.serverId
 
     @property
-    def version(self):
+    def version(self) -> str:
         """The version of Yamcs Server."""
         return self._proto.yamcsVersion
 
     @property
-    def default_yamcs_instance(self):
+    def default_yamcs_instance(self) -> Optional[str]:
         """Returns the default Yamcs instance."""
         if self._proto.HasField("defaultYamcsInstance"):
             return self._proto.defaultYamcsInstance
         return None
 
     def __str__(self):
         return f"{self.id} (v{self.version})"
@@ -51,43 +54,43 @@
     Info on a Yamcs User.
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def username(self):
+    def username(self) -> str:
         return self._proto.name
 
     @property
-    def superuser(self):
+    def superuser(self) -> bool:
         return self._proto.superuser
 
     @property
-    def system_privileges(self):
+    def system_privileges(self) -> List[str]:
         return [p for p in self._proto.systemPrivilege]
 
     @property
-    def object_privileges(self):
+    def object_privileges(self) -> List["ObjectPrivilege"]:
         return [ObjectPrivilege(p) for p in self._proto.objectPrivilege]
 
     def __str__(self):
         return self.username
 
 
 class ObjectPrivilege:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self._proto.type
 
     @property
-    def objects(self):
+    def objects(self) -> List[str]:
         return [o for o in self._proto.object]
 
     def __str__(self):
         return self.name
 
 
 class Event:
@@ -96,83 +99,79 @@
     messages in logging frameworks, but then targeted at operators.
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def generation_time(self):
+    def generation_time(self) -> datetime.datetime:
         """
         The time when the event was generated.
-
-        :type: :class:`~datetime.datetime`
         """
         if self._proto.HasField("generationTime"):
             return parse_server_time(self._proto.generationTime)
         return None
 
     @property
-    def reception_time(self):
+    def reception_time(self) -> datetime.datetime:
         """
         The time when the event was received by Yamcs.
-
-        :type: :class:`~datetime.datetime`
         """
         if self._proto.HasField("receptionTime"):
             return parse_server_time(self._proto.receptionTime)
         return None
 
     @property
-    def severity(self):
+    def severity(self) -> Optional[str]:
         """
         Severity level of the event. One of ``INFO``, ``WATCH``,
         ``WARNING``, ``DISTRESS``, ``CRITICAL`` or ``SEVERE``.
         """
         if self._proto.HasField("severity"):
             return events_pb2.Event.EventSeverity.Name(self._proto.severity)
         return None
 
     @property
-    def message(self):
+    def message(self) -> Optional[str]:
         """
         Event message.
         """
         if self._proto.HasField("message"):
             return self._proto.message
         return None
 
     @property
-    def sequence_number(self):
+    def sequence_number(self) -> int:
         """
         Sequence number. Usually this is assigned by the source of the event.
         """
         if self._proto.HasField("seqNumber"):
             return self._proto.seqNumber
         return None
 
     @property
-    def event_type(self):
+    def event_type(self) -> Optional[str]:
         """
         The event type. This is mission-specific and can be any string.
         """
         if self._proto.HasField("type"):
             return self._proto.type
         return None
 
     @property
-    def source(self):
+    def source(self) -> Optional[str]:
         """
         The event source. Can be any string.
         """
         if self._proto.HasField("source"):
             return self._proto.source
         return None
 
     @property
-    def extra(self):
+    def extra(self) -> Dict[str, str]:
         """
         Dict with extra event properties.
 
         .. versionadded:: 1.8.4
            Compatible with Yamcs 5.7.3 onwards
         """
         return {key: self._proto.extra[key] for key in self._proto.extra}
@@ -186,27 +185,25 @@
     Data holder used in link subscriptions.
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def event_type(self):
+    def event_type(self) -> str:
         """
         The type of the event. One of ``REGISTERED``, ``UNREGISTERED``,
         or ``UPDATED``.
         """
         return links_pb2.LinkEvent.Type.Name(self._proto.type)
 
     @property
-    def link(self):
+    def link(self) -> "Link":
         """
         Link state at the time of this event.
-
-        :type: :class:`.Link`
         """
         return Link(self._proto.linkInfo)
 
     def __str__(self):
         return f"[{self.event_type}] {self.link}"
 
 
@@ -219,132 +216,129 @@
 
     def __init__(self, proto):
         self._proto = proto
         self._actions = [LinkAction(action) for action in self._proto.actions]
         self._extra = {key: value for key, value in proto.extra.items()}
 
     @property
-    def instance(self):
+    def instance(self) -> str:
         """Name of the instance where this link is defined."""
         return self._proto.instance
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Name of this link (unique per instance)."""
         return self._proto.name
 
     @property
-    def class_name(self):
+    def class_name(self) -> str:
         """Name of this link's class."""
         return self._proto.type
 
     @property
-    def enabled(self):
+    def enabled(self) -> bool:
         """If ``True``, this link accepts or outputs data."""
         return not self._proto.disabled
 
     @property
-    def status(self):
+    def status(self) -> str:
         """Short status."""
         return self._proto.status
 
     @property
-    def in_count(self):
+    def in_count(self) -> int:
         """The number of inbound data events (example: packet count)."""
         return self._proto.dataInCount
 
     @property
-    def out_count(self):
+    def out_count(self) -> int:
         """The number of outbound data events (example: command count)."""
         return self._proto.dataOutCount
 
     @property
-    def actions(self):
+    def actions(self) -> List["LinkAction"]:
         """Custom actions."""
         return self._actions
 
     @property
-    def extra(self):
+    def extra(self) -> Dict[str, Any]:
         """Custom info fields."""
         return self._extra
 
     def __str__(self):
         desc = f"{self.instance}/{self.name}"
-        return f"{desc}: {self.status} (in: {self.in_count} out: {self.out_count})" \
-               f" Actions: {self._actions}"
+        return f"{desc}: {self.status} (in: {self.in_count} out: {self.out_count})"
 
 
 class LinkAction:
     def __init__(self, proto):
         self._proto = proto
 
     def __str__(self):
         return str(self._proto)
 
     @property
-    def id(self):
+    def id(self) -> str:
         """Action ID"""
         return self._proto.id
 
     @property
-    def label(self):
+    def label(self) -> str:
         """Label for the action"""
         return self._proto.label
 
     @property
-    def style(self):
+    def style(self) -> str:
         """Action style"""
         return self._proto.style
 
     @property
-    def enabled(self):
+    def enabled(self) -> bool:
         """Whether the action is currently enabled"""
         return self._proto.enabled
 
     @property
-    def checked(self):
+    def checked(self) -> bool:
         """Whether the action is currently checked"""
         return self._proto.checked
 
 
 class Instance:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Name of this instance."""
         return self._proto.name
 
     @property
-    def state(self):
+    def state(self) -> str:
         """
         State of this instance. One of ``OFFLINE``, ``INITIALIZING``,
         ``INITIALIZED``, ``STARTING``, ``RUNNING``, ``STOPPING`` or
         ``FAILED``.
         """
         if self._proto.HasField("state"):
             return yamcsManagement_pb2.YamcsInstance.InstanceState.Name(
                 self._proto.state
             )
         return None
 
     @property
-    def failure_cause(self):
+    def failure_cause(self) -> Optional[str]:
         """Failure message when ``state == 'FAILED'``"""
         if self._proto.HasField("failureCause"):
             return self._proto.failureCause
         return None
 
     @property
-    def mission_time(self):
+    def mission_time(self) -> datetime.datetime:
         """
         Mission time of this instance's time service.
-
-        :type: :class:`~datetime.datetime`
         """
         if self._proto.HasField("missionTime"):
             return parse_server_time(self._proto.missionTime)
         return None
 
     def __str__(self):
         return f"{self.name} [{self.state}]"
@@ -353,105 +347,130 @@
 class InstanceTemplate:
     """A template for creating an instance."""
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Name of this template."""
         return self._proto.name
 
     def __str__(self):
         return self.name
 
 
 class Service:
     """A Yamcs service."""
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Name of this service."""
         return self._proto.name
 
     @property
-    def instance(self):
+    def instance(self) -> str:
         """Name of the instance where this service is defined."""
         if self._proto.HasField("instance"):
             return self._proto.instance
         return None
 
     @property
-    def processor(self):
+    def processor(self) -> str:
         """Name of the processor where this service is defined."""
         if self._proto.HasField("processor"):
             return self._proto.processor
         return None
 
     @property
-    def class_name(self):
+    def class_name(self) -> str:
         """Name of this service's class."""
         return self._proto.className
 
     @property
-    def state(self):
+    def state(self) -> str:
         """State of this service."""
         if self._proto.HasField("state"):
             return yamcsManagement_pb2.ServiceState.Name(self._proto.state)
         return None
 
+    def failure_message(self) -> Optional[str]:
+        """
+        Short failure message when state is ``FAILED``
+
+        .. versionadded:: 1.9.0
+           Compatible with Yamcs 5.8.0 onwards
+        """
+        if self._proto.HasField("failureMessage"):
+            return self._proto.failureMessage
+        return None
+
+    def failure_cause(self) -> Optional[str]:
+        """
+        Java stacktrace when state is ``FAILED``
+
+        .. versionadded:: 1.9.0
+           Compatible with Yamcs 5.8.0 onwards
+        """
+        if self._proto.HasField("failureCause"):
+            return self._proto.failureCause
+        return None
+
     def __str__(self):
         return f"{self.name} [{self.state}]"
 
 
 class Processor:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Name of this processor."""
         return self._proto.name
 
     @property
-    def instance(self):
+    def instance(self) -> str:
         """Name of the instance where this processor is defined."""
         return self._proto.instance
 
     @property
-    def state(self):
+    def state(self) -> str:
         """State of this processor."""
         if self._proto.HasField("state"):
             return yamcsManagement_pb2.ServiceState.Name(self._proto.state)
         return None
 
     @property
-    def type(self):
+    def type(self) -> str:
         """Type of this processor."""
         return self._proto.type
 
     @property
-    def owner(self):
+    def owner(self) -> str:
         """User that owns this processor."""
         return self._proto.creator
 
     @property
-    def persistent(self):
+    def persistent(self) -> bool:
         """If ``True``, this processor does not close if no clients are connected."""
-        return not self._proto.persistent
+        return self._proto.persistent
 
     @property
-    def mission_time(self):
+    def protected(self) -> bool:
+        """If ``True``, this processor can not be deleted."""
+        return self._proto.protected
+
+    @property
+    def mission_time(self) -> datetime.datetime:
         """
         Mission time of this processor.
-
-        :type: :class:`~datetime.datetime`
         """
         if self._proto.HasField("time"):
             return parse_server_time(self._proto.time)
         return None
 
     def __str__(self):
         return f"{self.name} [{self.state}]"
```

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/alarms/alarms_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/alarms/alarms_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/alarms/alarms_service_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/alarms/alarms_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/archive/archive_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/archive/archive_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/archive/index_service_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/archive/index_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/archive/rocksdb_service_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/archive/rocksdb_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/audit/audit_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/audit/audit_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/buckets/buckets_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/buckets/buckets_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/commanding/clearance_service_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/commanding/clearance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/commanding/commanding_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/commanding/commanding_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='yamcs/protobuf/commanding/commanding.proto',
   package='yamcs.protobuf.commanding',
   syntax='proto2',
   serialized_options=_b('\n\022org.yamcs.protobuf'),
-  serialized_pb=_b('\n*yamcs/protobuf/commanding/commanding.proto\x12\x19yamcs.protobuf.commanding\x1a\x1ayamcs/protobuf/yamcs.proto\x1a\x1cyamcs/protobuf/mdb/mdb.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"`\n\tCommandId\x12\x16\n\x0egenerationTime\x18\x01 \x02(\x03\x12\x0e\n\x06origin\x18\x02 \x02(\t\x12\x16\n\x0esequenceNumber\x18\x03 \x02(\x05\x12\x13\n\x0b\x63ommandName\x18\x04 \x01(\t\"\x8a\x03\n\x10\x43ommandQueueInfo\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x15\n\rprocessorName\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x34\n\x05state\x18\x04 \x01(\x0e\x32%.yamcs.protobuf.commanding.QueueState\x12\x16\n\x0enbSentCommands\x18\x05 \x01(\x05\x12\x1a\n\x12nbRejectedCommands\x18\x06 \x01(\x05\x12\x1c\n\x14stateExpirationTimeS\x18\x07 \x01(\x05\x12;\n\x05\x65ntry\x18\x08 \x03(\x0b\x32,.yamcs.protobuf.commanding.CommandQueueEntry\x12\r\n\x05order\x18\t \x01(\x05\x12\r\n\x05users\x18\n \x03(\t\x12\x0e\n\x06groups\x18\x0b \x03(\t\x12L\n\x08minLevel\x18\x0c \x01(\x0e\x32:.yamcs.protobuf.mdb.SignificanceInfo.SignificanceLevelType\"\xfc\x02\n\x11\x43ommandQueueEntry\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x15\n\rprocessorName\x18\x02 \x01(\t\x12\x11\n\tqueueName\x18\x03 \x01(\t\x12\n\n\x02id\x18\x0e \x01(\t\x12\x0e\n\x06origin\x18\x0f \x01(\t\x12\x16\n\x0esequenceNumber\x18\x10 \x01(\x05\x12\x13\n\x0b\x63ommandName\x18\x11 \x01(\t\x12\x41\n\x0b\x61ssignments\x18\x12 \x03(\x0b\x32,.yamcs.protobuf.commanding.CommandAssignment\x12\x0e\n\x06\x62inary\x18\x06 \x01(\x0c\x12\x10\n\x08username\x18\x07 \x01(\t\x12\x10\n\x04uuid\x18\t \x01(\tB\x02\x18\x01\x12\x0f\n\x07\x63omment\x18\x0b \x01(\t\x12\x32\n\x0egenerationTime\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x1ependingTransmissionConstraints\x18\r \x01(\x08\"\xe8\x01\n\x11\x43ommandQueueEvent\x12?\n\x04type\x18\x01 \x01(\x0e\x32\x31.yamcs.protobuf.commanding.CommandQueueEvent.Type\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.yamcs.protobuf.commanding.CommandQueueEntry\"V\n\x04Type\x12\x11\n\rCOMMAND_ADDED\x10\x01\x12\x14\n\x10\x43OMMAND_REJECTED\x10\x02\x12\x10\n\x0c\x43OMMAND_SENT\x10\x03\x12\x13\n\x0f\x43OMMAND_UPDATED\x10\x04\"\xaf\x01\n\x13\x43ommandQueueRequest\x12>\n\tqueueInfo\x18\x01 \x01(\x0b\x32+.yamcs.protobuf.commanding.CommandQueueInfo\x12@\n\nqueueEntry\x18\x02 \x01(\x0b\x32,.yamcs.protobuf.commanding.CommandQueueEntry\x12\x16\n\x07rebuild\x18\x03 \x01(\x08:\x05\x66\x61lse\"i\n\x13\x43ommandSignificance\x12\x16\n\x0esequenceNumber\x18\x01 \x01(\x05\x12:\n\x0csignificance\x18\x02 \x01(\x0b\x32$.yamcs.protobuf.mdb.SignificanceInfo\"\xb5\x01\n\x0eVerifierConfig\x12\x0f\n\x07\x64isable\x18\x02 \x01(\x08\x12J\n\x0b\x63heckWindow\x18\x03 \x01(\x0b\x32\x35.yamcs.protobuf.commanding.VerifierConfig.CheckWindow\x1a\x46\n\x0b\x43heckWindow\x12\x1b\n\x13timeToStartChecking\x18\x01 \x01(\x03\x12\x1a\n\x12timeToStopChecking\x18\x02 \x01(\x03\"[\n\x17\x43ommandHistoryAttribute\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.yamcs.protobuf.Value\x12\x0c\n\x04time\x18\x03 \x01(\x03\"Z\n\x11\x43ommandAssignment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.yamcs.protobuf.Value\x12\x11\n\tuserInput\x18\x03 \x01(\x08\"\xd0\x02\n\x13\x43ommandHistoryEntry\x12\n\n\x02id\x18\x07 \x01(\t\x12\x13\n\x0b\x63ommandName\x18\x08 \x01(\t\x12\x0e\n\x06origin\x18\t \x01(\t\x12\x16\n\x0esequenceNumber\x18\n \x01(\x05\x12\x37\n\tcommandId\x18\x01 \x01(\x0b\x32$.yamcs.protobuf.commanding.CommandId\x12@\n\x04\x61ttr\x18\x03 \x03(\x0b\x32\x32.yamcs.protobuf.commanding.CommandHistoryAttribute\x12\x32\n\x0egenerationTime\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x41\n\x0b\x61ssignments\x18\x0b \x03(\x0b\x32,.yamcs.protobuf.commanding.CommandAssignment*4\n\nQueueState\x12\x0b\n\x07\x42LOCKED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07\x45NABLED\x10\x03\x42\x14\n\x12org.yamcs.protobuf')
+  serialized_pb=_b('\n*yamcs/protobuf/commanding/commanding.proto\x12\x19yamcs.protobuf.commanding\x1a\x1ayamcs/protobuf/yamcs.proto\x1a\x1cyamcs/protobuf/mdb/mdb.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"`\n\tCommandId\x12\x16\n\x0egenerationTime\x18\x01 \x02(\x03\x12\x0e\n\x06origin\x18\x02 \x02(\t\x12\x16\n\x0esequenceNumber\x18\x03 \x02(\x05\x12\x13\n\x0b\x63ommandName\x18\x04 \x01(\t\"\x8a\x03\n\x10\x43ommandQueueInfo\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x15\n\rprocessorName\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x34\n\x05state\x18\x04 \x01(\x0e\x32%.yamcs.protobuf.commanding.QueueState\x12\x16\n\x0enbSentCommands\x18\x05 \x01(\x05\x12\x1a\n\x12nbRejectedCommands\x18\x06 \x01(\x05\x12\x1c\n\x14stateExpirationTimeS\x18\x07 \x01(\x05\x12;\n\x05\x65ntry\x18\x08 \x03(\x0b\x32,.yamcs.protobuf.commanding.CommandQueueEntry\x12\r\n\x05order\x18\t \x01(\x05\x12\r\n\x05users\x18\n \x03(\t\x12\x0e\n\x06groups\x18\x0b \x03(\t\x12L\n\x08minLevel\x18\x0c \x01(\x0e\x32:.yamcs.protobuf.mdb.SignificanceInfo.SignificanceLevelType\"\xea\x02\n\x11\x43ommandQueueEntry\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x15\n\rprocessorName\x18\x02 \x01(\t\x12\x11\n\tqueueName\x18\x03 \x01(\t\x12\n\n\x02id\x18\x0e \x01(\t\x12\x0e\n\x06origin\x18\x0f \x01(\t\x12\x16\n\x0esequenceNumber\x18\x10 \x01(\x05\x12\x13\n\x0b\x63ommandName\x18\x11 \x01(\t\x12\x41\n\x0b\x61ssignments\x18\x12 \x03(\x0b\x32,.yamcs.protobuf.commanding.CommandAssignment\x12\x0e\n\x06\x62inary\x18\x06 \x01(\x0c\x12\x10\n\x08username\x18\x07 \x01(\t\x12\x0f\n\x07\x63omment\x18\x0b \x01(\t\x12\x32\n\x0egenerationTime\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x1ependingTransmissionConstraints\x18\r \x01(\x08\"\xe8\x01\n\x11\x43ommandQueueEvent\x12?\n\x04type\x18\x01 \x01(\x0e\x32\x31.yamcs.protobuf.commanding.CommandQueueEvent.Type\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.yamcs.protobuf.commanding.CommandQueueEntry\"V\n\x04Type\x12\x11\n\rCOMMAND_ADDED\x10\x01\x12\x14\n\x10\x43OMMAND_REJECTED\x10\x02\x12\x10\n\x0c\x43OMMAND_SENT\x10\x03\x12\x13\n\x0f\x43OMMAND_UPDATED\x10\x04\"\xaf\x01\n\x13\x43ommandQueueRequest\x12>\n\tqueueInfo\x18\x01 \x01(\x0b\x32+.yamcs.protobuf.commanding.CommandQueueInfo\x12@\n\nqueueEntry\x18\x02 \x01(\x0b\x32,.yamcs.protobuf.commanding.CommandQueueEntry\x12\x16\n\x07rebuild\x18\x03 \x01(\x08:\x05\x66\x61lse\"i\n\x13\x43ommandSignificance\x12\x16\n\x0esequenceNumber\x18\x01 \x01(\x05\x12:\n\x0csignificance\x18\x02 \x01(\x0b\x32$.yamcs.protobuf.mdb.SignificanceInfo\"\xb5\x01\n\x0eVerifierConfig\x12\x0f\n\x07\x64isable\x18\x02 \x01(\x08\x12J\n\x0b\x63heckWindow\x18\x03 \x01(\x0b\x32\x35.yamcs.protobuf.commanding.VerifierConfig.CheckWindow\x1a\x46\n\x0b\x43heckWindow\x12\x1b\n\x13timeToStartChecking\x18\x01 \x01(\x03\x12\x1a\n\x12timeToStopChecking\x18\x02 \x01(\x03\"[\n\x17\x43ommandHistoryAttribute\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.yamcs.protobuf.Value\x12\x0c\n\x04time\x18\x03 \x01(\x03\"Z\n\x11\x43ommandAssignment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.yamcs.protobuf.Value\x12\x11\n\tuserInput\x18\x03 \x01(\x08\"\xd0\x02\n\x13\x43ommandHistoryEntry\x12\n\n\x02id\x18\x07 \x01(\t\x12\x13\n\x0b\x63ommandName\x18\x08 \x01(\t\x12\x0e\n\x06origin\x18\t \x01(\t\x12\x16\n\x0esequenceNumber\x18\n \x01(\x05\x12\x37\n\tcommandId\x18\x01 \x01(\x0b\x32$.yamcs.protobuf.commanding.CommandId\x12@\n\x04\x61ttr\x18\x03 \x03(\x0b\x32\x32.yamcs.protobuf.commanding.CommandHistoryAttribute\x12\x32\n\x0egenerationTime\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x41\n\x0b\x61ssignments\x18\x0b \x03(\x0b\x32,.yamcs.protobuf.commanding.CommandAssignment*4\n\nQueueState\x12\x0b\n\x07\x42LOCKED\x10\x01\x12\x0c\n\x08\x44ISABLED\x10\x02\x12\x0b\n\x07\x45NABLED\x10\x03\x42\x14\n\x12org.yamcs.protobuf')
   ,
   dependencies=[yamcs_dot_protobuf_dot_yamcs__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_mdb_dot_mdb__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,])
 
 _QUEUESTATE = _descriptor.EnumDescriptor(
   name='QueueState',
   full_name='yamcs.protobuf.commanding.QueueState',
   filename=None,
@@ -45,16 +45,16 @@
     _descriptor.EnumValueDescriptor(
       name='ENABLED', index=2, number=3,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2270,
-  serialized_end=2322,
+  serialized_start=2252,
+  serialized_end=2304,
 )
 _sym_db.RegisterEnumDescriptor(_QUEUESTATE)
 
 QueueState = enum_type_wrapper.EnumTypeWrapper(_QUEUESTATE)
 BLOCKED = 1
 DISABLED = 2
 ENABLED = 3
@@ -81,16 +81,16 @@
     _descriptor.EnumValueDescriptor(
       name='COMMAND_UPDATED', index=3, number=4,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1189,
-  serialized_end=1275,
+  serialized_start=1171,
+  serialized_end=1257,
 )
 _sym_db.RegisterEnumDescriptor(_COMMANDQUEUEEVENT_TYPE)
 
 
 _COMMANDID = _descriptor.Descriptor(
   name='CommandId',
   full_name='yamcs.protobuf.commanding.CommandId',
@@ -325,36 +325,29 @@
       name='username', full_name='yamcs.protobuf.commanding.CommandQueueEntry.username', index=9,
       number=7, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='uuid', full_name='yamcs.protobuf.commanding.CommandQueueEntry.uuid', index=10,
-      number=9, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=_b('\030\001'), file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='comment', full_name='yamcs.protobuf.commanding.CommandQueueEntry.comment', index=11,
+      name='comment', full_name='yamcs.protobuf.commanding.CommandQueueEntry.comment', index=10,
       number=11, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='generationTime', full_name='yamcs.protobuf.commanding.CommandQueueEntry.generationTime', index=12,
+      name='generationTime', full_name='yamcs.protobuf.commanding.CommandQueueEntry.generationTime', index=11,
       number=12, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='pendingTransmissionConstraints', full_name='yamcs.protobuf.commanding.CommandQueueEntry.pendingTransmissionConstraints', index=13,
+      name='pendingTransmissionConstraints', full_name='yamcs.protobuf.commanding.CommandQueueEntry.pendingTransmissionConstraints', index=12,
       number=13, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -365,15 +358,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=660,
-  serialized_end=1040,
+  serialized_end=1022,
 )
 
 
 _COMMANDQUEUEEVENT = _descriptor.Descriptor(
   name='CommandQueueEvent',
   full_name='yamcs.protobuf.commanding.CommandQueueEvent',
   filename=None,
@@ -403,16 +396,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1043,
-  serialized_end=1275,
+  serialized_start=1025,
+  serialized_end=1257,
 )
 
 
 _COMMANDQUEUEREQUEST = _descriptor.Descriptor(
   name='CommandQueueRequest',
   full_name='yamcs.protobuf.commanding.CommandQueueRequest',
   filename=None,
@@ -448,16 +441,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1278,
-  serialized_end=1453,
+  serialized_start=1260,
+  serialized_end=1435,
 )
 
 
 _COMMANDSIGNIFICANCE = _descriptor.Descriptor(
   name='CommandSignificance',
   full_name='yamcs.protobuf.commanding.CommandSignificance',
   filename=None,
@@ -486,16 +479,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1455,
-  serialized_end=1560,
+  serialized_start=1437,
+  serialized_end=1542,
 )
 
 
 _VERIFIERCONFIG_CHECKWINDOW = _descriptor.Descriptor(
   name='CheckWindow',
   full_name='yamcs.protobuf.commanding.VerifierConfig.CheckWindow',
   filename=None,
@@ -524,16 +517,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1674,
-  serialized_end=1744,
+  serialized_start=1656,
+  serialized_end=1726,
 )
 
 _VERIFIERCONFIG = _descriptor.Descriptor(
   name='VerifierConfig',
   full_name='yamcs.protobuf.commanding.VerifierConfig',
   filename=None,
   file=DESCRIPTOR,
@@ -561,16 +554,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1563,
-  serialized_end=1744,
+  serialized_start=1545,
+  serialized_end=1726,
 )
 
 
 _COMMANDHISTORYATTRIBUTE = _descriptor.Descriptor(
   name='CommandHistoryAttribute',
   full_name='yamcs.protobuf.commanding.CommandHistoryAttribute',
   filename=None,
@@ -606,16 +599,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1746,
-  serialized_end=1837,
+  serialized_start=1728,
+  serialized_end=1819,
 )
 
 
 _COMMANDASSIGNMENT = _descriptor.Descriptor(
   name='CommandAssignment',
   full_name='yamcs.protobuf.commanding.CommandAssignment',
   filename=None,
@@ -651,16 +644,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1839,
-  serialized_end=1929,
+  serialized_start=1821,
+  serialized_end=1911,
 )
 
 
 _COMMANDHISTORYENTRY = _descriptor.Descriptor(
   name='CommandHistoryEntry',
   full_name='yamcs.protobuf.commanding.CommandHistoryEntry',
   filename=None,
@@ -731,16 +724,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1932,
-  serialized_end=2268,
+  serialized_start=1914,
+  serialized_end=2250,
 )
 
 _COMMANDQUEUEINFO.fields_by_name['state'].enum_type = _QUEUESTATE
 _COMMANDQUEUEINFO.fields_by_name['entry'].message_type = _COMMANDQUEUEENTRY
 _COMMANDQUEUEINFO.fields_by_name['minLevel'].enum_type = yamcs_dot_protobuf_dot_mdb_dot_mdb__pb2._SIGNIFICANCEINFO_SIGNIFICANCELEVELTYPE
 _COMMANDQUEUEENTRY.fields_by_name['assignments'].message_type = _COMMANDASSIGNMENT
 _COMMANDQUEUEENTRY.fields_by_name['generationTime'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
@@ -847,9 +840,8 @@
   __module__ = 'yamcs.protobuf.commanding.commanding_pb2'
   # @@protoc_insertion_point(class_scope:yamcs.protobuf.commanding.CommandHistoryEntry)
   ))
 _sym_db.RegisterMessage(CommandHistoryEntry)
 
 
 DESCRIPTOR._options = None
-_COMMANDQUEUEENTRY.fields_by_name['uuid']._options = None
 # @@protoc_insertion_point(module_scope)
```

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/commanding/commands_service_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/commanding/commands_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='yamcs/protobuf/commanding/commands_service.proto',
   package='yamcs.protobuf.commanding',
   syntax='proto2',
   serialized_options=_b('\n\022org.yamcs.protobufB\024CommandsServiceProtoP\001'),
-  serialized_pb=_b('\n0yamcs/protobuf/commanding/commands_service.proto\x12\x19yamcs.protobuf.commanding\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1byamcs/api/annotations.proto\x1a\x18yamcs/api/httpbody.proto\x1a*yamcs/protobuf/commanding/commanding.proto\x1a\x1ayamcs/protobuf/yamcs.proto\"\xd3\x01\n\x13ListCommandsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0f\n\x03pos\x18\x02 \x01(\x03\x42\x02\x18\x01\x12\r\n\x05limit\x18\x03 \x01(\x05\x12\r\n\x05order\x18\x04 \x01(\t\x12\t\n\x01q\x18\x05 \x01(\t\x12\x0c\n\x04next\x18\x06 \x01(\t\x12)\n\x05start\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05queue\x18\t \x01(\t\"\xd5\x05\n\x13IssueCommandRequest\x12\x10\n\x08instance\x18\x06 \x01(\t\x12\x11\n\tprocessor\x18\x07 \x01(\t\x12\x0c\n\x04name\x18\x08 \x01(\t\x12%\n\x04\x61rgs\x18\x10 \x01(\x0b\x32\x17.google.protobuf.Struct\x12Q\n\nassignment\x18\x01 \x03(\x0b\x32\x39.yamcs.protobuf.commanding.IssueCommandRequest.AssignmentB\x02\x18\x01\x12\x0e\n\x06origin\x18\x02 \x01(\t\x12\x16\n\x0esequenceNumber\x18\x03 \x01(\x05\x12\x0e\n\x06\x64ryRun\x18\x04 \x01(\x08\x12\x0f\n\x07\x63omment\x18\x05 \x01(\t\x12\x0e\n\x06stream\x18\x0b \x01(\t\x12&\n\x1e\x64isableTransmissionConstraints\x18\x0c \x01(\x08\x12\x18\n\x10\x64isableVerifiers\x18\r \x01(\x08\x12Z\n\x0everifierConfig\x18\x0e \x03(\x0b\x32\x42.yamcs.protobuf.commanding.IssueCommandRequest.VerifierConfigEntry\x12H\n\x05\x65xtra\x18\x0f \x03(\x0b\x32\x39.yamcs.protobuf.commanding.IssueCommandRequest.ExtraEntry\x1a)\n\nAssignment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x1a`\n\x13VerifierConfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x38\n\x05value\x18\x02 \x01(\x0b\x32).yamcs.protobuf.commanding.VerifierConfig:\x02\x38\x01\x1a\x43\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.yamcs.protobuf.Value:\x02\x38\x01\"\xb6\x02\n\x14IssueCommandResponse\x12\n\n\x02id\x18\x05 \x01(\t\x12\x32\n\x0egenerationTime\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x07 \x01(\t\x12\x16\n\x0esequenceNumber\x18\x08 \x01(\x05\x12\x13\n\x0b\x63ommandName\x18\t \x01(\t\x12\x12\n\x06source\x18\x02 \x01(\tB\x02\x18\x01\x12\x41\n\x0b\x61ssignments\x18\x0c \x03(\x0b\x32,.yamcs.protobuf.commanding.CommandAssignment\x12\x19\n\x11unprocessedBinary\x18\r \x01(\x0c\x12\x0e\n\x06\x62inary\x18\x04 \x01(\x0c\x12\x10\n\x08username\x18\x0b \x01(\t\x12\r\n\x05queue\x18\n \x01(\t\"\xa4\x01\n\x1bUpdateCommandHistoryRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\n\n\x02id\x18\x04 \x01(\t\x12\x46\n\nattributes\x18\x05 \x03(\x0b\x32\x32.yamcs.protobuf.commanding.CommandHistoryAttribute\"p\n\x14ListCommandsResponse\x12=\n\x05\x65ntry\x18\x01 \x03(\x0b\x32..yamcs.protobuf.commanding.CommandHistoryEntry\x12\x19\n\x11\x63ontinuationToken\x18\x02 \x01(\t\"1\n\x11GetCommandRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\"4\n\x14\x45xportCommandRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\"\x8c\x01\n\x15StreamCommandsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12)\n\x05start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04name\x18\x04 \x03(\t\"[\n\x18SubscribeCommandsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\x1a\n\x12ignorePastCommands\x18\x03 \x01(\x08\x32\xee\x08\n\x0b\x43ommandsApi\x12\xb1\x01\n\x0cIssueCommand\x12..yamcs.protobuf.commanding.IssueCommandRequest\x1a/.yamcs.protobuf.commanding.IssueCommandResponse\"@\x8a\x92\x03<\x1a\x37/api/processors/{instance}/{processor}/commands/{name*}:\x01*\x12\xae\x01\n\x14UpdateCommandHistory\x12\x36.yamcs.protobuf.commanding.UpdateCommandHistoryRequest\x1a\x16.google.protobuf.Empty\"F\x8a\x92\x03\x42\x1a=/api/processors/{instance}/{processor}/commandhistory/{name*}:\x01*\x12\x97\x01\n\x0cListCommands\x12..yamcs.protobuf.commanding.ListCommandsRequest\x1a/.yamcs.protobuf.commanding.ListCommandsResponse\"&\x8a\x92\x03\"\n /api/archive/{instance}/commands\x12\x97\x01\n\nGetCommand\x12,.yamcs.protobuf.commanding.GetCommandRequest\x1a..yamcs.protobuf.commanding.CommandHistoryEntry\"+\x8a\x92\x03\'\n%/api/archive/{instance}/commands/{id}\x12\xac\x01\n\x0eStreamCommands\x12\x30.yamcs.protobuf.commanding.StreamCommandsRequest\x1a..yamcs.protobuf.commanding.CommandHistoryEntry\"6\x8a\x92\x03\x32\x1a-/api/stream-archive/{instance}:streamCommands:\x01*0\x01\x12\x8a\x01\n\x11SubscribeCommands\x12\x33.yamcs.protobuf.commanding.SubscribeCommandsRequest\x1a..yamcs.protobuf.commanding.CommandHistoryEntry\"\x0e\xda\x92\x03\n\n\x08\x63ommands0\x01\x12\x89\x01\n\rExportCommand\x12/.yamcs.protobuf.commanding.ExportCommandRequest\x1a\x13.yamcs.api.HttpBody\"2\x8a\x92\x03.\n,/api/archive/{instance}/commands/{id}:exportB,\n\x12org.yamcs.protobufB\x14\x43ommandsServiceProtoP\x01')
+  serialized_pb=_b('\n0yamcs/protobuf/commanding/commands_service.proto\x12\x19yamcs.protobuf.commanding\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1byamcs/api/annotations.proto\x1a\x18yamcs/api/httpbody.proto\x1a*yamcs/protobuf/commanding/commanding.proto\x1a\x1ayamcs/protobuf/yamcs.proto\"\xd3\x01\n\x13ListCommandsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0f\n\x03pos\x18\x02 \x01(\x03\x42\x02\x18\x01\x12\r\n\x05limit\x18\x03 \x01(\x05\x12\r\n\x05order\x18\x04 \x01(\t\x12\t\n\x01q\x18\x05 \x01(\t\x12\x0c\n\x04next\x18\x06 \x01(\t\x12)\n\x05start\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05queue\x18\t \x01(\t\"\xd5\x05\n\x13IssueCommandRequest\x12\x10\n\x08instance\x18\x06 \x01(\t\x12\x11\n\tprocessor\x18\x07 \x01(\t\x12\x0c\n\x04name\x18\x08 \x01(\t\x12%\n\x04\x61rgs\x18\x10 \x01(\x0b\x32\x17.google.protobuf.Struct\x12Q\n\nassignment\x18\x01 \x03(\x0b\x32\x39.yamcs.protobuf.commanding.IssueCommandRequest.AssignmentB\x02\x18\x01\x12\x0e\n\x06origin\x18\x02 \x01(\t\x12\x16\n\x0esequenceNumber\x18\x03 \x01(\x05\x12\x0e\n\x06\x64ryRun\x18\x04 \x01(\x08\x12\x0f\n\x07\x63omment\x18\x05 \x01(\t\x12\x0e\n\x06stream\x18\x0b \x01(\t\x12&\n\x1e\x64isableTransmissionConstraints\x18\x0c \x01(\x08\x12\x18\n\x10\x64isableVerifiers\x18\r \x01(\x08\x12Z\n\x0everifierConfig\x18\x0e \x03(\x0b\x32\x42.yamcs.protobuf.commanding.IssueCommandRequest.VerifierConfigEntry\x12H\n\x05\x65xtra\x18\x0f \x03(\x0b\x32\x39.yamcs.protobuf.commanding.IssueCommandRequest.ExtraEntry\x1a)\n\nAssignment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x1a`\n\x13VerifierConfigEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x38\n\x05value\x18\x02 \x01(\x0b\x32).yamcs.protobuf.commanding.VerifierConfig:\x02\x38\x01\x1a\x43\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.yamcs.protobuf.Value:\x02\x38\x01\"\xa2\x02\n\x14IssueCommandResponse\x12\n\n\x02id\x18\x05 \x01(\t\x12\x32\n\x0egenerationTime\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06origin\x18\x07 \x01(\t\x12\x16\n\x0esequenceNumber\x18\x08 \x01(\x05\x12\x13\n\x0b\x63ommandName\x18\t \x01(\t\x12\x41\n\x0b\x61ssignments\x18\x0c \x03(\x0b\x32,.yamcs.protobuf.commanding.CommandAssignment\x12\x19\n\x11unprocessedBinary\x18\r \x01(\x0c\x12\x0e\n\x06\x62inary\x18\x04 \x01(\x0c\x12\x10\n\x08username\x18\x0b \x01(\t\x12\r\n\x05queue\x18\n \x01(\t\"\xa4\x01\n\x1bUpdateCommandHistoryRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\n\n\x02id\x18\x04 \x01(\t\x12\x46\n\nattributes\x18\x05 \x03(\x0b\x32\x32.yamcs.protobuf.commanding.CommandHistoryAttribute\"p\n\x14ListCommandsResponse\x12=\n\x05\x65ntry\x18\x01 \x03(\x0b\x32..yamcs.protobuf.commanding.CommandHistoryEntry\x12\x19\n\x11\x63ontinuationToken\x18\x02 \x01(\t\"1\n\x11GetCommandRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\"4\n\x14\x45xportCommandRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\"\x8c\x01\n\x15StreamCommandsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12)\n\x05start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04name\x18\x04 \x03(\t\"[\n\x18SubscribeCommandsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\x1a\n\x12ignorePastCommands\x18\x03 \x01(\x08\x32\xee\x08\n\x0b\x43ommandsApi\x12\xb1\x01\n\x0cIssueCommand\x12..yamcs.protobuf.commanding.IssueCommandRequest\x1a/.yamcs.protobuf.commanding.IssueCommandResponse\"@\x8a\x92\x03<\x1a\x37/api/processors/{instance}/{processor}/commands/{name*}:\x01*\x12\xae\x01\n\x14UpdateCommandHistory\x12\x36.yamcs.protobuf.commanding.UpdateCommandHistoryRequest\x1a\x16.google.protobuf.Empty\"F\x8a\x92\x03\x42\x1a=/api/processors/{instance}/{processor}/commandhistory/{name*}:\x01*\x12\x97\x01\n\x0cListCommands\x12..yamcs.protobuf.commanding.ListCommandsRequest\x1a/.yamcs.protobuf.commanding.ListCommandsResponse\"&\x8a\x92\x03\"\n /api/archive/{instance}/commands\x12\x97\x01\n\nGetCommand\x12,.yamcs.protobuf.commanding.GetCommandRequest\x1a..yamcs.protobuf.commanding.CommandHistoryEntry\"+\x8a\x92\x03\'\n%/api/archive/{instance}/commands/{id}\x12\xac\x01\n\x0eStreamCommands\x12\x30.yamcs.protobuf.commanding.StreamCommandsRequest\x1a..yamcs.protobuf.commanding.CommandHistoryEntry\"6\x8a\x92\x03\x32\x1a-/api/stream-archive/{instance}:streamCommands:\x01*0\x01\x12\x8a\x01\n\x11SubscribeCommands\x12\x33.yamcs.protobuf.commanding.SubscribeCommandsRequest\x1a..yamcs.protobuf.commanding.CommandHistoryEntry\"\x0e\xda\x92\x03\n\n\x08\x63ommands0\x01\x12\x89\x01\n\rExportCommand\x12/.yamcs.protobuf.commanding.ExportCommandRequest\x1a\x13.yamcs.api.HttpBody\"2\x8a\x92\x03.\n,/api/archive/{instance}/commands/{id}:exportB,\n\x12org.yamcs.protobufB\x14\x43ommandsServiceProtoP\x01')
   ,
   dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,google_dot_protobuf_dot_struct__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,yamcs_dot_api_dot_annotations__pb2.DESCRIPTOR,yamcs_dot_api_dot_httpbody__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_commanding_dot_commanding__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_yamcs__pb2.DESCRIPTOR,])
 
 
 
 
 _LISTCOMMANDSREQUEST = _descriptor.Descriptor(
@@ -393,50 +393,43 @@
       name='commandName', full_name='yamcs.protobuf.commanding.IssueCommandResponse.commandName', index=4,
       number=9, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='source', full_name='yamcs.protobuf.commanding.IssueCommandResponse.source', index=5,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=_b('\030\001'), file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='assignments', full_name='yamcs.protobuf.commanding.IssueCommandResponse.assignments', index=6,
+      name='assignments', full_name='yamcs.protobuf.commanding.IssueCommandResponse.assignments', index=5,
       number=12, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='unprocessedBinary', full_name='yamcs.protobuf.commanding.IssueCommandResponse.unprocessedBinary', index=7,
+      name='unprocessedBinary', full_name='yamcs.protobuf.commanding.IssueCommandResponse.unprocessedBinary', index=6,
       number=13, type=12, cpp_type=9, label=1,
       has_default_value=False, default_value=_b(""),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='binary', full_name='yamcs.protobuf.commanding.IssueCommandResponse.binary', index=8,
+      name='binary', full_name='yamcs.protobuf.commanding.IssueCommandResponse.binary', index=7,
       number=4, type=12, cpp_type=9, label=1,
       has_default_value=False, default_value=_b(""),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='username', full_name='yamcs.protobuf.commanding.IssueCommandResponse.username', index=9,
+      name='username', full_name='yamcs.protobuf.commanding.IssueCommandResponse.username', index=8,
       number=11, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='queue', full_name='yamcs.protobuf.commanding.IssueCommandResponse.queue', index=10,
+      name='queue', full_name='yamcs.protobuf.commanding.IssueCommandResponse.queue', index=9,
       number=10, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -447,15 +440,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=1241,
-  serialized_end=1551,
+  serialized_end=1531,
 )
 
 
 _UPDATECOMMANDHISTORYREQUEST = _descriptor.Descriptor(
   name='UpdateCommandHistoryRequest',
   full_name='yamcs.protobuf.commanding.UpdateCommandHistoryRequest',
   filename=None,
@@ -505,16 +498,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1554,
-  serialized_end=1718,
+  serialized_start=1534,
+  serialized_end=1698,
 )
 
 
 _LISTCOMMANDSRESPONSE = _descriptor.Descriptor(
   name='ListCommandsResponse',
   full_name='yamcs.protobuf.commanding.ListCommandsResponse',
   filename=None,
@@ -543,16 +536,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1720,
-  serialized_end=1832,
+  serialized_start=1700,
+  serialized_end=1812,
 )
 
 
 _GETCOMMANDREQUEST = _descriptor.Descriptor(
   name='GetCommandRequest',
   full_name='yamcs.protobuf.commanding.GetCommandRequest',
   filename=None,
@@ -581,16 +574,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1834,
-  serialized_end=1883,
+  serialized_start=1814,
+  serialized_end=1863,
 )
 
 
 _EXPORTCOMMANDREQUEST = _descriptor.Descriptor(
   name='ExportCommandRequest',
   full_name='yamcs.protobuf.commanding.ExportCommandRequest',
   filename=None,
@@ -619,16 +612,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1885,
-  serialized_end=1937,
+  serialized_start=1865,
+  serialized_end=1917,
 )
 
 
 _STREAMCOMMANDSREQUEST = _descriptor.Descriptor(
   name='StreamCommandsRequest',
   full_name='yamcs.protobuf.commanding.StreamCommandsRequest',
   filename=None,
@@ -671,16 +664,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1940,
-  serialized_end=2080,
+  serialized_start=1920,
+  serialized_end=2060,
 )
 
 
 _SUBSCRIBECOMMANDSREQUEST = _descriptor.Descriptor(
   name='SubscribeCommandsRequest',
   full_name='yamcs.protobuf.commanding.SubscribeCommandsRequest',
   filename=None,
@@ -716,16 +709,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2082,
-  serialized_end=2173,
+  serialized_start=2062,
+  serialized_end=2153,
 )
 
 _LISTCOMMANDSREQUEST.fields_by_name['start'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _LISTCOMMANDSREQUEST.fields_by_name['stop'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _ISSUECOMMANDREQUEST_ASSIGNMENT.containing_type = _ISSUECOMMANDREQUEST
 _ISSUECOMMANDREQUEST_VERIFIERCONFIGENTRY.fields_by_name['value'].message_type = yamcs_dot_protobuf_dot_commanding_dot_commanding__pb2._VERIFIERCONFIG
 _ISSUECOMMANDREQUEST_VERIFIERCONFIGENTRY.containing_type = _ISSUECOMMANDREQUEST
@@ -841,24 +834,23 @@
 
 
 DESCRIPTOR._options = None
 _LISTCOMMANDSREQUEST.fields_by_name['pos']._options = None
 _ISSUECOMMANDREQUEST_VERIFIERCONFIGENTRY._options = None
 _ISSUECOMMANDREQUEST_EXTRAENTRY._options = None
 _ISSUECOMMANDREQUEST.fields_by_name['assignment']._options = None
-_ISSUECOMMANDRESPONSE.fields_by_name['source']._options = None
 
 _COMMANDSAPI = _descriptor.ServiceDescriptor(
   name='CommandsApi',
   full_name='yamcs.protobuf.commanding.CommandsApi',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
-  serialized_start=2176,
-  serialized_end=3310,
+  serialized_start=2156,
+  serialized_end=3290,
   methods=[
   _descriptor.MethodDescriptor(
     name='IssueCommand',
     full_name='yamcs.protobuf.commanding.CommandsApi.IssueCommand',
     index=0,
     containing_service=None,
     input_type=_ISSUECOMMANDREQUEST,
```

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/commanding/queue_service_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/commanding/queue_service_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='yamcs/protobuf/commanding/queue_service.proto',
   package='yamcs.protobuf.commanding',
   syntax='proto2',
   serialized_options=_b('\n\022org.yamcs.protobufB\021QueueServiceProtoP\001'),
-  serialized_pb=_b('\n-yamcs/protobuf/commanding/queue_service.proto\x12\x19yamcs.protobuf.commanding\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1byamcs/api/annotations.proto\x1a*yamcs/protobuf/commanding/commanding.proto\"8\n\x11ListQueuesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\"Q\n\x12ListQueuesResponse\x12;\n\x06queues\x18\x01 \x03(\x0b\x32+.yamcs.protobuf.commanding.CommandQueueInfo\"F\n\x1fSubscribeQueueStatisticsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\"B\n\x1bSubscribeQueueEventsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\"E\n\x0fGetQueueRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\"U\n\x10\x45\x64itQueueRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\x12\r\n\x05state\x18\x04 \x01(\t\"H\n\x12\x45nableQueueRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\"I\n\x13\x44isableQueueRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\"G\n\x11\x42lockQueueRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\"O\n\x19ListQueuedCommandsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\"\\\n\x1aListQueuedCommandsResponse\x12>\n\x08\x63ommands\x18\x01 \x03(\x0b\x32,.yamcs.protobuf.commanding.CommandQueueEntry\"h\n\x15\x45\x64itQueueEntryRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\x12\x0c\n\x04uuid\x18\x04 \x01(\t\x12\r\n\x05state\x18\x05 \x01(\t\"[\n\x14\x41\x63\x63\x65ptCommandRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\"[\n\x14RejectCommandRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t2\xfb\x11\n\x08QueueApi\x12\x9e\x01\n\nListQueues\x12,.yamcs.protobuf.commanding.ListQueuesRequest\x1a-.yamcs.protobuf.commanding.ListQueuesResponse\"3\x8a\x92\x03/\n-/api/processors/{instance}/{processor}/queues\x12\xa0\x01\n\x08GetQueue\x12*.yamcs.protobuf.commanding.GetQueueRequest\x1a+.yamcs.protobuf.commanding.CommandQueueInfo\";\x8a\x92\x03\x37\n5/api/processors/{instance}/{processor}/queues/{queue}\x12\xa9\x01\n\x0bUpdateQueue\x12+.yamcs.protobuf.commanding.EditQueueRequest\x1a+.yamcs.protobuf.commanding.CommandQueueInfo\"@\x8a\x92\x03<*5/api/processors/{instance}/{processor}/queues/{queue}0\x01:\x01*\x12\xe2\x01\n\x0b\x45nableQueue\x12-.yamcs.protobuf.commanding.EnableQueueRequest\x1a+.yamcs.protobuf.commanding.CommandQueueInfo\"w\x8a\x92\x03s\x1a</api/processors/{instance}/{processor}/queues/{queue}:enableb3Queue \'{queue}\' enabled for processor \'{processor}\'\x12\xe6\x01\n\x0c\x44isableQueue\x12..yamcs.protobuf.commanding.DisableQueueRequest\x1a+.yamcs.protobuf.commanding.CommandQueueInfo\"y\x8a\x92\x03u\x1a=/api/processors/{instance}/{processor}/queues/{queue}:disableb4Queue \'{queue}\' disabled for processor \'{processor}\'\x12\xdf\x01\n\nBlockQueue\x12,.yamcs.protobuf.commanding.BlockQueueRequest\x1a+.yamcs.protobuf.commanding.CommandQueueInfo\"v\x8a\x92\x03r\x1a;/api/processors/{instance}/{processor}/queues/{queue}:blockb3Queue \'{queue}\' blocked for processor \'{processor}\'\x12\x98\x01\n\x18SubscribeQueueStatistics\x12:.yamcs.protobuf.commanding.SubscribeQueueStatisticsRequest\x1a+.yamcs.protobuf.commanding.CommandQueueInfo\"\x11\xda\x92\x03\r\n\x0bqueue-stats0\x01\x12\x92\x01\n\x14SubscribeQueueEvents\x12\x36.yamcs.protobuf.commanding.SubscribeQueueEventsRequest\x1a,.yamcs.protobuf.commanding.CommandQueueEvent\"\x12\xda\x92\x03\x0e\n\x0cqueue-events0\x01\x12\x8a\x02\n\x12ListQueuedCommands\x12\x34.yamcs.protobuf.commanding.ListQueuedCommandsRequest\x1a\x35.yamcs.protobuf.commanding.ListQueuedCommandsResponse\"\x86\x01\x8a\x92\x03\x81\x01\n>/api/processors/{instance}/{processor}/queues/{queue}/commandsZ?\n=/api/processors/{instance}/{processor}/queues/{queue}/entries\x12\xad\x01\n\x10UpdateQueueEntry\x12\x30.yamcs.protobuf.commanding.EditQueueEntryRequest\x1a\x16.google.protobuf.Empty\"O\x8a\x92\x03K*D/api/processors/{instance}/{processor}/queues/{queue}/entries/{uuid}0\x01:\x01*\x12\xaf\x01\n\rAcceptCommand\x12/.yamcs.protobuf.commanding.AcceptCommandRequest\x1a\x16.google.protobuf.Empty\"U\x8a\x92\x03Q\x1aO/api/processors/{instance}/{processor}/queues/{queue}/commands/{command}:accept\x12\xaf\x01\n\rRejectCommand\x12/.yamcs.protobuf.commanding.RejectCommandRequest\x1a\x16.google.protobuf.Empty\"U\x8a\x92\x03Q\x1aO/api/processors/{instance}/{processor}/queues/{queue}/commands/{command}:rejectB)\n\x12org.yamcs.protobufB\x11QueueServiceProtoP\x01')
+  serialized_pb=_b('\n-yamcs/protobuf/commanding/queue_service.proto\x12\x19yamcs.protobuf.commanding\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1byamcs/api/annotations.proto\x1a*yamcs/protobuf/commanding/commanding.proto\"8\n\x11ListQueuesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\"Q\n\x12ListQueuesResponse\x12;\n\x06queues\x18\x01 \x03(\x0b\x32+.yamcs.protobuf.commanding.CommandQueueInfo\"F\n\x1fSubscribeQueueStatisticsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\"B\n\x1bSubscribeQueueEventsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\"E\n\x0fGetQueueRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\"H\n\x12\x45nableQueueRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\"I\n\x13\x44isableQueueRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\"G\n\x11\x42lockQueueRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\"O\n\x19ListQueuedCommandsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\"\\\n\x1aListQueuedCommandsResponse\x12>\n\x08\x63ommands\x18\x01 \x03(\x0b\x32,.yamcs.protobuf.commanding.CommandQueueEntry\"[\n\x14\x41\x63\x63\x65ptCommandRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\"[\n\x14RejectCommandRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x02 \x01(\t\x12\r\n\x05queue\x18\x03 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t2\x9f\x0f\n\x08QueueApi\x12\x9e\x01\n\nListQueues\x12,.yamcs.protobuf.commanding.ListQueuesRequest\x1a-.yamcs.protobuf.commanding.ListQueuesResponse\"3\x8a\x92\x03/\n-/api/processors/{instance}/{processor}/queues\x12\xa0\x01\n\x08GetQueue\x12*.yamcs.protobuf.commanding.GetQueueRequest\x1a+.yamcs.protobuf.commanding.CommandQueueInfo\";\x8a\x92\x03\x37\n5/api/processors/{instance}/{processor}/queues/{queue}\x12\xe2\x01\n\x0b\x45nableQueue\x12-.yamcs.protobuf.commanding.EnableQueueRequest\x1a+.yamcs.protobuf.commanding.CommandQueueInfo\"w\x8a\x92\x03s\x1a</api/processors/{instance}/{processor}/queues/{queue}:enableb3Queue \'{queue}\' enabled for processor \'{processor}\'\x12\xe6\x01\n\x0c\x44isableQueue\x12..yamcs.protobuf.commanding.DisableQueueRequest\x1a+.yamcs.protobuf.commanding.CommandQueueInfo\"y\x8a\x92\x03u\x1a=/api/processors/{instance}/{processor}/queues/{queue}:disableb4Queue \'{queue}\' disabled for processor \'{processor}\'\x12\xdf\x01\n\nBlockQueue\x12,.yamcs.protobuf.commanding.BlockQueueRequest\x1a+.yamcs.protobuf.commanding.CommandQueueInfo\"v\x8a\x92\x03r\x1a;/api/processors/{instance}/{processor}/queues/{queue}:blockb3Queue \'{queue}\' blocked for processor \'{processor}\'\x12\x98\x01\n\x18SubscribeQueueStatistics\x12:.yamcs.protobuf.commanding.SubscribeQueueStatisticsRequest\x1a+.yamcs.protobuf.commanding.CommandQueueInfo\"\x11\xda\x92\x03\r\n\x0bqueue-stats0\x01\x12\x92\x01\n\x14SubscribeQueueEvents\x12\x36.yamcs.protobuf.commanding.SubscribeQueueEventsRequest\x1a,.yamcs.protobuf.commanding.CommandQueueEvent\"\x12\xda\x92\x03\x0e\n\x0cqueue-events0\x01\x12\x8a\x02\n\x12ListQueuedCommands\x12\x34.yamcs.protobuf.commanding.ListQueuedCommandsRequest\x1a\x35.yamcs.protobuf.commanding.ListQueuedCommandsResponse\"\x86\x01\x8a\x92\x03\x81\x01\n>/api/processors/{instance}/{processor}/queues/{queue}/commandsZ?\n=/api/processors/{instance}/{processor}/queues/{queue}/entries\x12\xaf\x01\n\rAcceptCommand\x12/.yamcs.protobuf.commanding.AcceptCommandRequest\x1a\x16.google.protobuf.Empty\"U\x8a\x92\x03Q\x1aO/api/processors/{instance}/{processor}/queues/{queue}/commands/{command}:accept\x12\xaf\x01\n\rRejectCommand\x12/.yamcs.protobuf.commanding.RejectCommandRequest\x1a\x16.google.protobuf.Empty\"U\x8a\x92\x03Q\x1aO/api/processors/{instance}/{processor}/queues/{queue}/commands/{command}:rejectB)\n\x12org.yamcs.protobufB\x11QueueServiceProtoP\x01')
   ,
   dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,yamcs_dot_api_dot_annotations__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_commanding_dot_commanding__pb2.DESCRIPTOR,])
 
 
 
 
 _LISTQUEUESREQUEST = _descriptor.Descriptor(
@@ -216,66 +216,14 @@
   oneofs=[
   ],
   serialized_start=459,
   serialized_end=528,
 )
 
 
-_EDITQUEUEREQUEST = _descriptor.Descriptor(
-  name='EditQueueRequest',
-  full_name='yamcs.protobuf.commanding.EditQueueRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='instance', full_name='yamcs.protobuf.commanding.EditQueueRequest.instance', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='processor', full_name='yamcs.protobuf.commanding.EditQueueRequest.processor', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='queue', full_name='yamcs.protobuf.commanding.EditQueueRequest.queue', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='state', full_name='yamcs.protobuf.commanding.EditQueueRequest.state', index=3,
-      number=4, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=530,
-  serialized_end=615,
-)
-
-
 _ENABLEQUEUEREQUEST = _descriptor.Descriptor(
   name='EnableQueueRequest',
   full_name='yamcs.protobuf.commanding.EnableQueueRequest',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
@@ -308,16 +256,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=617,
-  serialized_end=689,
+  serialized_start=530,
+  serialized_end=602,
 )
 
 
 _DISABLEQUEUEREQUEST = _descriptor.Descriptor(
   name='DisableQueueRequest',
   full_name='yamcs.protobuf.commanding.DisableQueueRequest',
   filename=None,
@@ -353,16 +301,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=691,
-  serialized_end=764,
+  serialized_start=604,
+  serialized_end=677,
 )
 
 
 _BLOCKQUEUEREQUEST = _descriptor.Descriptor(
   name='BlockQueueRequest',
   full_name='yamcs.protobuf.commanding.BlockQueueRequest',
   filename=None,
@@ -398,16 +346,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=766,
-  serialized_end=837,
+  serialized_start=679,
+  serialized_end=750,
 )
 
 
 _LISTQUEUEDCOMMANDSREQUEST = _descriptor.Descriptor(
   name='ListQueuedCommandsRequest',
   full_name='yamcs.protobuf.commanding.ListQueuedCommandsRequest',
   filename=None,
@@ -443,16 +391,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=839,
-  serialized_end=918,
+  serialized_start=752,
+  serialized_end=831,
 )
 
 
 _LISTQUEUEDCOMMANDSRESPONSE = _descriptor.Descriptor(
   name='ListQueuedCommandsResponse',
   full_name='yamcs.protobuf.commanding.ListQueuedCommandsResponse',
   filename=None,
@@ -474,75 +422,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=920,
-  serialized_end=1012,
-)
-
-
-_EDITQUEUEENTRYREQUEST = _descriptor.Descriptor(
-  name='EditQueueEntryRequest',
-  full_name='yamcs.protobuf.commanding.EditQueueEntryRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='instance', full_name='yamcs.protobuf.commanding.EditQueueEntryRequest.instance', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='processor', full_name='yamcs.protobuf.commanding.EditQueueEntryRequest.processor', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='queue', full_name='yamcs.protobuf.commanding.EditQueueEntryRequest.queue', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='uuid', full_name='yamcs.protobuf.commanding.EditQueueEntryRequest.uuid', index=3,
-      number=4, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='state', full_name='yamcs.protobuf.commanding.EditQueueEntryRequest.state', index=4,
-      number=5, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=_b("").decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto2',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=1014,
-  serialized_end=1118,
+  serialized_start=833,
+  serialized_end=925,
 )
 
 
 _ACCEPTCOMMANDREQUEST = _descriptor.Descriptor(
   name='AcceptCommandRequest',
   full_name='yamcs.protobuf.commanding.AcceptCommandRequest',
   filename=None,
@@ -585,16 +474,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1120,
-  serialized_end=1211,
+  serialized_start=927,
+  serialized_end=1018,
 )
 
 
 _REJECTCOMMANDREQUEST = _descriptor.Descriptor(
   name='RejectCommandRequest',
   full_name='yamcs.protobuf.commanding.RejectCommandRequest',
   filename=None,
@@ -637,32 +526,30 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1213,
-  serialized_end=1304,
+  serialized_start=1020,
+  serialized_end=1111,
 )
 
 _LISTQUEUESRESPONSE.fields_by_name['queues'].message_type = yamcs_dot_protobuf_dot_commanding_dot_commanding__pb2._COMMANDQUEUEINFO
 _LISTQUEUEDCOMMANDSRESPONSE.fields_by_name['commands'].message_type = yamcs_dot_protobuf_dot_commanding_dot_commanding__pb2._COMMANDQUEUEENTRY
 DESCRIPTOR.message_types_by_name['ListQueuesRequest'] = _LISTQUEUESREQUEST
 DESCRIPTOR.message_types_by_name['ListQueuesResponse'] = _LISTQUEUESRESPONSE
 DESCRIPTOR.message_types_by_name['SubscribeQueueStatisticsRequest'] = _SUBSCRIBEQUEUESTATISTICSREQUEST
 DESCRIPTOR.message_types_by_name['SubscribeQueueEventsRequest'] = _SUBSCRIBEQUEUEEVENTSREQUEST
 DESCRIPTOR.message_types_by_name['GetQueueRequest'] = _GETQUEUEREQUEST
-DESCRIPTOR.message_types_by_name['EditQueueRequest'] = _EDITQUEUEREQUEST
 DESCRIPTOR.message_types_by_name['EnableQueueRequest'] = _ENABLEQUEUEREQUEST
 DESCRIPTOR.message_types_by_name['DisableQueueRequest'] = _DISABLEQUEUEREQUEST
 DESCRIPTOR.message_types_by_name['BlockQueueRequest'] = _BLOCKQUEUEREQUEST
 DESCRIPTOR.message_types_by_name['ListQueuedCommandsRequest'] = _LISTQUEUEDCOMMANDSREQUEST
 DESCRIPTOR.message_types_by_name['ListQueuedCommandsResponse'] = _LISTQUEUEDCOMMANDSRESPONSE
-DESCRIPTOR.message_types_by_name['EditQueueEntryRequest'] = _EDITQUEUEENTRYREQUEST
 DESCRIPTOR.message_types_by_name['AcceptCommandRequest'] = _ACCEPTCOMMANDREQUEST
 DESCRIPTOR.message_types_by_name['RejectCommandRequest'] = _REJECTCOMMANDREQUEST
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 ListQueuesRequest = _reflection.GeneratedProtocolMessageType('ListQueuesRequest', (_message.Message,), dict(
   DESCRIPTOR = _LISTQUEUESREQUEST,
   __module__ = 'yamcs.protobuf.commanding.queue_service_pb2'
@@ -694,21 +581,14 @@
 GetQueueRequest = _reflection.GeneratedProtocolMessageType('GetQueueRequest', (_message.Message,), dict(
   DESCRIPTOR = _GETQUEUEREQUEST,
   __module__ = 'yamcs.protobuf.commanding.queue_service_pb2'
   # @@protoc_insertion_point(class_scope:yamcs.protobuf.commanding.GetQueueRequest)
   ))
 _sym_db.RegisterMessage(GetQueueRequest)
 
-EditQueueRequest = _reflection.GeneratedProtocolMessageType('EditQueueRequest', (_message.Message,), dict(
-  DESCRIPTOR = _EDITQUEUEREQUEST,
-  __module__ = 'yamcs.protobuf.commanding.queue_service_pb2'
-  # @@protoc_insertion_point(class_scope:yamcs.protobuf.commanding.EditQueueRequest)
-  ))
-_sym_db.RegisterMessage(EditQueueRequest)
-
 EnableQueueRequest = _reflection.GeneratedProtocolMessageType('EnableQueueRequest', (_message.Message,), dict(
   DESCRIPTOR = _ENABLEQUEUEREQUEST,
   __module__ = 'yamcs.protobuf.commanding.queue_service_pb2'
   # @@protoc_insertion_point(class_scope:yamcs.protobuf.commanding.EnableQueueRequest)
   ))
 _sym_db.RegisterMessage(EnableQueueRequest)
 
@@ -736,21 +616,14 @@
 ListQueuedCommandsResponse = _reflection.GeneratedProtocolMessageType('ListQueuedCommandsResponse', (_message.Message,), dict(
   DESCRIPTOR = _LISTQUEUEDCOMMANDSRESPONSE,
   __module__ = 'yamcs.protobuf.commanding.queue_service_pb2'
   # @@protoc_insertion_point(class_scope:yamcs.protobuf.commanding.ListQueuedCommandsResponse)
   ))
 _sym_db.RegisterMessage(ListQueuedCommandsResponse)
 
-EditQueueEntryRequest = _reflection.GeneratedProtocolMessageType('EditQueueEntryRequest', (_message.Message,), dict(
-  DESCRIPTOR = _EDITQUEUEENTRYREQUEST,
-  __module__ = 'yamcs.protobuf.commanding.queue_service_pb2'
-  # @@protoc_insertion_point(class_scope:yamcs.protobuf.commanding.EditQueueEntryRequest)
-  ))
-_sym_db.RegisterMessage(EditQueueEntryRequest)
-
 AcceptCommandRequest = _reflection.GeneratedProtocolMessageType('AcceptCommandRequest', (_message.Message,), dict(
   DESCRIPTOR = _ACCEPTCOMMANDREQUEST,
   __module__ = 'yamcs.protobuf.commanding.queue_service_pb2'
   # @@protoc_insertion_point(class_scope:yamcs.protobuf.commanding.AcceptCommandRequest)
   ))
 _sym_db.RegisterMessage(AcceptCommandRequest)
 
@@ -766,16 +639,16 @@
 
 _QUEUEAPI = _descriptor.ServiceDescriptor(
   name='QueueApi',
   full_name='yamcs.protobuf.commanding.QueueApi',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
-  serialized_start=1307,
-  serialized_end=3606,
+  serialized_start=1114,
+  serialized_end=3065,
   methods=[
   _descriptor.MethodDescriptor(
     name='ListQueues',
     full_name='yamcs.protobuf.commanding.QueueApi.ListQueues',
     index=0,
     containing_service=None,
     input_type=_LISTQUEUESREQUEST,
@@ -788,98 +661,80 @@
     index=1,
     containing_service=None,
     input_type=_GETQUEUEREQUEST,
     output_type=yamcs_dot_protobuf_dot_commanding_dot_commanding__pb2._COMMANDQUEUEINFO,
     serialized_options=_b('\212\222\0037\n5/api/processors/{instance}/{processor}/queues/{queue}'),
   ),
   _descriptor.MethodDescriptor(
-    name='UpdateQueue',
-    full_name='yamcs.protobuf.commanding.QueueApi.UpdateQueue',
-    index=2,
-    containing_service=None,
-    input_type=_EDITQUEUEREQUEST,
-    output_type=yamcs_dot_protobuf_dot_commanding_dot_commanding__pb2._COMMANDQUEUEINFO,
-    serialized_options=_b('\212\222\003<*5/api/processors/{instance}/{processor}/queues/{queue}0\001:\001*'),
-  ),
-  _descriptor.MethodDescriptor(
     name='EnableQueue',
     full_name='yamcs.protobuf.commanding.QueueApi.EnableQueue',
-    index=3,
+    index=2,
     containing_service=None,
     input_type=_ENABLEQUEUEREQUEST,
     output_type=yamcs_dot_protobuf_dot_commanding_dot_commanding__pb2._COMMANDQUEUEINFO,
     serialized_options=_b('\212\222\003s\032</api/processors/{instance}/{processor}/queues/{queue}:enableb3Queue \'{queue}\' enabled for processor \'{processor}\''),
   ),
   _descriptor.MethodDescriptor(
     name='DisableQueue',
     full_name='yamcs.protobuf.commanding.QueueApi.DisableQueue',
-    index=4,
+    index=3,
     containing_service=None,
     input_type=_DISABLEQUEUEREQUEST,
     output_type=yamcs_dot_protobuf_dot_commanding_dot_commanding__pb2._COMMANDQUEUEINFO,
     serialized_options=_b('\212\222\003u\032=/api/processors/{instance}/{processor}/queues/{queue}:disableb4Queue \'{queue}\' disabled for processor \'{processor}\''),
   ),
   _descriptor.MethodDescriptor(
     name='BlockQueue',
     full_name='yamcs.protobuf.commanding.QueueApi.BlockQueue',
-    index=5,
+    index=4,
     containing_service=None,
     input_type=_BLOCKQUEUEREQUEST,
     output_type=yamcs_dot_protobuf_dot_commanding_dot_commanding__pb2._COMMANDQUEUEINFO,
     serialized_options=_b('\212\222\003r\032;/api/processors/{instance}/{processor}/queues/{queue}:blockb3Queue \'{queue}\' blocked for processor \'{processor}\''),
   ),
   _descriptor.MethodDescriptor(
     name='SubscribeQueueStatistics',
     full_name='yamcs.protobuf.commanding.QueueApi.SubscribeQueueStatistics',
-    index=6,
+    index=5,
     containing_service=None,
     input_type=_SUBSCRIBEQUEUESTATISTICSREQUEST,
     output_type=yamcs_dot_protobuf_dot_commanding_dot_commanding__pb2._COMMANDQUEUEINFO,
     serialized_options=_b('\332\222\003\r\n\013queue-stats'),
   ),
   _descriptor.MethodDescriptor(
     name='SubscribeQueueEvents',
     full_name='yamcs.protobuf.commanding.QueueApi.SubscribeQueueEvents',
-    index=7,
+    index=6,
     containing_service=None,
     input_type=_SUBSCRIBEQUEUEEVENTSREQUEST,
     output_type=yamcs_dot_protobuf_dot_commanding_dot_commanding__pb2._COMMANDQUEUEEVENT,
     serialized_options=_b('\332\222\003\016\n\014queue-events'),
   ),
   _descriptor.MethodDescriptor(
     name='ListQueuedCommands',
     full_name='yamcs.protobuf.commanding.QueueApi.ListQueuedCommands',
-    index=8,
+    index=7,
     containing_service=None,
     input_type=_LISTQUEUEDCOMMANDSREQUEST,
     output_type=_LISTQUEUEDCOMMANDSRESPONSE,
     serialized_options=_b('\212\222\003\201\001\n>/api/processors/{instance}/{processor}/queues/{queue}/commandsZ?\n=/api/processors/{instance}/{processor}/queues/{queue}/entries'),
   ),
   _descriptor.MethodDescriptor(
-    name='UpdateQueueEntry',
-    full_name='yamcs.protobuf.commanding.QueueApi.UpdateQueueEntry',
-    index=9,
-    containing_service=None,
-    input_type=_EDITQUEUEENTRYREQUEST,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=_b('\212\222\003K*D/api/processors/{instance}/{processor}/queues/{queue}/entries/{uuid}0\001:\001*'),
-  ),
-  _descriptor.MethodDescriptor(
     name='AcceptCommand',
     full_name='yamcs.protobuf.commanding.QueueApi.AcceptCommand',
-    index=10,
+    index=8,
     containing_service=None,
     input_type=_ACCEPTCOMMANDREQUEST,
     output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     serialized_options=_b('\212\222\003Q\032O/api/processors/{instance}/{processor}/queues/{queue}/commands/{command}:accept'),
   ),
   _descriptor.MethodDescriptor(
     name='RejectCommand',
     full_name='yamcs.protobuf.commanding.QueueApi.RejectCommand',
-    index=11,
+    index=9,
     containing_service=None,
     input_type=_REJECTCOMMANDREQUEST,
     output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     serialized_options=_b('\212\222\003Q\032O/api/processors/{instance}/{processor}/queues/{queue}/commands/{command}:reject'),
   ),
 ])
 _sym_db.RegisterServiceDescriptor(_QUEUEAPI)
```

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/cop1/cop1_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/cop1/cop1_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/database/database_service_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/database/database_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/events/events_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/events/events_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/events/events_service_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/events/events_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/iam/iam_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/iam/iam_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/iam/sessions_service_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/iam/sessions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/links/links_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/links/links_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/mdb/mdb_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/mdb/mdb_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='yamcs/protobuf/mdb/mdb.proto',
   package='yamcs.protobuf.mdb',
   syntax='proto2',
   serialized_options=_b('\n\022org.yamcs.protobuf'),
-  serialized_pb=_b('\n\x1cyamcs/protobuf/mdb/mdb.proto\x12\x12yamcs.protobuf.mdb\x1a\x1byamcs/api/annotations.proto\x1a\x18yamcs/api/httpbody.proto\x1a\x1ayamcs/protobuf/yamcs.proto\"\xf8\x01\n\x0fMissionDatabase\x12\x12\n\nconfigName\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x38\n\x0bspaceSystem\x18\x04 \x03(\x0b\x32#.yamcs.protobuf.mdb.SpaceSystemInfo\x12\x16\n\x0eparameterCount\x18\x06 \x01(\x05\x12\x16\n\x0e\x63ontainerCount\x18\x07 \x01(\x05\x12\x14\n\x0c\x63ommandCount\x18\x08 \x01(\x05\x12\x16\n\x0e\x61lgorithmCount\x18\t \x01(\x05\x12\x1a\n\x12parameterTypeCount\x18\n \x01(\x05\"M\n\x0bHistoryInfo\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x04 \x01(\t\"\x18\n\x08UnitInfo\x12\x0c\n\x04unit\x18\x01 \x01(\t\"\x97\x01\n\nAlarmRange\x12\x31\n\x05level\x18\x01 \x01(\x0e\x32\".yamcs.protobuf.mdb.AlarmLevelType\x12\x14\n\x0cminInclusive\x18\x02 \x01(\x01\x12\x14\n\x0cmaxInclusive\x18\x03 \x01(\x01\x12\x14\n\x0cminExclusive\x18\x04 \x01(\x01\x12\x14\n\x0cmaxExclusive\x18\x05 \x01(\x01\"T\n\x10\x45numerationAlarm\x12\x31\n\x05level\x18\x01 \x01(\x0e\x32\".yamcs.protobuf.mdb.AlarmLevelType\x12\r\n\x05label\x18\x03 \x01(\t\"\x9c\x01\n\tAlarmInfo\x12\x15\n\rminViolations\x18\x01 \x01(\x05\x12\x38\n\x10staticAlarmRange\x18\x02 \x03(\x0b\x32\x1e.yamcs.protobuf.mdb.AlarmRange\x12>\n\x10\x65numerationAlarm\x18\x03 \x03(\x0b\x32$.yamcs.protobuf.mdb.EnumerationAlarm\"\x89\x01\n\x10\x43ontextAlarmInfo\x12\x36\n\ncomparison\x18\x01 \x03(\x0b\x32\".yamcs.protobuf.mdb.ComparisonInfo\x12,\n\x05\x61larm\x18\x02 \x01(\x0b\x32\x1d.yamcs.protobuf.mdb.AlarmInfo\x12\x0f\n\x07\x63ontext\x18\x03 \x01(\t\"\xd1\x02\n\x10\x44\x61taEncodingInfo\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32).yamcs.protobuf.mdb.DataEncodingInfo.Type\x12\x14\n\x0clittleEndian\x18\x02 \x01(\x08\x12\x12\n\nsizeInBits\x18\x03 \x01(\x05\x12\x10\n\x08\x65ncoding\x18\x04 \x01(\t\x12=\n\x11\x64\x65\x66\x61ultCalibrator\x18\x06 \x01(\x0b\x32\".yamcs.protobuf.mdb.CalibratorInfo\x12\x44\n\x11\x63ontextCalibrator\x18\x07 \x03(\x0b\x32).yamcs.protobuf.mdb.ContextCalibratorInfo\"C\n\x04Type\x12\n\n\x06\x42INARY\x10\x00\x12\x0b\n\x07\x42OOLEAN\x10\x01\x12\t\n\x05\x46LOAT\x10\x02\x12\x0b\n\x07INTEGER\x10\x03\x12\n\n\x06STRING\x10\x04\"\x98\x01\n\x15\x43ontextCalibratorInfo\x12\x36\n\ncomparison\x18\x01 \x03(\x0b\x32\".yamcs.protobuf.mdb.ComparisonInfo\x12\x36\n\ncalibrator\x18\x02 \x01(\x0b\x32\".yamcs.protobuf.mdb.CalibratorInfo\x12\x0f\n\x07\x63ontext\x18\x03 \x01(\t\"\xf8\x02\n\x0e\x43\x61libratorInfo\x12J\n\x14polynomialCalibrator\x18\x02 \x01(\x0b\x32,.yamcs.protobuf.mdb.PolynomialCalibratorInfo\x12\x42\n\x10splineCalibrator\x18\x03 \x01(\x0b\x32(.yamcs.protobuf.mdb.SplineCalibratorInfo\x12R\n\x18javaExpressionCalibrator\x18\x04 \x01(\x0b\x32\x30.yamcs.protobuf.mdb.JavaExpressionCalibratorInfo\x12\x35\n\x04type\x18\x05 \x01(\x0e\x32\'.yamcs.protobuf.mdb.CalibratorInfo.Type\"K\n\x04Type\x12\x0e\n\nPOLYNOMIAL\x10\x00\x12\n\n\x06SPLINE\x10\x01\x12\x12\n\x0eMATH_OPERATION\x10\x02\x12\x13\n\x0fJAVA_EXPRESSION\x10\x03\"/\n\x18PolynomialCalibratorInfo\x12\x13\n\x0b\x63oefficient\x18\x01 \x03(\x01\"\x93\x01\n\x14SplineCalibratorInfo\x12G\n\x05point\x18\x01 \x03(\x0b\x32\x38.yamcs.protobuf.mdb.SplineCalibratorInfo.SplinePointInfo\x1a\x32\n\x0fSplinePointInfo\x12\x0b\n\x03raw\x18\x01 \x01(\x01\x12\x12\n\ncalibrated\x18\x02 \x01(\x01\"/\n\x1cJavaExpressionCalibratorInfo\x12\x0f\n\x07\x66ormula\x18\x01 \x01(\t\">\n\tEnumValue\x12\r\n\x05value\x18\x01 \x01(\x03\x12\r\n\x05label\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\"\xd2\x05\n\x11ParameterTypeInfo\x12\x0f\n\x07\x65ngType\x18\x01 \x01(\t\x12:\n\x0c\x64\x61taEncoding\x18\x02 \x01(\x0b\x32$.yamcs.protobuf.mdb.DataEncodingInfo\x12-\n\x07unitSet\x18\x03 \x03(\x0b\x32\x1c.yamcs.protobuf.mdb.UnitInfo\x12\x33\n\x0c\x64\x65\x66\x61ultAlarm\x18\x04 \x01(\x0b\x32\x1d.yamcs.protobuf.mdb.AlarmInfo\x12\x30\n\tenumValue\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.mdb.EnumValue\x12>\n\x10\x61\x62soluteTimeInfo\x18\x06 \x01(\x0b\x32$.yamcs.protobuf.mdb.AbsoluteTimeInfo\x12:\n\x0c\x63ontextAlarm\x18\x07 \x03(\x0b\x32$.yamcs.protobuf.mdb.ContextAlarmInfo\x12.\n\x06member\x18\x08 \x03(\x0b\x32\x1e.yamcs.protobuf.mdb.MemberInfo\x12\x30\n\tarrayInfo\x18\t \x01(\x0b\x32\x1d.yamcs.protobuf.mdb.ArrayInfo\x12O\n\rancillaryData\x18\n \x03(\x0b\x32\x38.yamcs.protobuf.mdb.ParameterTypeInfo.AncillaryDataEntry\x12>\n\x0cnumberFormat\x18\x0b \x01(\x0b\x32(.yamcs.protobuf.mdb.NumberFormatTypeInfo\x12\x0e\n\x06signed\x18\x0c \x01(\x08\x1a[\n\x12\x41ncillaryDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.yamcs.protobuf.mdb.AncillaryDataInfo:\x02\x38\x01\"\xb5\x02\n\x14NumberFormatTypeInfo\x12\x12\n\nnumberBase\x18\x01 \x01(\t\x12\x1d\n\x15minimumFractionDigits\x18\x02 \x01(\x05\x12\x1d\n\x15maximumFractionDigits\x18\x03 \x01(\x05\x12\x1c\n\x14minimumIntegerDigits\x18\x04 \x01(\x05\x12\x1c\n\x14maximumIntegerDigits\x18\x05 \x01(\x05\x12\x16\n\x0enegativeSuffix\x18\x06 \x01(\t\x12\x16\n\x0epositiveSuffix\x18\x07 \x01(\t\x12\x16\n\x0enegativePrefix\x18\x08 \x01(\t\x12\x16\n\x0epositivePrefix\x18\t \x01(\t\x12\x1d\n\x15showThousandsGrouping\x18\n \x01(\x08\x12\x10\n\x08notation\x18\x0b \x01(\t\"5\n\x13GetContainerRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x8d\x01\n\x10\x41\x62soluteTimeInfo\x12\x14\n\x0cinitialValue\x18\x01 \x01(\t\x12\r\n\x05scale\x18\x02 \x01(\x01\x12\x0e\n\x06offset\x18\x03 \x01(\x01\x12\x35\n\noffsetFrom\x18\x04 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\r\n\x05\x65poch\x18\x05 \x01(\t\"\xb0\x01\n\nMemberInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x33\n\x04type\x18\x06 \x01(\x0b\x32%.yamcs.protobuf.mdb.ParameterTypeInfo\"\xcd\x01\n\x12\x41rgumentMemberInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x32\n\x04type\x18\x06 \x01(\x0b\x32$.yamcs.protobuf.mdb.ArgumentTypeInfo\x12\x14\n\x0cinitialValue\x18\x07 \x01(\t\"\x84\x01\n\x16ParameterDimensionInfo\x12\x12\n\nfixedValue\x18\x01 \x01(\x03\x12\x34\n\tparameter\x18\x02 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\r\n\x05slope\x18\x03 \x01(\x03\x12\x11\n\tintercept\x18\x04 \x01(\x03\"\x80\x01\n\tArrayInfo\x12\x33\n\x04type\x18\x01 \x01(\x0b\x32%.yamcs.protobuf.mdb.ParameterTypeInfo\x12>\n\ndimensions\x18\x03 \x03(\x0b\x32*.yamcs.protobuf.mdb.ParameterDimensionInfo\"x\n\nUsedByInfo\x12\x34\n\talgorithm\x18\x01 \x03(\x0b\x32!.yamcs.protobuf.mdb.AlgorithmInfo\x12\x34\n\tcontainer\x18\x02 \x03(\x0b\x32!.yamcs.protobuf.mdb.ContainerInfo\"\xea\x03\n\rParameterInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rqualifiedName\x18\x02 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x33\n\x04type\x18\x06 \x01(\x0b\x32%.yamcs.protobuf.mdb.ParameterTypeInfo\x12\x36\n\ndataSource\x18\x07 \x01(\x0e\x32\".yamcs.protobuf.mdb.DataSourceType\x12.\n\x06usedBy\x18\x08 \x01(\x0b\x32\x1e.yamcs.protobuf.mdb.UsedByInfo\x12K\n\rancillaryData\x18\t \x03(\x0b\x32\x34.yamcs.protobuf.mdb.ParameterInfo.AncillaryDataEntry\x12\x0c\n\x04path\x18\n \x03(\t\x1a[\n\x12\x41ncillaryDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.yamcs.protobuf.mdb.AncillaryDataInfo:\x02\x38\x01\"B\n\x11\x41ncillaryDataInfo\x12\r\n\x05value\x18\x01 \x01(\t\x12\x10\n\x08mimeType\x18\x02 \x01(\t\x12\x0c\n\x04href\x18\x03 \x01(\t\"\x9f\x04\n\x10\x41rgumentTypeInfo\x12\x0f\n\x07\x65ngType\x18\x01 \x01(\t\x12:\n\x0c\x64\x61taEncoding\x18\x02 \x01(\x0b\x32$.yamcs.protobuf.mdb.DataEncodingInfo\x12-\n\x07unitSet\x18\x03 \x03(\x0b\x32\x1c.yamcs.protobuf.mdb.UnitInfo\x12\x30\n\tenumValue\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.mdb.EnumValue\x12\x10\n\x08rangeMin\x18\x06 \x01(\x01\x12\x10\n\x08rangeMax\x18\x07 \x01(\x01\x12\x36\n\x06member\x18\x08 \x03(\x0b\x32&.yamcs.protobuf.mdb.ArgumentMemberInfo\x12\x17\n\x0fzeroStringValue\x18\t \x01(\t\x12\x16\n\x0eoneStringValue\x18\n \x01(\t\x12\x10\n\x08minChars\x18\x0b \x01(\x05\x12\x10\n\x08maxChars\x18\x0c \x01(\x05\x12\x0e\n\x06signed\x18\r \x01(\x08\x12\x10\n\x08minBytes\x18\x0e \x01(\x05\x12\x10\n\x08maxBytes\x18\x0f \x01(\x05\x12=\n\ndimensions\x18\x10 \x03(\x0b\x32).yamcs.protobuf.mdb.ArgumentDimensionInfo\x12\x39\n\x0b\x65lementType\x18\x11 \x01(\x0b\x32$.yamcs.protobuf.mdb.ArgumentTypeInfo\"\x95\x01\n\x15\x41rgumentDimensionInfo\x12\x12\n\nfixedValue\x18\x01 \x01(\x03\x12\x34\n\tparameter\x18\x02 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x10\n\x08\x61rgument\x18\x03 \x01(\t\x12\r\n\x05slope\x18\x04 \x01(\x03\x12\x11\n\tintercept\x18\x05 \x01(\x03\"{\n\x0c\x41rgumentInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x14\n\x0cinitialValue\x18\x04 \x01(\t\x12\x32\n\x04type\x18\x06 \x01(\x0b\x32$.yamcs.protobuf.mdb.ArgumentTypeInfo\"5\n\x16\x41rgumentAssignmentInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xe5\x01\n\x10SignificanceInfo\x12T\n\x10\x63onsequenceLevel\x18\x01 \x01(\x0e\x32:.yamcs.protobuf.mdb.SignificanceInfo.SignificanceLevelType\x12\x18\n\x10reasonForWarning\x18\x02 \x01(\t\"a\n\x15SignificanceLevelType\x12\x08\n\x04NONE\x10\x01\x12\t\n\x05WATCH\x10\x02\x12\x0b\n\x07WARNING\x10\x03\x12\x0c\n\x08\x44ISTRESS\x10\x04\x12\x0c\n\x08\x43RITICAL\x10\x05\x12\n\n\x06SEVERE\x10\x06\"\xdd\x02\n\x0e\x43omparisonInfo\x12\x34\n\tparameter\x18\x01 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x41\n\x08operator\x18\x02 \x01(\x0e\x32/.yamcs.protobuf.mdb.ComparisonInfo.OperatorType\x12\r\n\x05value\x18\x03 \x01(\t\x12\x32\n\x08\x61rgument\x18\x04 \x01(\x0b\x32 .yamcs.protobuf.mdb.ArgumentInfo\"\x8e\x01\n\x0cOperatorType\x12\x0c\n\x08\x45QUAL_TO\x10\x01\x12\x10\n\x0cNOT_EQUAL_TO\x10\x02\x12\x10\n\x0cGREATER_THAN\x10\x03\x12\x1c\n\x18GREATER_THAN_OR_EQUAL_TO\x10\x04\x12\x10\n\x0cSMALLER_THAN\x10\x05\x12\x1c\n\x18SMALLER_THAN_OR_EQUAL_TO\x10\x06\"A\n\x1aTransmissionConstraintInfo\x12\x12\n\nexpression\x18\x03 \x01(\t\x12\x0f\n\x07timeout\x18\x02 \x01(\x03\"\xf7\x05\n\x0b\x43ommandInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rqualifiedName\x18\x02 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x34\n\x0b\x62\x61seCommand\x18\x06 \x01(\x0b\x32\x1f.yamcs.protobuf.mdb.CommandInfo\x12\x10\n\x08\x61\x62stract\x18\x07 \x01(\x08\x12\x32\n\x08\x61rgument\x18\x08 \x03(\x0b\x32 .yamcs.protobuf.mdb.ArgumentInfo\x12\x46\n\x12\x61rgumentAssignment\x18\t \x03(\x0b\x32*.yamcs.protobuf.mdb.ArgumentAssignmentInfo\x12:\n\x0csignificance\x18\n \x01(\x0b\x32$.yamcs.protobuf.mdb.SignificanceInfo\x12\x42\n\nconstraint\x18\x0b \x03(\x0b\x32..yamcs.protobuf.mdb.TransmissionConstraintInfo\x12\x42\n\x10\x63ommandContainer\x18\r \x01(\x0b\x32(.yamcs.protobuf.mdb.CommandContainerInfo\x12\x32\n\x08verifier\x18\x0e \x03(\x0b\x32 .yamcs.protobuf.mdb.VerifierInfo\x12I\n\rancillaryData\x18\x0f \x03(\x0b\x32\x32.yamcs.protobuf.mdb.CommandInfo.AncillaryDataEntry\x1a[\n\x12\x41ncillaryDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.yamcs.protobuf.mdb.AncillaryDataInfo:\x02\x38\x01\"\xd1\x03\n\x0cVerifierInfo\x12\r\n\x05stage\x18\x01 \x01(\t\x12\x34\n\tcontainer\x18\x02 \x01(\x0b\x32!.yamcs.protobuf.mdb.ContainerInfo\x12\x34\n\talgorithm\x18\x03 \x01(\x0b\x32!.yamcs.protobuf.mdb.AlgorithmInfo\x12I\n\tonSuccess\x18\x04 \x01(\x0e\x32\x36.yamcs.protobuf.mdb.VerifierInfo.TerminationActionType\x12\x46\n\x06onFail\x18\x05 \x01(\x0e\x32\x36.yamcs.protobuf.mdb.VerifierInfo.TerminationActionType\x12I\n\tonTimeout\x18\x06 \x01(\x0e\x32\x36.yamcs.protobuf.mdb.VerifierInfo.TerminationActionType\x12\x38\n\x0b\x63heckWindow\x18\x07 \x01(\x0b\x32#.yamcs.protobuf.mdb.CheckWindowInfo\".\n\x15TerminationActionType\x12\x0b\n\x07SUCCESS\x10\x01\x12\x08\n\x04\x46\x41IL\x10\x02\"^\n\x0f\x43heckWindowInfo\x12\x1b\n\x13timeToStartChecking\x18\x01 \x01(\x03\x12\x1a\n\x12timeToStopChecking\x18\x02 \x01(\x03\x12\x12\n\nrelativeTo\x18\x03 \x01(\t\"n\n\nRepeatInfo\x12\x12\n\nfixedCount\x18\x01 \x01(\x03\x12\x37\n\x0c\x64ynamicCount\x18\x02 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x13\n\x0b\x62itsBetween\x18\x03 \x01(\x05\"\xcd\x03\n\x11SequenceEntryInfo\x12\x16\n\x0elocationInBits\x18\x01 \x01(\x05\x12V\n\x11referenceLocation\x18\x02 \x01(\x0e\x32;.yamcs.protobuf.mdb.SequenceEntryInfo.ReferenceLocationType\x12\x34\n\tcontainer\x18\x03 \x01(\x0b\x32!.yamcs.protobuf.mdb.ContainerInfo\x12\x34\n\tparameter\x18\x04 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x32\n\x08\x61rgument\x18\x06 \x01(\x0b\x32 .yamcs.protobuf.mdb.ArgumentInfo\x12\x36\n\nfixedValue\x18\x07 \x01(\x0b\x32\".yamcs.protobuf.mdb.FixedValueInfo\x12.\n\x06repeat\x18\x05 \x01(\x0b\x32\x1e.yamcs.protobuf.mdb.RepeatInfo\"@\n\x15ReferenceLocationType\x12\x13\n\x0f\x43ONTAINER_START\x10\x01\x12\x12\n\x0ePREVIOUS_ENTRY\x10\x02\"D\n\x0e\x46ixedValueInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08hexValue\x18\x02 \x01(\t\x12\x12\n\nsizeInBits\x18\x03 \x01(\x05\"\xa7\x02\n\x14\x43ommandContainerInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rqualifiedName\x18\x02 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x12\n\nsizeInBits\x18\x06 \x01(\x05\x12?\n\rbaseContainer\x18\x07 \x01(\x0b\x32(.yamcs.protobuf.mdb.CommandContainerInfo\x12\x34\n\x05\x65ntry\x18\x08 \x03(\x0b\x32%.yamcs.protobuf.mdb.SequenceEntryInfo\"\xc9\x04\n\rContainerInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rqualifiedName\x18\x02 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x13\n\x0bmaxInterval\x18\x06 \x01(\x03\x12\x12\n\nsizeInBits\x18\x07 \x01(\x05\x12\x38\n\rbaseContainer\x18\x08 \x01(\x0b\x32!.yamcs.protobuf.mdb.ContainerInfo\x12?\n\x13restrictionCriteria\x18\t \x03(\x0b\x32\".yamcs.protobuf.mdb.ComparisonInfo\x12\x34\n\x05\x65ntry\x18\n \x03(\x0b\x32%.yamcs.protobuf.mdb.SequenceEntryInfo\x12.\n\x06usedBy\x18\x0b \x01(\x0b\x32\x1e.yamcs.protobuf.mdb.UsedByInfo\x12K\n\rancillaryData\x18\x0c \x03(\x0b\x32\x34.yamcs.protobuf.mdb.ContainerInfo.AncillaryDataEntry\x1a[\n\x12\x41ncillaryDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.yamcs.protobuf.mdb.AncillaryDataInfo:\x02\x38\x01\"\xbf\x01\n\x12InputParameterInfo\x12\x34\n\tparameter\x18\x01 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x11\n\tinputName\x18\x02 \x01(\t\x12\x19\n\x11parameterInstance\x18\x03 \x01(\x05\x12\x11\n\tmandatory\x18\x04 \x01(\x08\x12\x32\n\x08\x61rgument\x18\x05 \x01(\x0b\x32 .yamcs.protobuf.mdb.ArgumentInfo\"_\n\x13OutputParameterInfo\x12\x34\n\tparameter\x18\x01 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x12\n\noutputName\x18\x02 \x01(\t\"\x8e\x04\n\rAlgorithmInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rqualifiedName\x18\x02 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x36\n\x05scope\x18\x06 \x01(\x0e\x32\'.yamcs.protobuf.mdb.AlgorithmInfo.Scope\x12\x10\n\x08language\x18\x07 \x01(\t\x12\x0c\n\x04text\x18\x08 \x01(\t\x12>\n\x0einputParameter\x18\t \x03(\x0b\x32&.yamcs.protobuf.mdb.InputParameterInfo\x12@\n\x0foutputParameter\x18\n \x03(\x0b\x32\'.yamcs.protobuf.mdb.OutputParameterInfo\x12<\n\x11onParameterUpdate\x18\x0b \x03(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x16\n\x0eonPeriodicRate\x18\x0c \x03(\x03\"G\n\x05Scope\x12\n\n\x06GLOBAL\x10\x00\x12\x18\n\x14\x43OMMAND_VERIFICATION\x10\x01\x12\x18\n\x14\x43ONTAINER_PROCESSING\x10\x02\"`\n\x17ListSpaceSystemsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\t\n\x01q\x18\x02 \x01(\t\x12\x0c\n\x04next\x18\x07 \x01(\t\x12\x0b\n\x03pos\x18\x08 \x01(\x05\x12\r\n\x05limit\x18\t \x01(\x05\"n\n\x15ListContainersRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\t\n\x01q\x18\x02 \x01(\t\x12\x0e\n\x06system\x18\n \x01(\t\x12\x0c\n\x04next\x18\x07 \x01(\t\x12\x0b\n\x03pos\x18\x08 \x01(\x05\x12\r\n\x05limit\x18\t \x01(\x05\"\xa6\x01\n\x15ListAlgorithmsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\t\n\x01q\x18\x02 \x01(\t\x12\x0e\n\x06system\x18\n \x01(\t\x12\x0c\n\x04next\x18\x07 \x01(\t\x12\x0b\n\x03pos\x18\x08 \x01(\x05\x12\r\n\x05limit\x18\t \x01(\x05\x12\x36\n\x05scope\x18\x0b \x01(\x0e\x32\'.yamcs.protobuf.mdb.AlgorithmInfo.Scope\"\x91\x01\n\x13ListCommandsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\t\n\x01q\x18\x02 \x01(\t\x12\x0e\n\x06system\x18\x0b \x01(\t\x12\x0f\n\x07\x64\x65tails\x18\x04 \x01(\x08\x12\x0c\n\x04next\x18\x07 \x01(\t\x12\x0b\n\x03pos\x18\x08 \x01(\x05\x12\r\n\x05limit\x18\t \x01(\x05\x12\x12\n\nnoAbstract\x18\n \x01(\x08\"5\n\x13GetParameterRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xd8\x01\n\x15ListParametersRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\t\n\x01q\x18\x02 \x01(\t\x12\x15\n\rsearchMembers\x18\x0c \x01(\x08\x12\x0f\n\x07\x64\x65tails\x18\x04 \x01(\x08\x12\x0c\n\x04type\x18\x05 \x03(\t\x12\x32\n\x06source\x18\n \x01(\x0e\x32\".yamcs.protobuf.mdb.DataSourceType\x12\x0e\n\x06system\x18\x0b \x01(\t\x12\x0c\n\x04next\x18\x07 \x01(\t\x12\x0b\n\x03pos\x18\x08 \x01(\x05\x12\r\n\x05limit\x18\t \x01(\x05\"\x93\x01\n\x16ListParametersResponse\x12\x14\n\x0cspaceSystems\x18\x04 \x03(\t\x12\x35\n\nparameters\x18\x01 \x03(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x19\n\x11\x63ontinuationToken\x18\x02 \x01(\t\x12\x11\n\ttotalSize\x18\x03 \x01(\x05\"X\n\x19\x42\x61tchGetParametersRequest\x12\x10\n\x08instance\x18\x02 \x01(\t\x12)\n\x02id\x18\x01 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\"\xec\x01\n\x1a\x42\x61tchGetParametersResponse\x12U\n\x08response\x18\x01 \x03(\x0b\x32\x43.yamcs.protobuf.mdb.BatchGetParametersResponse.GetParameterResponse\x1aw\n\x14GetParameterResponse\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x34\n\tparameter\x18\x02 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\"\x93\x01\n\x16ListContainersResponse\x12\x14\n\x0cspaceSystems\x18\x04 \x03(\t\x12\x35\n\ncontainers\x18\x01 \x03(\x0b\x32!.yamcs.protobuf.mdb.ContainerInfo\x12\x19\n\x11\x63ontinuationToken\x18\x02 \x01(\t\x12\x11\n\ttotalSize\x18\x03 \x01(\x05\"\x8d\x01\n\x14ListCommandsResponse\x12\x14\n\x0cspaceSystems\x18\x04 \x03(\t\x12\x31\n\x08\x63ommands\x18\x01 \x03(\x0b\x32\x1f.yamcs.protobuf.mdb.CommandInfo\x12\x19\n\x11\x63ontinuationToken\x18\x02 \x01(\t\x12\x11\n\ttotalSize\x18\x03 \x01(\x05\"\x93\x01\n\x16ListAlgorithmsResponse\x12\x14\n\x0cspaceSystems\x18\x04 \x03(\t\x12\x35\n\nalgorithms\x18\x01 \x03(\x0b\x32!.yamcs.protobuf.mdb.AlgorithmInfo\x12\x19\n\x11\x63ontinuationToken\x18\x02 \x01(\t\x12\x11\n\ttotalSize\x18\x03 \x01(\x05\"5\n\x13GetAlgorithmRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"-\n\x19GetMissionDatabaseRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"4\n ExportJavaMissionDatabaseRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"\x83\x01\n\x18ListSpaceSystemsResponse\x12\x39\n\x0cspaceSystems\x18\x01 \x03(\x0b\x32#.yamcs.protobuf.mdb.SpaceSystemInfo\x12\x19\n\x11\x63ontinuationToken\x18\x02 \x01(\t\x12\x11\n\ttotalSize\x18\x03 \x01(\x05\"7\n\x15GetSpaceSystemRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"3\n\x11GetCommandRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xb8\x03\n\x0fSpaceSystemInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rqualifiedName\x18\x02 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x10 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\x30\n\x07history\x18\x0e \x03(\x0b\x32\x1f.yamcs.protobuf.mdb.HistoryInfo\x12\x30\n\x03sub\x18\x0f \x03(\x0b\x32#.yamcs.protobuf.mdb.SpaceSystemInfo\x12M\n\rancillaryData\x18\x11 \x03(\x0b\x32\x36.yamcs.protobuf.mdb.SpaceSystemInfo.AncillaryDataEntry\x1a[\n\x12\x41ncillaryDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.yamcs.protobuf.mdb.AncillaryDataInfo:\x02\x38\x01*\xa2\x01\n\x0e\x44\x61taSourceType\x12\x0f\n\x0bTELEMETERED\x10\x00\x12\x0b\n\x07\x44\x45RIVED\x10\x01\x12\x0c\n\x08\x43ONSTANT\x10\x02\x12\t\n\x05LOCAL\x10\x03\x12\n\n\x06SYSTEM\x10\x04\x12\x0b\n\x07\x43OMMAND\x10\x05\x12\x13\n\x0f\x43OMMAND_HISTORY\x10\x06\x12\r\n\tEXTERNAL1\x10\x07\x12\r\n\tEXTERNAL2\x10\x08\x12\r\n\tEXTERNAL3\x10\t*\\\n\x0e\x41larmLevelType\x12\n\n\x06NORMAL\x10\x00\x12\t\n\x05WATCH\x10\x01\x12\x0b\n\x07WARNING\x10\x02\x12\x0c\n\x08\x44ISTRESS\x10\x03\x12\x0c\n\x08\x43RITICAL\x10\x04\x12\n\n\x06SEVERE\x10\x05\x32\x93\x0f\n\x06MdbApi\x12\x83\x01\n\x12GetMissionDatabase\x12-.yamcs.protobuf.mdb.GetMissionDatabaseRequest\x1a#.yamcs.protobuf.mdb.MissionDatabase\"\x19\x8a\x92\x03\x15\n\x13/api/mdb/{instance}\x12\x8c\x01\n\x19\x45xportJavaMissionDatabase\x12\x34.yamcs.protobuf.mdb.ExportJavaMissionDatabaseRequest\x1a\x13.yamcs.api.HttpBody\"$\x8a\x92\x03 \n\x1e/api/mdb/{instance}:exportJava\x12\xa4\x01\n\x10ListSpaceSystems\x12+.yamcs.protobuf.mdb.ListSpaceSystemsRequest\x1a,.yamcs.protobuf.mdb.ListSpaceSystemsResponse\"5\x8a\x92\x03\x31\n!/api/mdb/{instance}/space-systemsR\x0cspaceSystems\x12\x91\x01\n\x0eGetSpaceSystem\x12).yamcs.protobuf.mdb.GetSpaceSystemRequest\x1a#.yamcs.protobuf.mdb.SpaceSystemInfo\"/\x8a\x92\x03+\n)/api/mdb/{instance}/space-systems/{name*}\x12\x99\x01\n\x0eListParameters\x12).yamcs.protobuf.mdb.ListParametersRequest\x1a*.yamcs.protobuf.mdb.ListParametersResponse\"0\x8a\x92\x03,\n\x1e/api/mdb/{instance}/parametersR\nparameters\x12\x88\x01\n\x0cGetParameter\x12\'.yamcs.protobuf.mdb.GetParameterRequest\x1a!.yamcs.protobuf.mdb.ParameterInfo\",\x8a\x92\x03(\n&/api/mdb/{instance}/parameters/{name*}\x12\xa5\x01\n\x12\x42\x61tchGetParameters\x12-.yamcs.protobuf.mdb.BatchGetParametersRequest\x1a..yamcs.protobuf.mdb.BatchGetParametersResponse\"0\x8a\x92\x03,\x1a\'/api/mdb/{instance}/parameters:batchGet:\x01*\x12\x99\x01\n\x0eListContainers\x12).yamcs.protobuf.mdb.ListContainersRequest\x1a*.yamcs.protobuf.mdb.ListContainersResponse\"0\x8a\x92\x03,\n\x1e/api/mdb/{instance}/containersR\ncontainers\x12\x88\x01\n\x0cGetContainer\x12\'.yamcs.protobuf.mdb.GetContainerRequest\x1a!.yamcs.protobuf.mdb.ContainerInfo\",\x8a\x92\x03(\n&/api/mdb/{instance}/containers/{name*}\x12\x8f\x01\n\x0cListCommands\x12\'.yamcs.protobuf.mdb.ListCommandsRequest\x1a(.yamcs.protobuf.mdb.ListCommandsResponse\",\x8a\x92\x03(\n\x1c/api/mdb/{instance}/commandsR\x08\x63ommands\x12\x80\x01\n\nGetCommand\x12%.yamcs.protobuf.mdb.GetCommandRequest\x1a\x1f.yamcs.protobuf.mdb.CommandInfo\"*\x8a\x92\x03&\n$/api/mdb/{instance}/commands/{name*}\x12\x99\x01\n\x0eListAlgorithms\x12).yamcs.protobuf.mdb.ListAlgorithmsRequest\x1a*.yamcs.protobuf.mdb.ListAlgorithmsResponse\"0\x8a\x92\x03,\n\x1e/api/mdb/{instance}/algorithmsR\nalgorithms\x12\x88\x01\n\x0cGetAlgorithm\x12\'.yamcs.protobuf.mdb.GetAlgorithmRequest\x1a!.yamcs.protobuf.mdb.AlgorithmInfo\",\x8a\x92\x03(\n&/api/mdb/{instance}/algorithms/{name*}\x1a\x07\x82\x80\x01\x03MDBB\x14\n\x12org.yamcs.protobuf')
+  serialized_pb=_b('\n\x1cyamcs/protobuf/mdb/mdb.proto\x12\x12yamcs.protobuf.mdb\x1a\x1byamcs/api/annotations.proto\x1a\x18yamcs/api/httpbody.proto\x1a\x1ayamcs/protobuf/yamcs.proto\"\xf8\x01\n\x0fMissionDatabase\x12\x12\n\nconfigName\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x38\n\x0bspaceSystem\x18\x04 \x03(\x0b\x32#.yamcs.protobuf.mdb.SpaceSystemInfo\x12\x16\n\x0eparameterCount\x18\x06 \x01(\x05\x12\x16\n\x0e\x63ontainerCount\x18\x07 \x01(\x05\x12\x14\n\x0c\x63ommandCount\x18\x08 \x01(\x05\x12\x16\n\x0e\x61lgorithmCount\x18\t \x01(\x05\x12\x1a\n\x12parameterTypeCount\x18\n \x01(\x05\"M\n\x0bHistoryInfo\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x04 \x01(\t\"\x18\n\x08UnitInfo\x12\x0c\n\x04unit\x18\x01 \x01(\t\"\x97\x01\n\nAlarmRange\x12\x31\n\x05level\x18\x01 \x01(\x0e\x32\".yamcs.protobuf.mdb.AlarmLevelType\x12\x14\n\x0cminInclusive\x18\x02 \x01(\x01\x12\x14\n\x0cmaxInclusive\x18\x03 \x01(\x01\x12\x14\n\x0cminExclusive\x18\x04 \x01(\x01\x12\x14\n\x0cmaxExclusive\x18\x05 \x01(\x01\"T\n\x10\x45numerationAlarm\x12\x31\n\x05level\x18\x01 \x01(\x0e\x32\".yamcs.protobuf.mdb.AlarmLevelType\x12\r\n\x05label\x18\x03 \x01(\t\"\x9c\x01\n\tAlarmInfo\x12\x15\n\rminViolations\x18\x01 \x01(\x05\x12\x38\n\x10staticAlarmRange\x18\x02 \x03(\x0b\x32\x1e.yamcs.protobuf.mdb.AlarmRange\x12>\n\x10\x65numerationAlarm\x18\x03 \x03(\x0b\x32$.yamcs.protobuf.mdb.EnumerationAlarm\"\x89\x01\n\x10\x43ontextAlarmInfo\x12\x36\n\ncomparison\x18\x01 \x03(\x0b\x32\".yamcs.protobuf.mdb.ComparisonInfo\x12,\n\x05\x61larm\x18\x02 \x01(\x0b\x32\x1d.yamcs.protobuf.mdb.AlarmInfo\x12\x0f\n\x07\x63ontext\x18\x03 \x01(\t\"\xd1\x02\n\x10\x44\x61taEncodingInfo\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32).yamcs.protobuf.mdb.DataEncodingInfo.Type\x12\x14\n\x0clittleEndian\x18\x02 \x01(\x08\x12\x12\n\nsizeInBits\x18\x03 \x01(\x05\x12\x10\n\x08\x65ncoding\x18\x04 \x01(\t\x12=\n\x11\x64\x65\x66\x61ultCalibrator\x18\x06 \x01(\x0b\x32\".yamcs.protobuf.mdb.CalibratorInfo\x12\x44\n\x11\x63ontextCalibrator\x18\x07 \x03(\x0b\x32).yamcs.protobuf.mdb.ContextCalibratorInfo\"C\n\x04Type\x12\n\n\x06\x42INARY\x10\x00\x12\x0b\n\x07\x42OOLEAN\x10\x01\x12\t\n\x05\x46LOAT\x10\x02\x12\x0b\n\x07INTEGER\x10\x03\x12\n\n\x06STRING\x10\x04\"\x98\x01\n\x15\x43ontextCalibratorInfo\x12\x36\n\ncomparison\x18\x01 \x03(\x0b\x32\".yamcs.protobuf.mdb.ComparisonInfo\x12\x36\n\ncalibrator\x18\x02 \x01(\x0b\x32\".yamcs.protobuf.mdb.CalibratorInfo\x12\x0f\n\x07\x63ontext\x18\x03 \x01(\t\"\xf8\x02\n\x0e\x43\x61libratorInfo\x12J\n\x14polynomialCalibrator\x18\x02 \x01(\x0b\x32,.yamcs.protobuf.mdb.PolynomialCalibratorInfo\x12\x42\n\x10splineCalibrator\x18\x03 \x01(\x0b\x32(.yamcs.protobuf.mdb.SplineCalibratorInfo\x12R\n\x18javaExpressionCalibrator\x18\x04 \x01(\x0b\x32\x30.yamcs.protobuf.mdb.JavaExpressionCalibratorInfo\x12\x35\n\x04type\x18\x05 \x01(\x0e\x32\'.yamcs.protobuf.mdb.CalibratorInfo.Type\"K\n\x04Type\x12\x0e\n\nPOLYNOMIAL\x10\x00\x12\n\n\x06SPLINE\x10\x01\x12\x12\n\x0eMATH_OPERATION\x10\x02\x12\x13\n\x0fJAVA_EXPRESSION\x10\x03\"/\n\x18PolynomialCalibratorInfo\x12\x13\n\x0b\x63oefficient\x18\x01 \x03(\x01\"\x93\x01\n\x14SplineCalibratorInfo\x12G\n\x05point\x18\x01 \x03(\x0b\x32\x38.yamcs.protobuf.mdb.SplineCalibratorInfo.SplinePointInfo\x1a\x32\n\x0fSplinePointInfo\x12\x0b\n\x03raw\x18\x01 \x01(\x01\x12\x12\n\ncalibrated\x18\x02 \x01(\x01\"/\n\x1cJavaExpressionCalibratorInfo\x12\x0f\n\x07\x66ormula\x18\x01 \x01(\t\">\n\tEnumValue\x12\r\n\x05value\x18\x01 \x01(\x03\x12\r\n\x05label\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\"\xd2\x05\n\x11ParameterTypeInfo\x12\x0f\n\x07\x65ngType\x18\x01 \x01(\t\x12:\n\x0c\x64\x61taEncoding\x18\x02 \x01(\x0b\x32$.yamcs.protobuf.mdb.DataEncodingInfo\x12-\n\x07unitSet\x18\x03 \x03(\x0b\x32\x1c.yamcs.protobuf.mdb.UnitInfo\x12\x33\n\x0c\x64\x65\x66\x61ultAlarm\x18\x04 \x01(\x0b\x32\x1d.yamcs.protobuf.mdb.AlarmInfo\x12\x30\n\tenumValue\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.mdb.EnumValue\x12>\n\x10\x61\x62soluteTimeInfo\x18\x06 \x01(\x0b\x32$.yamcs.protobuf.mdb.AbsoluteTimeInfo\x12:\n\x0c\x63ontextAlarm\x18\x07 \x03(\x0b\x32$.yamcs.protobuf.mdb.ContextAlarmInfo\x12.\n\x06member\x18\x08 \x03(\x0b\x32\x1e.yamcs.protobuf.mdb.MemberInfo\x12\x30\n\tarrayInfo\x18\t \x01(\x0b\x32\x1d.yamcs.protobuf.mdb.ArrayInfo\x12O\n\rancillaryData\x18\n \x03(\x0b\x32\x38.yamcs.protobuf.mdb.ParameterTypeInfo.AncillaryDataEntry\x12>\n\x0cnumberFormat\x18\x0b \x01(\x0b\x32(.yamcs.protobuf.mdb.NumberFormatTypeInfo\x12\x0e\n\x06signed\x18\x0c \x01(\x08\x1a[\n\x12\x41ncillaryDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.yamcs.protobuf.mdb.AncillaryDataInfo:\x02\x38\x01\"\xb5\x02\n\x14NumberFormatTypeInfo\x12\x12\n\nnumberBase\x18\x01 \x01(\t\x12\x1d\n\x15minimumFractionDigits\x18\x02 \x01(\x05\x12\x1d\n\x15maximumFractionDigits\x18\x03 \x01(\x05\x12\x1c\n\x14minimumIntegerDigits\x18\x04 \x01(\x05\x12\x1c\n\x14maximumIntegerDigits\x18\x05 \x01(\x05\x12\x16\n\x0enegativeSuffix\x18\x06 \x01(\t\x12\x16\n\x0epositiveSuffix\x18\x07 \x01(\t\x12\x16\n\x0enegativePrefix\x18\x08 \x01(\t\x12\x16\n\x0epositivePrefix\x18\t \x01(\t\x12\x1d\n\x15showThousandsGrouping\x18\n \x01(\x08\x12\x10\n\x08notation\x18\x0b \x01(\t\"5\n\x13GetContainerRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x8d\x01\n\x10\x41\x62soluteTimeInfo\x12\x14\n\x0cinitialValue\x18\x01 \x01(\t\x12\r\n\x05scale\x18\x02 \x01(\x01\x12\x0e\n\x06offset\x18\x03 \x01(\x01\x12\x35\n\noffsetFrom\x18\x04 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\r\n\x05\x65poch\x18\x05 \x01(\t\"\xb0\x01\n\nMemberInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x33\n\x04type\x18\x06 \x01(\x0b\x32%.yamcs.protobuf.mdb.ParameterTypeInfo\"\xcd\x01\n\x12\x41rgumentMemberInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x32\n\x04type\x18\x06 \x01(\x0b\x32$.yamcs.protobuf.mdb.ArgumentTypeInfo\x12\x14\n\x0cinitialValue\x18\x07 \x01(\t\"\x84\x01\n\x16ParameterDimensionInfo\x12\x12\n\nfixedValue\x18\x01 \x01(\x03\x12\x34\n\tparameter\x18\x02 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\r\n\x05slope\x18\x03 \x01(\x03\x12\x11\n\tintercept\x18\x04 \x01(\x03\"\x80\x01\n\tArrayInfo\x12\x33\n\x04type\x18\x01 \x01(\x0b\x32%.yamcs.protobuf.mdb.ParameterTypeInfo\x12>\n\ndimensions\x18\x03 \x03(\x0b\x32*.yamcs.protobuf.mdb.ParameterDimensionInfo\"x\n\nUsedByInfo\x12\x34\n\talgorithm\x18\x01 \x03(\x0b\x32!.yamcs.protobuf.mdb.AlgorithmInfo\x12\x34\n\tcontainer\x18\x02 \x03(\x0b\x32!.yamcs.protobuf.mdb.ContainerInfo\"\xea\x03\n\rParameterInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rqualifiedName\x18\x02 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x33\n\x04type\x18\x06 \x01(\x0b\x32%.yamcs.protobuf.mdb.ParameterTypeInfo\x12\x36\n\ndataSource\x18\x07 \x01(\x0e\x32\".yamcs.protobuf.mdb.DataSourceType\x12.\n\x06usedBy\x18\x08 \x01(\x0b\x32\x1e.yamcs.protobuf.mdb.UsedByInfo\x12K\n\rancillaryData\x18\t \x03(\x0b\x32\x34.yamcs.protobuf.mdb.ParameterInfo.AncillaryDataEntry\x12\x0c\n\x04path\x18\n \x03(\t\x1a[\n\x12\x41ncillaryDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.yamcs.protobuf.mdb.AncillaryDataInfo:\x02\x38\x01\"B\n\x11\x41ncillaryDataInfo\x12\r\n\x05value\x18\x01 \x01(\t\x12\x10\n\x08mimeType\x18\x02 \x01(\t\x12\x0c\n\x04href\x18\x03 \x01(\t\"\x9f\x04\n\x10\x41rgumentTypeInfo\x12\x0f\n\x07\x65ngType\x18\x01 \x01(\t\x12:\n\x0c\x64\x61taEncoding\x18\x02 \x01(\x0b\x32$.yamcs.protobuf.mdb.DataEncodingInfo\x12-\n\x07unitSet\x18\x03 \x03(\x0b\x32\x1c.yamcs.protobuf.mdb.UnitInfo\x12\x30\n\tenumValue\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.mdb.EnumValue\x12\x10\n\x08rangeMin\x18\x06 \x01(\x01\x12\x10\n\x08rangeMax\x18\x07 \x01(\x01\x12\x36\n\x06member\x18\x08 \x03(\x0b\x32&.yamcs.protobuf.mdb.ArgumentMemberInfo\x12\x17\n\x0fzeroStringValue\x18\t \x01(\t\x12\x16\n\x0eoneStringValue\x18\n \x01(\t\x12\x10\n\x08minChars\x18\x0b \x01(\x05\x12\x10\n\x08maxChars\x18\x0c \x01(\x05\x12\x0e\n\x06signed\x18\r \x01(\x08\x12\x10\n\x08minBytes\x18\x0e \x01(\x05\x12\x10\n\x08maxBytes\x18\x0f \x01(\x05\x12=\n\ndimensions\x18\x10 \x03(\x0b\x32).yamcs.protobuf.mdb.ArgumentDimensionInfo\x12\x39\n\x0b\x65lementType\x18\x11 \x01(\x0b\x32$.yamcs.protobuf.mdb.ArgumentTypeInfo\"\x95\x01\n\x15\x41rgumentDimensionInfo\x12\x12\n\nfixedValue\x18\x01 \x01(\x03\x12\x34\n\tparameter\x18\x02 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x10\n\x08\x61rgument\x18\x03 \x01(\t\x12\r\n\x05slope\x18\x04 \x01(\x03\x12\x11\n\tintercept\x18\x05 \x01(\x03\"{\n\x0c\x41rgumentInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x14\n\x0cinitialValue\x18\x04 \x01(\t\x12\x32\n\x04type\x18\x06 \x01(\x0b\x32$.yamcs.protobuf.mdb.ArgumentTypeInfo\"5\n\x16\x41rgumentAssignmentInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xe5\x01\n\x10SignificanceInfo\x12T\n\x10\x63onsequenceLevel\x18\x01 \x01(\x0e\x32:.yamcs.protobuf.mdb.SignificanceInfo.SignificanceLevelType\x12\x18\n\x10reasonForWarning\x18\x02 \x01(\t\"a\n\x15SignificanceLevelType\x12\x08\n\x04NONE\x10\x01\x12\t\n\x05WATCH\x10\x02\x12\x0b\n\x07WARNING\x10\x03\x12\x0c\n\x08\x44ISTRESS\x10\x04\x12\x0c\n\x08\x43RITICAL\x10\x05\x12\n\n\x06SEVERE\x10\x06\"\xdd\x02\n\x0e\x43omparisonInfo\x12\x34\n\tparameter\x18\x01 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x41\n\x08operator\x18\x02 \x01(\x0e\x32/.yamcs.protobuf.mdb.ComparisonInfo.OperatorType\x12\r\n\x05value\x18\x03 \x01(\t\x12\x32\n\x08\x61rgument\x18\x04 \x01(\x0b\x32 .yamcs.protobuf.mdb.ArgumentInfo\"\x8e\x01\n\x0cOperatorType\x12\x0c\n\x08\x45QUAL_TO\x10\x01\x12\x10\n\x0cNOT_EQUAL_TO\x10\x02\x12\x10\n\x0cGREATER_THAN\x10\x03\x12\x1c\n\x18GREATER_THAN_OR_EQUAL_TO\x10\x04\x12\x10\n\x0cSMALLER_THAN\x10\x05\x12\x1c\n\x18SMALLER_THAN_OR_EQUAL_TO\x10\x06\"A\n\x1aTransmissionConstraintInfo\x12\x12\n\nexpression\x18\x03 \x01(\t\x12\x0f\n\x07timeout\x18\x02 \x01(\x03\"\xf7\x05\n\x0b\x43ommandInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rqualifiedName\x18\x02 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x34\n\x0b\x62\x61seCommand\x18\x06 \x01(\x0b\x32\x1f.yamcs.protobuf.mdb.CommandInfo\x12\x10\n\x08\x61\x62stract\x18\x07 \x01(\x08\x12\x32\n\x08\x61rgument\x18\x08 \x03(\x0b\x32 .yamcs.protobuf.mdb.ArgumentInfo\x12\x46\n\x12\x61rgumentAssignment\x18\t \x03(\x0b\x32*.yamcs.protobuf.mdb.ArgumentAssignmentInfo\x12:\n\x0csignificance\x18\n \x01(\x0b\x32$.yamcs.protobuf.mdb.SignificanceInfo\x12\x42\n\nconstraint\x18\x0b \x03(\x0b\x32..yamcs.protobuf.mdb.TransmissionConstraintInfo\x12\x42\n\x10\x63ommandContainer\x18\r \x01(\x0b\x32(.yamcs.protobuf.mdb.CommandContainerInfo\x12\x32\n\x08verifier\x18\x0e \x03(\x0b\x32 .yamcs.protobuf.mdb.VerifierInfo\x12I\n\rancillaryData\x18\x0f \x03(\x0b\x32\x32.yamcs.protobuf.mdb.CommandInfo.AncillaryDataEntry\x1a[\n\x12\x41ncillaryDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.yamcs.protobuf.mdb.AncillaryDataInfo:\x02\x38\x01\"\xd1\x03\n\x0cVerifierInfo\x12\r\n\x05stage\x18\x01 \x01(\t\x12\x34\n\tcontainer\x18\x02 \x01(\x0b\x32!.yamcs.protobuf.mdb.ContainerInfo\x12\x34\n\talgorithm\x18\x03 \x01(\x0b\x32!.yamcs.protobuf.mdb.AlgorithmInfo\x12I\n\tonSuccess\x18\x04 \x01(\x0e\x32\x36.yamcs.protobuf.mdb.VerifierInfo.TerminationActionType\x12\x46\n\x06onFail\x18\x05 \x01(\x0e\x32\x36.yamcs.protobuf.mdb.VerifierInfo.TerminationActionType\x12I\n\tonTimeout\x18\x06 \x01(\x0e\x32\x36.yamcs.protobuf.mdb.VerifierInfo.TerminationActionType\x12\x38\n\x0b\x63heckWindow\x18\x07 \x01(\x0b\x32#.yamcs.protobuf.mdb.CheckWindowInfo\".\n\x15TerminationActionType\x12\x0b\n\x07SUCCESS\x10\x01\x12\x08\n\x04\x46\x41IL\x10\x02\"^\n\x0f\x43heckWindowInfo\x12\x1b\n\x13timeToStartChecking\x18\x01 \x01(\x03\x12\x1a\n\x12timeToStopChecking\x18\x02 \x01(\x03\x12\x12\n\nrelativeTo\x18\x03 \x01(\t\"n\n\nRepeatInfo\x12\x12\n\nfixedCount\x18\x01 \x01(\x03\x12\x37\n\x0c\x64ynamicCount\x18\x02 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x13\n\x0b\x62itsBetween\x18\x03 \x01(\x05\"\xcd\x03\n\x11SequenceEntryInfo\x12\x16\n\x0elocationInBits\x18\x01 \x01(\x05\x12V\n\x11referenceLocation\x18\x02 \x01(\x0e\x32;.yamcs.protobuf.mdb.SequenceEntryInfo.ReferenceLocationType\x12\x34\n\tcontainer\x18\x03 \x01(\x0b\x32!.yamcs.protobuf.mdb.ContainerInfo\x12\x34\n\tparameter\x18\x04 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x32\n\x08\x61rgument\x18\x06 \x01(\x0b\x32 .yamcs.protobuf.mdb.ArgumentInfo\x12\x36\n\nfixedValue\x18\x07 \x01(\x0b\x32\".yamcs.protobuf.mdb.FixedValueInfo\x12.\n\x06repeat\x18\x05 \x01(\x0b\x32\x1e.yamcs.protobuf.mdb.RepeatInfo\"@\n\x15ReferenceLocationType\x12\x13\n\x0f\x43ONTAINER_START\x10\x01\x12\x12\n\x0ePREVIOUS_ENTRY\x10\x02\"D\n\x0e\x46ixedValueInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08hexValue\x18\x02 \x01(\t\x12\x12\n\nsizeInBits\x18\x03 \x01(\x05\"\xa7\x02\n\x14\x43ommandContainerInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rqualifiedName\x18\x02 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x12\n\nsizeInBits\x18\x06 \x01(\x05\x12?\n\rbaseContainer\x18\x07 \x01(\x0b\x32(.yamcs.protobuf.mdb.CommandContainerInfo\x12\x34\n\x05\x65ntry\x18\x08 \x03(\x0b\x32%.yamcs.protobuf.mdb.SequenceEntryInfo\"\xc9\x04\n\rContainerInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rqualifiedName\x18\x02 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x13\n\x0bmaxInterval\x18\x06 \x01(\x03\x12\x12\n\nsizeInBits\x18\x07 \x01(\x05\x12\x38\n\rbaseContainer\x18\x08 \x01(\x0b\x32!.yamcs.protobuf.mdb.ContainerInfo\x12?\n\x13restrictionCriteria\x18\t \x03(\x0b\x32\".yamcs.protobuf.mdb.ComparisonInfo\x12\x34\n\x05\x65ntry\x18\n \x03(\x0b\x32%.yamcs.protobuf.mdb.SequenceEntryInfo\x12.\n\x06usedBy\x18\x0b \x01(\x0b\x32\x1e.yamcs.protobuf.mdb.UsedByInfo\x12K\n\rancillaryData\x18\x0c \x03(\x0b\x32\x34.yamcs.protobuf.mdb.ContainerInfo.AncillaryDataEntry\x1a[\n\x12\x41ncillaryDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.yamcs.protobuf.mdb.AncillaryDataInfo:\x02\x38\x01\"\xbf\x01\n\x12InputParameterInfo\x12\x34\n\tparameter\x18\x01 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x11\n\tinputName\x18\x02 \x01(\t\x12\x19\n\x11parameterInstance\x18\x03 \x01(\x05\x12\x11\n\tmandatory\x18\x04 \x01(\x08\x12\x32\n\x08\x61rgument\x18\x05 \x01(\x0b\x32 .yamcs.protobuf.mdb.ArgumentInfo\"_\n\x13OutputParameterInfo\x12\x34\n\tparameter\x18\x01 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x12\n\noutputName\x18\x02 \x01(\t\"\x87\x02\n\x0bMathElement\x12\x32\n\x04type\x18\x01 \x01(\x0e\x32$.yamcs.protobuf.mdb.MathElement.Type\x12\x10\n\x08operator\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\x12\x34\n\tparameter\x18\x04 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x19\n\x11parameterInstance\x18\x05 \x01(\x05\"R\n\x04Type\x12\x11\n\rVALUE_OPERAND\x10\x01\x12\x1a\n\x16THIS_PARAMETER_OPERAND\x10\x02\x12\x0c\n\x08OPERATOR\x10\x03\x12\r\n\tPARAMETER\x10\x04\"\x99\x05\n\rAlgorithmInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rqualifiedName\x18\x02 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x05 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x36\n\x05scope\x18\x06 \x01(\x0e\x32\'.yamcs.protobuf.mdb.AlgorithmInfo.Scope\x12\x34\n\x04type\x18\r \x01(\x0e\x32&.yamcs.protobuf.mdb.AlgorithmInfo.Type\x12\x10\n\x08language\x18\x07 \x01(\t\x12\x0c\n\x04text\x18\x08 \x01(\t\x12>\n\x0einputParameter\x18\t \x03(\x0b\x32&.yamcs.protobuf.mdb.InputParameterInfo\x12@\n\x0foutputParameter\x18\n \x03(\x0b\x32\'.yamcs.protobuf.mdb.OutputParameterInfo\x12<\n\x11onParameterUpdate\x18\x0b \x03(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x16\n\x0eonPeriodicRate\x18\x0c \x03(\x03\x12\x35\n\x0cmathElements\x18\x0e \x03(\x0b\x32\x1f.yamcs.protobuf.mdb.MathElement\"\x1c\n\x04Type\x12\n\n\x06\x43USTOM\x10\x01\x12\x08\n\x04MATH\x10\x02\"G\n\x05Scope\x12\n\n\x06GLOBAL\x10\x00\x12\x18\n\x14\x43OMMAND_VERIFICATION\x10\x01\x12\x18\n\x14\x43ONTAINER_PROCESSING\x10\x02\"`\n\x17ListSpaceSystemsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\t\n\x01q\x18\x02 \x01(\t\x12\x0c\n\x04next\x18\x07 \x01(\t\x12\x0b\n\x03pos\x18\x08 \x01(\x05\x12\r\n\x05limit\x18\t \x01(\x05\"n\n\x15ListContainersRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\t\n\x01q\x18\x02 \x01(\t\x12\x0e\n\x06system\x18\n \x01(\t\x12\x0c\n\x04next\x18\x07 \x01(\t\x12\x0b\n\x03pos\x18\x08 \x01(\x05\x12\r\n\x05limit\x18\t \x01(\x05\"\xa6\x01\n\x15ListAlgorithmsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\t\n\x01q\x18\x02 \x01(\t\x12\x0e\n\x06system\x18\n \x01(\t\x12\x0c\n\x04next\x18\x07 \x01(\t\x12\x0b\n\x03pos\x18\x08 \x01(\x05\x12\r\n\x05limit\x18\t \x01(\x05\x12\x36\n\x05scope\x18\x0b \x01(\x0e\x32\'.yamcs.protobuf.mdb.AlgorithmInfo.Scope\"\x91\x01\n\x13ListCommandsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\t\n\x01q\x18\x02 \x01(\t\x12\x0e\n\x06system\x18\x0b \x01(\t\x12\x0f\n\x07\x64\x65tails\x18\x04 \x01(\x08\x12\x0c\n\x04next\x18\x07 \x01(\t\x12\x0b\n\x03pos\x18\x08 \x01(\x05\x12\r\n\x05limit\x18\t \x01(\x05\x12\x12\n\nnoAbstract\x18\n \x01(\x08\"5\n\x13GetParameterRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xd8\x01\n\x15ListParametersRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\t\n\x01q\x18\x02 \x01(\t\x12\x15\n\rsearchMembers\x18\x0c \x01(\x08\x12\x0f\n\x07\x64\x65tails\x18\x04 \x01(\x08\x12\x0c\n\x04type\x18\x05 \x03(\t\x12\x32\n\x06source\x18\n \x01(\x0e\x32\".yamcs.protobuf.mdb.DataSourceType\x12\x0e\n\x06system\x18\x0b \x01(\t\x12\x0c\n\x04next\x18\x07 \x01(\t\x12\x0b\n\x03pos\x18\x08 \x01(\x05\x12\r\n\x05limit\x18\t \x01(\x05\"\x93\x01\n\x16ListParametersResponse\x12\x14\n\x0cspaceSystems\x18\x04 \x03(\t\x12\x35\n\nparameters\x18\x01 \x03(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\x12\x19\n\x11\x63ontinuationToken\x18\x02 \x01(\t\x12\x11\n\ttotalSize\x18\x03 \x01(\x05\"X\n\x19\x42\x61tchGetParametersRequest\x12\x10\n\x08instance\x18\x02 \x01(\t\x12)\n\x02id\x18\x01 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\"\xec\x01\n\x1a\x42\x61tchGetParametersResponse\x12U\n\x08response\x18\x01 \x03(\x0b\x32\x43.yamcs.protobuf.mdb.BatchGetParametersResponse.GetParameterResponse\x1aw\n\x14GetParameterResponse\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x34\n\tparameter\x18\x02 \x01(\x0b\x32!.yamcs.protobuf.mdb.ParameterInfo\"\x93\x01\n\x16ListContainersResponse\x12\x14\n\x0cspaceSystems\x18\x04 \x03(\t\x12\x35\n\ncontainers\x18\x01 \x03(\x0b\x32!.yamcs.protobuf.mdb.ContainerInfo\x12\x19\n\x11\x63ontinuationToken\x18\x02 \x01(\t\x12\x11\n\ttotalSize\x18\x03 \x01(\x05\"\x8d\x01\n\x14ListCommandsResponse\x12\x14\n\x0cspaceSystems\x18\x04 \x03(\t\x12\x31\n\x08\x63ommands\x18\x01 \x03(\x0b\x32\x1f.yamcs.protobuf.mdb.CommandInfo\x12\x19\n\x11\x63ontinuationToken\x18\x02 \x01(\t\x12\x11\n\ttotalSize\x18\x03 \x01(\x05\"\x93\x01\n\x16ListAlgorithmsResponse\x12\x14\n\x0cspaceSystems\x18\x04 \x03(\t\x12\x35\n\nalgorithms\x18\x01 \x03(\x0b\x32!.yamcs.protobuf.mdb.AlgorithmInfo\x12\x19\n\x11\x63ontinuationToken\x18\x02 \x01(\t\x12\x11\n\ttotalSize\x18\x03 \x01(\x05\"5\n\x13GetAlgorithmRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"-\n\x19GetMissionDatabaseRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"4\n ExportJavaMissionDatabaseRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"\x83\x01\n\x18ListSpaceSystemsResponse\x12\x39\n\x0cspaceSystems\x18\x01 \x03(\x0b\x32#.yamcs.protobuf.mdb.SpaceSystemInfo\x12\x19\n\x11\x63ontinuationToken\x18\x02 \x01(\t\x12\x11\n\ttotalSize\x18\x03 \x01(\x05\"7\n\x15GetSpaceSystemRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"3\n\x11\x45xportXtceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"3\n\x11GetCommandRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xb8\x03\n\x0fSpaceSystemInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rqualifiedName\x18\x02 \x01(\t\x12\x18\n\x10shortDescription\x18\x03 \x01(\t\x12\x17\n\x0flongDescription\x18\x04 \x01(\t\x12,\n\x05\x61lias\x18\x10 \x03(\x0b\x32\x1d.yamcs.protobuf.NamedObjectId\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\x30\n\x07history\x18\x0e \x03(\x0b\x32\x1f.yamcs.protobuf.mdb.HistoryInfo\x12\x30\n\x03sub\x18\x0f \x03(\x0b\x32#.yamcs.protobuf.mdb.SpaceSystemInfo\x12M\n\rancillaryData\x18\x11 \x03(\x0b\x32\x36.yamcs.protobuf.mdb.SpaceSystemInfo.AncillaryDataEntry\x1a[\n\x12\x41ncillaryDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.yamcs.protobuf.mdb.AncillaryDataInfo:\x02\x38\x01*\xa2\x01\n\x0e\x44\x61taSourceType\x12\x0f\n\x0bTELEMETERED\x10\x00\x12\x0b\n\x07\x44\x45RIVED\x10\x01\x12\x0c\n\x08\x43ONSTANT\x10\x02\x12\t\n\x05LOCAL\x10\x03\x12\n\n\x06SYSTEM\x10\x04\x12\x0b\n\x07\x43OMMAND\x10\x05\x12\x13\n\x0f\x43OMMAND_HISTORY\x10\x06\x12\r\n\tEXTERNAL1\x10\x07\x12\r\n\tEXTERNAL2\x10\x08\x12\r\n\tEXTERNAL3\x10\t*\\\n\x0e\x41larmLevelType\x12\n\n\x06NORMAL\x10\x00\x12\t\n\x05WATCH\x10\x01\x12\x0b\n\x07WARNING\x10\x02\x12\x0c\n\x08\x44ISTRESS\x10\x03\x12\x0c\n\x08\x43RITICAL\x10\x04\x12\n\n\x06SEVERE\x10\x05\x32\x9a\x10\n\x06MdbApi\x12\x83\x01\n\x12GetMissionDatabase\x12-.yamcs.protobuf.mdb.GetMissionDatabaseRequest\x1a#.yamcs.protobuf.mdb.MissionDatabase\"\x19\x8a\x92\x03\x15\n\x13/api/mdb/{instance}\x12\x8c\x01\n\x19\x45xportJavaMissionDatabase\x12\x34.yamcs.protobuf.mdb.ExportJavaMissionDatabaseRequest\x1a\x13.yamcs.api.HttpBody\"$\x8a\x92\x03 \n\x1e/api/mdb/{instance}:exportJava\x12\xa4\x01\n\x10ListSpaceSystems\x12+.yamcs.protobuf.mdb.ListSpaceSystemsRequest\x1a,.yamcs.protobuf.mdb.ListSpaceSystemsResponse\"5\x8a\x92\x03\x31\n!/api/mdb/{instance}/space-systemsR\x0cspaceSystems\x12\x91\x01\n\x0eGetSpaceSystem\x12).yamcs.protobuf.mdb.GetSpaceSystemRequest\x1a#.yamcs.protobuf.mdb.SpaceSystemInfo\"/\x8a\x92\x03+\n)/api/mdb/{instance}/space-systems/{name*}\x12\x84\x01\n\nExportXtce\x12%.yamcs.protobuf.mdb.ExportXtceRequest\x1a\x13.yamcs.api.HttpBody\":\x8a\x92\x03\x36\n4/api/mdb/{instance}/space-systems/{name*}:exportXTCE\x12\x99\x01\n\x0eListParameters\x12).yamcs.protobuf.mdb.ListParametersRequest\x1a*.yamcs.protobuf.mdb.ListParametersResponse\"0\x8a\x92\x03,\n\x1e/api/mdb/{instance}/parametersR\nparameters\x12\x88\x01\n\x0cGetParameter\x12\'.yamcs.protobuf.mdb.GetParameterRequest\x1a!.yamcs.protobuf.mdb.ParameterInfo\",\x8a\x92\x03(\n&/api/mdb/{instance}/parameters/{name*}\x12\xa5\x01\n\x12\x42\x61tchGetParameters\x12-.yamcs.protobuf.mdb.BatchGetParametersRequest\x1a..yamcs.protobuf.mdb.BatchGetParametersResponse\"0\x8a\x92\x03,\x1a\'/api/mdb/{instance}/parameters:batchGet:\x01*\x12\x99\x01\n\x0eListContainers\x12).yamcs.protobuf.mdb.ListContainersRequest\x1a*.yamcs.protobuf.mdb.ListContainersResponse\"0\x8a\x92\x03,\n\x1e/api/mdb/{instance}/containersR\ncontainers\x12\x88\x01\n\x0cGetContainer\x12\'.yamcs.protobuf.mdb.GetContainerRequest\x1a!.yamcs.protobuf.mdb.ContainerInfo\",\x8a\x92\x03(\n&/api/mdb/{instance}/containers/{name*}\x12\x8f\x01\n\x0cListCommands\x12\'.yamcs.protobuf.mdb.ListCommandsRequest\x1a(.yamcs.protobuf.mdb.ListCommandsResponse\",\x8a\x92\x03(\n\x1c/api/mdb/{instance}/commandsR\x08\x63ommands\x12\x80\x01\n\nGetCommand\x12%.yamcs.protobuf.mdb.GetCommandRequest\x1a\x1f.yamcs.protobuf.mdb.CommandInfo\"*\x8a\x92\x03&\n$/api/mdb/{instance}/commands/{name*}\x12\x99\x01\n\x0eListAlgorithms\x12).yamcs.protobuf.mdb.ListAlgorithmsRequest\x1a*.yamcs.protobuf.mdb.ListAlgorithmsResponse\"0\x8a\x92\x03,\n\x1e/api/mdb/{instance}/algorithmsR\nalgorithms\x12\x88\x01\n\x0cGetAlgorithm\x12\'.yamcs.protobuf.mdb.GetAlgorithmRequest\x1a!.yamcs.protobuf.mdb.AlgorithmInfo\",\x8a\x92\x03(\n&/api/mdb/{instance}/algorithms/{name*}\x1a\x07\x82\x80\x01\x03MDBB\x14\n\x12org.yamcs.protobuf')
   ,
   dependencies=[yamcs_dot_api_dot_annotations__pb2.DESCRIPTOR,yamcs_dot_api_dot_httpbody__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_yamcs__pb2.DESCRIPTOR,])
 
 _DATASOURCETYPE = _descriptor.EnumDescriptor(
   name='DataSourceType',
   full_name='yamcs.protobuf.mdb.DataSourceType',
   filename=None,
@@ -73,16 +73,16 @@
     _descriptor.EnumValueDescriptor(
       name='EXTERNAL3', index=9, number=9,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=12563,
-  serialized_end=12725,
+  serialized_start=13021,
+  serialized_end=13183,
 )
 _sym_db.RegisterEnumDescriptor(_DATASOURCETYPE)
 
 DataSourceType = enum_type_wrapper.EnumTypeWrapper(_DATASOURCETYPE)
 _ALARMLEVELTYPE = _descriptor.EnumDescriptor(
   name='AlarmLevelType',
   full_name='yamcs.protobuf.mdb.AlarmLevelType',
@@ -112,16 +112,16 @@
     _descriptor.EnumValueDescriptor(
       name='SEVERE', index=5, number=5,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=12727,
-  serialized_end=12819,
+  serialized_start=13185,
+  serialized_end=13277,
 )
 _sym_db.RegisterEnumDescriptor(_ALARMLEVELTYPE)
 
 AlarmLevelType = enum_type_wrapper.EnumTypeWrapper(_ALARMLEVELTYPE)
 TELEMETERED = 0
 DERIVED = 1
 CONSTANT = 2
@@ -320,14 +320,66 @@
   containing_type=None,
   serialized_options=None,
   serialized_start=8153,
   serialized_end=8217,
 )
 _sym_db.RegisterEnumDescriptor(_SEQUENCEENTRYINFO_REFERENCELOCATIONTYPE)
 
+_MATHELEMENT_TYPE = _descriptor.EnumDescriptor(
+  name='Type',
+  full_name='yamcs.protobuf.mdb.MathElement.Type',
+  filename=None,
+  file=DESCRIPTOR,
+  values=[
+    _descriptor.EnumValueDescriptor(
+      name='VALUE_OPERAND', index=0, number=1,
+      serialized_options=None,
+      type=None),
+    _descriptor.EnumValueDescriptor(
+      name='THIS_PARAMETER_OPERAND', index=1, number=2,
+      serialized_options=None,
+      type=None),
+    _descriptor.EnumValueDescriptor(
+      name='OPERATOR', index=2, number=3,
+      serialized_options=None,
+      type=None),
+    _descriptor.EnumValueDescriptor(
+      name='PARAMETER', index=3, number=4,
+      serialized_options=None,
+      type=None),
+  ],
+  containing_type=None,
+  serialized_options=None,
+  serialized_start=9648,
+  serialized_end=9730,
+)
+_sym_db.RegisterEnumDescriptor(_MATHELEMENT_TYPE)
+
+_ALGORITHMINFO_TYPE = _descriptor.EnumDescriptor(
+  name='Type',
+  full_name='yamcs.protobuf.mdb.AlgorithmInfo.Type',
+  filename=None,
+  file=DESCRIPTOR,
+  values=[
+    _descriptor.EnumValueDescriptor(
+      name='CUSTOM', index=0, number=1,
+      serialized_options=None,
+      type=None),
+    _descriptor.EnumValueDescriptor(
+      name='MATH', index=1, number=2,
+      serialized_options=None,
+      type=None),
+  ],
+  containing_type=None,
+  serialized_options=None,
+  serialized_start=10297,
+  serialized_end=10325,
+)
+_sym_db.RegisterEnumDescriptor(_ALGORITHMINFO_TYPE)
+
 _ALGORITHMINFO_SCOPE = _descriptor.EnumDescriptor(
   name='Scope',
   full_name='yamcs.protobuf.mdb.AlgorithmInfo.Scope',
   filename=None,
   file=DESCRIPTOR,
   values=[
     _descriptor.EnumValueDescriptor(
@@ -341,16 +393,16 @@
     _descriptor.EnumValueDescriptor(
       name='CONTAINER_PROCESSING', index=2, number=2,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=9922,
-  serialized_end=9993,
+  serialized_start=10327,
+  serialized_end=10398,
 )
 _sym_db.RegisterEnumDescriptor(_ALGORITHMINFO_SCOPE)
 
 
 _MISSIONDATABASE = _descriptor.Descriptor(
   name='MissionDatabase',
   full_name='yamcs.protobuf.mdb.MissionDatabase',
@@ -2995,14 +3047,74 @@
   oneofs=[
   ],
   serialized_start=9369,
   serialized_end=9464,
 )
 
 
+_MATHELEMENT = _descriptor.Descriptor(
+  name='MathElement',
+  full_name='yamcs.protobuf.mdb.MathElement',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='yamcs.protobuf.mdb.MathElement.type', index=0,
+      number=1, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=1,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='operator', full_name='yamcs.protobuf.mdb.MathElement.operator', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='value', full_name='yamcs.protobuf.mdb.MathElement.value', index=2,
+      number=3, type=1, cpp_type=5, label=1,
+      has_default_value=False, default_value=float(0),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='parameter', full_name='yamcs.protobuf.mdb.MathElement.parameter', index=3,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='parameterInstance', full_name='yamcs.protobuf.mdb.MathElement.parameterInstance', index=4,
+      number=5, type=5, cpp_type=1, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+    _MATHELEMENT_TYPE,
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=9467,
+  serialized_end=9730,
+)
+
+
 _ALGORITHMINFO = _descriptor.Descriptor(
   name='AlgorithmInfo',
   full_name='yamcs.protobuf.mdb.AlgorithmInfo',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
@@ -3045,70 +3157,85 @@
       name='scope', full_name='yamcs.protobuf.mdb.AlgorithmInfo.scope', index=5,
       number=6, type=14, cpp_type=8, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='language', full_name='yamcs.protobuf.mdb.AlgorithmInfo.language', index=6,
+      name='type', full_name='yamcs.protobuf.mdb.AlgorithmInfo.type', index=6,
+      number=13, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=1,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='language', full_name='yamcs.protobuf.mdb.AlgorithmInfo.language', index=7,
       number=7, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='text', full_name='yamcs.protobuf.mdb.AlgorithmInfo.text', index=7,
+      name='text', full_name='yamcs.protobuf.mdb.AlgorithmInfo.text', index=8,
       number=8, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='inputParameter', full_name='yamcs.protobuf.mdb.AlgorithmInfo.inputParameter', index=8,
+      name='inputParameter', full_name='yamcs.protobuf.mdb.AlgorithmInfo.inputParameter', index=9,
       number=9, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='outputParameter', full_name='yamcs.protobuf.mdb.AlgorithmInfo.outputParameter', index=9,
+      name='outputParameter', full_name='yamcs.protobuf.mdb.AlgorithmInfo.outputParameter', index=10,
       number=10, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='onParameterUpdate', full_name='yamcs.protobuf.mdb.AlgorithmInfo.onParameterUpdate', index=10,
+      name='onParameterUpdate', full_name='yamcs.protobuf.mdb.AlgorithmInfo.onParameterUpdate', index=11,
       number=11, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='onPeriodicRate', full_name='yamcs.protobuf.mdb.AlgorithmInfo.onPeriodicRate', index=11,
+      name='onPeriodicRate', full_name='yamcs.protobuf.mdb.AlgorithmInfo.onPeriodicRate', index=12,
       number=12, type=3, cpp_type=2, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='mathElements', full_name='yamcs.protobuf.mdb.AlgorithmInfo.mathElements', index=13,
+      number=14, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
+    _ALGORITHMINFO_TYPE,
     _ALGORITHMINFO_SCOPE,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9467,
-  serialized_end=9993,
+  serialized_start=9733,
+  serialized_end=10398,
 )
 
 
 _LISTSPACESYSTEMSREQUEST = _descriptor.Descriptor(
   name='ListSpaceSystemsRequest',
   full_name='yamcs.protobuf.mdb.ListSpaceSystemsRequest',
   filename=None,
@@ -3158,16 +3285,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9995,
-  serialized_end=10091,
+  serialized_start=10400,
+  serialized_end=10496,
 )
 
 
 _LISTCONTAINERSREQUEST = _descriptor.Descriptor(
   name='ListContainersRequest',
   full_name='yamcs.protobuf.mdb.ListContainersRequest',
   filename=None,
@@ -3224,16 +3351,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10093,
-  serialized_end=10203,
+  serialized_start=10498,
+  serialized_end=10608,
 )
 
 
 _LISTALGORITHMSREQUEST = _descriptor.Descriptor(
   name='ListAlgorithmsRequest',
   full_name='yamcs.protobuf.mdb.ListAlgorithmsRequest',
   filename=None,
@@ -3297,16 +3424,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10206,
-  serialized_end=10372,
+  serialized_start=10611,
+  serialized_end=10777,
 )
 
 
 _LISTCOMMANDSREQUEST = _descriptor.Descriptor(
   name='ListCommandsRequest',
   full_name='yamcs.protobuf.mdb.ListCommandsRequest',
   filename=None,
@@ -3377,16 +3504,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10375,
-  serialized_end=10520,
+  serialized_start=10780,
+  serialized_end=10925,
 )
 
 
 _GETPARAMETERREQUEST = _descriptor.Descriptor(
   name='GetParameterRequest',
   full_name='yamcs.protobuf.mdb.GetParameterRequest',
   filename=None,
@@ -3415,16 +3542,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10522,
-  serialized_end=10575,
+  serialized_start=10927,
+  serialized_end=10980,
 )
 
 
 _LISTPARAMETERSREQUEST = _descriptor.Descriptor(
   name='ListParametersRequest',
   full_name='yamcs.protobuf.mdb.ListParametersRequest',
   filename=None,
@@ -3509,16 +3636,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10578,
-  serialized_end=10794,
+  serialized_start=10983,
+  serialized_end=11199,
 )
 
 
 _LISTPARAMETERSRESPONSE = _descriptor.Descriptor(
   name='ListParametersResponse',
   full_name='yamcs.protobuf.mdb.ListParametersResponse',
   filename=None,
@@ -3561,16 +3688,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10797,
-  serialized_end=10944,
+  serialized_start=11202,
+  serialized_end=11349,
 )
 
 
 _BATCHGETPARAMETERSREQUEST = _descriptor.Descriptor(
   name='BatchGetParametersRequest',
   full_name='yamcs.protobuf.mdb.BatchGetParametersRequest',
   filename=None,
@@ -3599,16 +3726,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10946,
-  serialized_end=11034,
+  serialized_start=11351,
+  serialized_end=11439,
 )
 
 
 _BATCHGETPARAMETERSRESPONSE_GETPARAMETERRESPONSE = _descriptor.Descriptor(
   name='GetParameterResponse',
   full_name='yamcs.protobuf.mdb.BatchGetParametersResponse.GetParameterResponse',
   filename=None,
@@ -3637,16 +3764,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11154,
-  serialized_end=11273,
+  serialized_start=11559,
+  serialized_end=11678,
 )
 
 _BATCHGETPARAMETERSRESPONSE = _descriptor.Descriptor(
   name='BatchGetParametersResponse',
   full_name='yamcs.protobuf.mdb.BatchGetParametersResponse',
   filename=None,
   file=DESCRIPTOR,
@@ -3667,16 +3794,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11037,
-  serialized_end=11273,
+  serialized_start=11442,
+  serialized_end=11678,
 )
 
 
 _LISTCONTAINERSRESPONSE = _descriptor.Descriptor(
   name='ListContainersResponse',
   full_name='yamcs.protobuf.mdb.ListContainersResponse',
   filename=None,
@@ -3719,16 +3846,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11276,
-  serialized_end=11423,
+  serialized_start=11681,
+  serialized_end=11828,
 )
 
 
 _LISTCOMMANDSRESPONSE = _descriptor.Descriptor(
   name='ListCommandsResponse',
   full_name='yamcs.protobuf.mdb.ListCommandsResponse',
   filename=None,
@@ -3771,16 +3898,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11426,
-  serialized_end=11567,
+  serialized_start=11831,
+  serialized_end=11972,
 )
 
 
 _LISTALGORITHMSRESPONSE = _descriptor.Descriptor(
   name='ListAlgorithmsResponse',
   full_name='yamcs.protobuf.mdb.ListAlgorithmsResponse',
   filename=None,
@@ -3823,16 +3950,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11570,
-  serialized_end=11717,
+  serialized_start=11975,
+  serialized_end=12122,
 )
 
 
 _GETALGORITHMREQUEST = _descriptor.Descriptor(
   name='GetAlgorithmRequest',
   full_name='yamcs.protobuf.mdb.GetAlgorithmRequest',
   filename=None,
@@ -3861,16 +3988,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11719,
-  serialized_end=11772,
+  serialized_start=12124,
+  serialized_end=12177,
 )
 
 
 _GETMISSIONDATABASEREQUEST = _descriptor.Descriptor(
   name='GetMissionDatabaseRequest',
   full_name='yamcs.protobuf.mdb.GetMissionDatabaseRequest',
   filename=None,
@@ -3892,16 +4019,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11774,
-  serialized_end=11819,
+  serialized_start=12179,
+  serialized_end=12224,
 )
 
 
 _EXPORTJAVAMISSIONDATABASEREQUEST = _descriptor.Descriptor(
   name='ExportJavaMissionDatabaseRequest',
   full_name='yamcs.protobuf.mdb.ExportJavaMissionDatabaseRequest',
   filename=None,
@@ -3923,16 +4050,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11821,
-  serialized_end=11873,
+  serialized_start=12226,
+  serialized_end=12278,
 )
 
 
 _LISTSPACESYSTEMSRESPONSE = _descriptor.Descriptor(
   name='ListSpaceSystemsResponse',
   full_name='yamcs.protobuf.mdb.ListSpaceSystemsResponse',
   filename=None,
@@ -3968,16 +4095,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11876,
-  serialized_end=12007,
+  serialized_start=12281,
+  serialized_end=12412,
 )
 
 
 _GETSPACESYSTEMREQUEST = _descriptor.Descriptor(
   name='GetSpaceSystemRequest',
   full_name='yamcs.protobuf.mdb.GetSpaceSystemRequest',
   filename=None,
@@ -4006,16 +4133,54 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12009,
-  serialized_end=12064,
+  serialized_start=12414,
+  serialized_end=12469,
+)
+
+
+_EXPORTXTCEREQUEST = _descriptor.Descriptor(
+  name='ExportXtceRequest',
+  full_name='yamcs.protobuf.mdb.ExportXtceRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='instance', full_name='yamcs.protobuf.mdb.ExportXtceRequest.instance', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='name', full_name='yamcs.protobuf.mdb.ExportXtceRequest.name', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=12471,
+  serialized_end=12522,
 )
 
 
 _GETCOMMANDREQUEST = _descriptor.Descriptor(
   name='GetCommandRequest',
   full_name='yamcs.protobuf.mdb.GetCommandRequest',
   filename=None,
@@ -4044,16 +4209,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12066,
-  serialized_end=12117,
+  serialized_start=12524,
+  serialized_end=12575,
 )
 
 
 _SPACESYSTEMINFO_ANCILLARYDATAENTRY = _descriptor.Descriptor(
   name='AncillaryDataEntry',
   full_name='yamcs.protobuf.mdb.SpaceSystemInfo.AncillaryDataEntry',
   filename=None,
@@ -4168,16 +4333,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12120,
-  serialized_end=12560,
+  serialized_start=12578,
+  serialized_end=13018,
 )
 
 _MISSIONDATABASE.fields_by_name['spaceSystem'].message_type = _SPACESYSTEMINFO
 _ALARMRANGE.fields_by_name['level'].enum_type = _ALARMLEVELTYPE
 _ENUMERATIONALARM.fields_by_name['level'].enum_type = _ALARMLEVELTYPE
 _ALARMINFO.fields_by_name['staticAlarmRange'].message_type = _ALARMRANGE
 _ALARMINFO.fields_by_name['enumerationAlarm'].message_type = _ENUMERATIONALARM
@@ -4275,19 +4440,25 @@
 _CONTAINERINFO.fields_by_name['restrictionCriteria'].message_type = _COMPARISONINFO
 _CONTAINERINFO.fields_by_name['entry'].message_type = _SEQUENCEENTRYINFO
 _CONTAINERINFO.fields_by_name['usedBy'].message_type = _USEDBYINFO
 _CONTAINERINFO.fields_by_name['ancillaryData'].message_type = _CONTAINERINFO_ANCILLARYDATAENTRY
 _INPUTPARAMETERINFO.fields_by_name['parameter'].message_type = _PARAMETERINFO
 _INPUTPARAMETERINFO.fields_by_name['argument'].message_type = _ARGUMENTINFO
 _OUTPUTPARAMETERINFO.fields_by_name['parameter'].message_type = _PARAMETERINFO
+_MATHELEMENT.fields_by_name['type'].enum_type = _MATHELEMENT_TYPE
+_MATHELEMENT.fields_by_name['parameter'].message_type = _PARAMETERINFO
+_MATHELEMENT_TYPE.containing_type = _MATHELEMENT
 _ALGORITHMINFO.fields_by_name['alias'].message_type = yamcs_dot_protobuf_dot_yamcs__pb2._NAMEDOBJECTID
 _ALGORITHMINFO.fields_by_name['scope'].enum_type = _ALGORITHMINFO_SCOPE
+_ALGORITHMINFO.fields_by_name['type'].enum_type = _ALGORITHMINFO_TYPE
 _ALGORITHMINFO.fields_by_name['inputParameter'].message_type = _INPUTPARAMETERINFO
 _ALGORITHMINFO.fields_by_name['outputParameter'].message_type = _OUTPUTPARAMETERINFO
 _ALGORITHMINFO.fields_by_name['onParameterUpdate'].message_type = _PARAMETERINFO
+_ALGORITHMINFO.fields_by_name['mathElements'].message_type = _MATHELEMENT
+_ALGORITHMINFO_TYPE.containing_type = _ALGORITHMINFO
 _ALGORITHMINFO_SCOPE.containing_type = _ALGORITHMINFO
 _LISTALGORITHMSREQUEST.fields_by_name['scope'].enum_type = _ALGORITHMINFO_SCOPE
 _LISTPARAMETERSREQUEST.fields_by_name['source'].enum_type = _DATASOURCETYPE
 _LISTPARAMETERSRESPONSE.fields_by_name['parameters'].message_type = _PARAMETERINFO
 _BATCHGETPARAMETERSREQUEST.fields_by_name['id'].message_type = yamcs_dot_protobuf_dot_yamcs__pb2._NAMEDOBJECTID
 _BATCHGETPARAMETERSRESPONSE_GETPARAMETERRESPONSE.fields_by_name['id'].message_type = yamcs_dot_protobuf_dot_yamcs__pb2._NAMEDOBJECTID
 _BATCHGETPARAMETERSRESPONSE_GETPARAMETERRESPONSE.fields_by_name['parameter'].message_type = _PARAMETERINFO
@@ -4341,14 +4512,15 @@
 DESCRIPTOR.message_types_by_name['RepeatInfo'] = _REPEATINFO
 DESCRIPTOR.message_types_by_name['SequenceEntryInfo'] = _SEQUENCEENTRYINFO
 DESCRIPTOR.message_types_by_name['FixedValueInfo'] = _FIXEDVALUEINFO
 DESCRIPTOR.message_types_by_name['CommandContainerInfo'] = _COMMANDCONTAINERINFO
 DESCRIPTOR.message_types_by_name['ContainerInfo'] = _CONTAINERINFO
 DESCRIPTOR.message_types_by_name['InputParameterInfo'] = _INPUTPARAMETERINFO
 DESCRIPTOR.message_types_by_name['OutputParameterInfo'] = _OUTPUTPARAMETERINFO
+DESCRIPTOR.message_types_by_name['MathElement'] = _MATHELEMENT
 DESCRIPTOR.message_types_by_name['AlgorithmInfo'] = _ALGORITHMINFO
 DESCRIPTOR.message_types_by_name['ListSpaceSystemsRequest'] = _LISTSPACESYSTEMSREQUEST
 DESCRIPTOR.message_types_by_name['ListContainersRequest'] = _LISTCONTAINERSREQUEST
 DESCRIPTOR.message_types_by_name['ListAlgorithmsRequest'] = _LISTALGORITHMSREQUEST
 DESCRIPTOR.message_types_by_name['ListCommandsRequest'] = _LISTCOMMANDSREQUEST
 DESCRIPTOR.message_types_by_name['GetParameterRequest'] = _GETPARAMETERREQUEST
 DESCRIPTOR.message_types_by_name['ListParametersRequest'] = _LISTPARAMETERSREQUEST
@@ -4359,14 +4531,15 @@
 DESCRIPTOR.message_types_by_name['ListCommandsResponse'] = _LISTCOMMANDSRESPONSE
 DESCRIPTOR.message_types_by_name['ListAlgorithmsResponse'] = _LISTALGORITHMSRESPONSE
 DESCRIPTOR.message_types_by_name['GetAlgorithmRequest'] = _GETALGORITHMREQUEST
 DESCRIPTOR.message_types_by_name['GetMissionDatabaseRequest'] = _GETMISSIONDATABASEREQUEST
 DESCRIPTOR.message_types_by_name['ExportJavaMissionDatabaseRequest'] = _EXPORTJAVAMISSIONDATABASEREQUEST
 DESCRIPTOR.message_types_by_name['ListSpaceSystemsResponse'] = _LISTSPACESYSTEMSRESPONSE
 DESCRIPTOR.message_types_by_name['GetSpaceSystemRequest'] = _GETSPACESYSTEMREQUEST
+DESCRIPTOR.message_types_by_name['ExportXtceRequest'] = _EXPORTXTCEREQUEST
 DESCRIPTOR.message_types_by_name['GetCommandRequest'] = _GETCOMMANDREQUEST
 DESCRIPTOR.message_types_by_name['SpaceSystemInfo'] = _SPACESYSTEMINFO
 DESCRIPTOR.enum_types_by_name['DataSourceType'] = _DATASOURCETYPE
 DESCRIPTOR.enum_types_by_name['AlarmLevelType'] = _ALARMLEVELTYPE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 MissionDatabase = _reflection.GeneratedProtocolMessageType('MissionDatabase', (_message.Message,), dict(
@@ -4699,14 +4872,21 @@
 OutputParameterInfo = _reflection.GeneratedProtocolMessageType('OutputParameterInfo', (_message.Message,), dict(
   DESCRIPTOR = _OUTPUTPARAMETERINFO,
   __module__ = 'yamcs.protobuf.mdb.mdb_pb2'
   # @@protoc_insertion_point(class_scope:yamcs.protobuf.mdb.OutputParameterInfo)
   ))
 _sym_db.RegisterMessage(OutputParameterInfo)
 
+MathElement = _reflection.GeneratedProtocolMessageType('MathElement', (_message.Message,), dict(
+  DESCRIPTOR = _MATHELEMENT,
+  __module__ = 'yamcs.protobuf.mdb.mdb_pb2'
+  # @@protoc_insertion_point(class_scope:yamcs.protobuf.mdb.MathElement)
+  ))
+_sym_db.RegisterMessage(MathElement)
+
 AlgorithmInfo = _reflection.GeneratedProtocolMessageType('AlgorithmInfo', (_message.Message,), dict(
   DESCRIPTOR = _ALGORITHMINFO,
   __module__ = 'yamcs.protobuf.mdb.mdb_pb2'
   # @@protoc_insertion_point(class_scope:yamcs.protobuf.mdb.AlgorithmInfo)
   ))
 _sym_db.RegisterMessage(AlgorithmInfo)
 
@@ -4833,14 +5013,21 @@
 GetSpaceSystemRequest = _reflection.GeneratedProtocolMessageType('GetSpaceSystemRequest', (_message.Message,), dict(
   DESCRIPTOR = _GETSPACESYSTEMREQUEST,
   __module__ = 'yamcs.protobuf.mdb.mdb_pb2'
   # @@protoc_insertion_point(class_scope:yamcs.protobuf.mdb.GetSpaceSystemRequest)
   ))
 _sym_db.RegisterMessage(GetSpaceSystemRequest)
 
+ExportXtceRequest = _reflection.GeneratedProtocolMessageType('ExportXtceRequest', (_message.Message,), dict(
+  DESCRIPTOR = _EXPORTXTCEREQUEST,
+  __module__ = 'yamcs.protobuf.mdb.mdb_pb2'
+  # @@protoc_insertion_point(class_scope:yamcs.protobuf.mdb.ExportXtceRequest)
+  ))
+_sym_db.RegisterMessage(ExportXtceRequest)
+
 GetCommandRequest = _reflection.GeneratedProtocolMessageType('GetCommandRequest', (_message.Message,), dict(
   DESCRIPTOR = _GETCOMMANDREQUEST,
   __module__ = 'yamcs.protobuf.mdb.mdb_pb2'
   # @@protoc_insertion_point(class_scope:yamcs.protobuf.mdb.GetCommandRequest)
   ))
 _sym_db.RegisterMessage(GetCommandRequest)
 
@@ -4869,16 +5056,16 @@
 
 _MDBAPI = _descriptor.ServiceDescriptor(
   name='MdbApi',
   full_name='yamcs.protobuf.mdb.MdbApi',
   file=DESCRIPTOR,
   index=0,
   serialized_options=_b('\202\200\001\003MDB'),
-  serialized_start=12822,
-  serialized_end=14761,
+  serialized_start=13280,
+  serialized_end=15354,
   methods=[
   _descriptor.MethodDescriptor(
     name='GetMissionDatabase',
     full_name='yamcs.protobuf.mdb.MdbApi.GetMissionDatabase',
     index=0,
     containing_service=None,
     input_type=_GETMISSIONDATABASEREQUEST,
@@ -4909,89 +5096,98 @@
     index=3,
     containing_service=None,
     input_type=_GETSPACESYSTEMREQUEST,
     output_type=_SPACESYSTEMINFO,
     serialized_options=_b('\212\222\003+\n)/api/mdb/{instance}/space-systems/{name*}'),
   ),
   _descriptor.MethodDescriptor(
+    name='ExportXtce',
+    full_name='yamcs.protobuf.mdb.MdbApi.ExportXtce',
+    index=4,
+    containing_service=None,
+    input_type=_EXPORTXTCEREQUEST,
+    output_type=yamcs_dot_api_dot_httpbody__pb2._HTTPBODY,
+    serialized_options=_b('\212\222\0036\n4/api/mdb/{instance}/space-systems/{name*}:exportXTCE'),
+  ),
+  _descriptor.MethodDescriptor(
     name='ListParameters',
     full_name='yamcs.protobuf.mdb.MdbApi.ListParameters',
-    index=4,
+    index=5,
     containing_service=None,
     input_type=_LISTPARAMETERSREQUEST,
     output_type=_LISTPARAMETERSRESPONSE,
     serialized_options=_b('\212\222\003,\n\036/api/mdb/{instance}/parametersR\nparameters'),
   ),
   _descriptor.MethodDescriptor(
     name='GetParameter',
     full_name='yamcs.protobuf.mdb.MdbApi.GetParameter',
-    index=5,
+    index=6,
     containing_service=None,
     input_type=_GETPARAMETERREQUEST,
     output_type=_PARAMETERINFO,
     serialized_options=_b('\212\222\003(\n&/api/mdb/{instance}/parameters/{name*}'),
   ),
   _descriptor.MethodDescriptor(
     name='BatchGetParameters',
     full_name='yamcs.protobuf.mdb.MdbApi.BatchGetParameters',
-    index=6,
+    index=7,
     containing_service=None,
     input_type=_BATCHGETPARAMETERSREQUEST,
     output_type=_BATCHGETPARAMETERSRESPONSE,
     serialized_options=_b('\212\222\003,\032\'/api/mdb/{instance}/parameters:batchGet:\001*'),
   ),
   _descriptor.MethodDescriptor(
     name='ListContainers',
     full_name='yamcs.protobuf.mdb.MdbApi.ListContainers',
-    index=7,
+    index=8,
     containing_service=None,
     input_type=_LISTCONTAINERSREQUEST,
     output_type=_LISTCONTAINERSRESPONSE,
     serialized_options=_b('\212\222\003,\n\036/api/mdb/{instance}/containersR\ncontainers'),
   ),
   _descriptor.MethodDescriptor(
     name='GetContainer',
     full_name='yamcs.protobuf.mdb.MdbApi.GetContainer',
-    index=8,
+    index=9,
     containing_service=None,
     input_type=_GETCONTAINERREQUEST,
     output_type=_CONTAINERINFO,
     serialized_options=_b('\212\222\003(\n&/api/mdb/{instance}/containers/{name*}'),
   ),
   _descriptor.MethodDescriptor(
     name='ListCommands',
     full_name='yamcs.protobuf.mdb.MdbApi.ListCommands',
-    index=9,
+    index=10,
     containing_service=None,
     input_type=_LISTCOMMANDSREQUEST,
     output_type=_LISTCOMMANDSRESPONSE,
     serialized_options=_b('\212\222\003(\n\034/api/mdb/{instance}/commandsR\010commands'),
   ),
   _descriptor.MethodDescriptor(
     name='GetCommand',
     full_name='yamcs.protobuf.mdb.MdbApi.GetCommand',
-    index=10,
+    index=11,
     containing_service=None,
     input_type=_GETCOMMANDREQUEST,
     output_type=_COMMANDINFO,
     serialized_options=_b('\212\222\003&\n$/api/mdb/{instance}/commands/{name*}'),
   ),
   _descriptor.MethodDescriptor(
     name='ListAlgorithms',
     full_name='yamcs.protobuf.mdb.MdbApi.ListAlgorithms',
-    index=11,
+    index=12,
     containing_service=None,
     input_type=_LISTALGORITHMSREQUEST,
     output_type=_LISTALGORITHMSRESPONSE,
     serialized_options=_b('\212\222\003,\n\036/api/mdb/{instance}/algorithmsR\nalgorithms'),
   ),
   _descriptor.MethodDescriptor(
     name='GetAlgorithm',
     full_name='yamcs.protobuf.mdb.MdbApi.GetAlgorithm',
-    index=12,
+    index=13,
     containing_service=None,
     input_type=_GETALGORITHMREQUEST,
     output_type=_ALGORITHMINFO,
     serialized_options=_b('\212\222\003(\n&/api/mdb/{instance}/algorithms/{name*}'),
   ),
 ])
 _sym_db.RegisterServiceDescriptor(_MDBAPI)
```

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/packets/packets_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/packets/packets_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/packets/packets_service_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/packets/packets_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/processing/mdb_override_service_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/processing/mdb_override_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/processing/processing_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/processing/processing_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/pvalue/pvalue_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/pvalue/pvalue_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/replication/replication_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/replication/replication_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/table/table_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/table/table_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='yamcs/protobuf/table/table.proto',
   package='yamcs.protobuf.table',
   syntax='proto2',
   serialized_options=_b('\n\022org.yamcs.protobuf'),
-  serialized_pb=_b('\n yamcs/protobuf/table/table.proto\x12\x14yamcs.protobuf.table\x1a\x1byamcs/api/annotations.proto\x1a\x1ayamcs/protobuf/yamcs.proto\x1a\x34yamcs/protobuf/yamcsManagement/yamcsManagement.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xdd\x01\n\x03Row\x12\x35\n\x07\x63olumns\x18\x01 \x03(\x0b\x32$.yamcs.protobuf.table.Row.ColumnInfo\x12-\n\x05\x63\x65lls\x18\x02 \x03(\x0b\x32\x1e.yamcs.protobuf.table.Row.Cell\x1aH\n\nColumnInfo\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x12\n\nprotoClass\x18\x04 \x01(\t\x1a&\n\x04\x43\x65ll\x12\x10\n\x08\x63olumnId\x18\x01 \x01(\r\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"@\n\x0fReadRowsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0c\n\x04\x63ols\x18\x03 \x03(\t\"[\n\x10WriteRowsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12&\n\x03row\x18\x03 \x01(\x0b\x32\x19.yamcs.protobuf.table.Row\"\"\n\x11WriteRowsResponse\x12\r\n\x05\x63ount\x18\x01 \x01(\r\")\n\x18WriteRowsExceptionDetail\x12\r\n\x05\x63ount\x18\x01 \x01(\r\"2\n\tListValue\x12%\n\x06values\x18\x01 \x03(\x0b\x32\x15.yamcs.protobuf.Value\"8\n\x11\x45xecuteSqlRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tstatement\x18\x02 \x01(\t\"m\n\tResultSet\x12\x31\n\x07\x63olumns\x18\x01 \x03(\x0b\x32 .yamcs.protobuf.table.ColumnInfo\x12-\n\x04rows\x18\x02 \x03(\x0b\x32\x1f.yamcs.protobuf.table.ListValue\"%\n\x11ListTablesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"E\n\x12ListTablesResponse\x12/\n\x06tables\x18\x01 \x03(\x0b\x32\x1f.yamcs.protobuf.table.TableInfo\"1\n\x0fGetTableRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"n\n\x13GetTableDataRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ols\x18\x03 \x03(\t\x12\x0b\n\x03pos\x18\x04 \x01(\x03\x12\r\n\x05limit\x18\x05 \x01(\x05\x12\r\n\x05order\x18\x06 \x01(\t\"&\n\x12ListStreamsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"H\n\x13ListStreamsResponse\x12\x31\n\x07streams\x18\x01 \x03(\x0b\x32 .yamcs.protobuf.table.StreamInfo\"2\n\x10GetStreamRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\":\n\x16SubscribeStreamRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0e\n\x06stream\x18\x02 \x01(\t\"@\n\nColumnData\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.yamcs.protobuf.Value\"N\n\nStreamData\x12\x0e\n\x06stream\x18\x01 \x01(\t\x12\x30\n\x06\x63olumn\x18\x02 \x03(\x0b\x32 .yamcs.protobuf.table.ColumnData\"4\n SubscribeStreamStatisticsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"\x89\x01\n\tTableData\x12;\n\x06record\x18\x01 \x03(\x0b\x32+.yamcs.protobuf.table.TableData.TableRecord\x1a?\n\x0bTableRecord\x12\x30\n\x06\x63olumn\x18\x01 \x03(\x0b\x32 .yamcs.protobuf.table.ColumnData\"s\n\nColumnInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x32\n\tenumValue\x18\x03 \x03(\x0b\x32\x1f.yamcs.protobuf.table.EnumValue\x12\x15\n\rautoIncrement\x18\x04 \x01(\x08\")\n\tEnumValue\x12\r\n\x05value\x18\x01 \x01(\x05\x12\r\n\x05label\x18\x02 \x01(\t\"\xc6\x02\n\tTableInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x33\n\tkeyColumn\x18\x02 \x03(\x0b\x32 .yamcs.protobuf.table.ColumnInfo\x12\x35\n\x0bvalueColumn\x18\x03 \x03(\x0b\x32 .yamcs.protobuf.table.ColumnInfo\x12\x0e\n\x06script\x18\x04 \x01(\t\x12\x17\n\x0fhistogramColumn\x18\x05 \x03(\t\x12\x15\n\rstorageEngine\x18\x06 \x01(\t\x12\x15\n\rformatVersion\x18\x07 \x01(\x05\x12\x12\n\ntablespace\x18\x08 \x01(\t\x12\x12\n\ncompressed\x18\t \x01(\x08\x12@\n\x10partitioningInfo\x18\n \x01(\x0b\x32&.yamcs.protobuf.table.PartitioningInfo\"\xf5\x01\n\x10PartitioningInfo\x12\x45\n\x04type\x18\x01 \x01(\x0e\x32\x37.yamcs.protobuf.table.PartitioningInfo.PartitioningType\x12\x12\n\ntimeColumn\x18\x02 \x01(\t\x12\x1b\n\x13timePartitionSchema\x18\x03 \x01(\t\x12\x13\n\x0bvalueColumn\x18\x04 \x01(\t\x12\x17\n\x0fvalueColumnType\x18\x05 \x01(\t\";\n\x10PartitioningType\x12\x08\n\x04TIME\x10\x01\x12\t\n\x05VALUE\x10\x02\x12\x12\n\x0eTIME_AND_VALUE\x10\x03\"o\n\nStreamInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x30\n\x06\x63olumn\x18\x02 \x03(\x0b\x32 .yamcs.protobuf.table.ColumnInfo\x12\x0e\n\x06script\x18\x03 \x01(\t\x12\x11\n\tdataCount\x18\x04 \x01(\x03\"\x8f\x01\n\x17RebuildHistogramRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12)\n\x05start\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x1a\n\x18RebuildHistogramResponse2\xbf\r\n\x08TableApi\x12\x83\x01\n\nExecuteSql\x12\'.yamcs.protobuf.table.ExecuteSqlRequest\x1a\x1f.yamcs.protobuf.table.ResultSet\"+\x8a\x92\x03\'\x1a\"/api/archive/{instance}:executeSql:\x01*\x12\x97\x01\n\x13\x45xecuteStreamingSql\x12\'.yamcs.protobuf.table.ExecuteSqlRequest\x1a\x1f.yamcs.protobuf.table.ResultSet\"4\x8a\x92\x03\x30\x1a+/api/archive/{instance}:executeStreamingSql:\x01*0\x01\x12\x89\x01\n\x0bListStreams\x12(.yamcs.protobuf.table.ListStreamsRequest\x1a).yamcs.protobuf.table.ListStreamsResponse\"%\x8a\x92\x03!\n\x1f/api/archive/{instance}/streams\x12\x96\x01\n\x19SubscribeStreamStatistics\x12\x36.yamcs.protobuf.table.SubscribeStreamStatisticsRequest\x1a+.yamcs.protobuf.yamcsManagement.StreamEvent\"\x12\xda\x92\x03\x0e\n\x0cstream-stats0\x01\x12\x83\x01\n\tGetStream\x12&.yamcs.protobuf.table.GetStreamRequest\x1a .yamcs.protobuf.table.StreamInfo\",\x8a\x92\x03(\n&/api/archive/{instance}/streams/{name}\x12q\n\x0fSubscribeStream\x12,.yamcs.protobuf.table.SubscribeStreamRequest\x1a .yamcs.protobuf.table.StreamData\"\x0c\xda\x92\x03\x08\n\x06stream0\x01\x12\x85\x01\n\nListTables\x12\'.yamcs.protobuf.table.ListTablesRequest\x1a(.yamcs.protobuf.table.ListTablesResponse\"$\x8a\x92\x03 \n\x1e/api/archive/{instance}/tables\x12\x7f\n\x08GetTable\x12%.yamcs.protobuf.table.GetTableRequest\x1a\x1f.yamcs.protobuf.table.TableInfo\"+\x8a\x92\x03\'\n%/api/archive/{instance}/tables/{name}\x12\x8c\x01\n\x0cGetTableData\x12).yamcs.protobuf.table.GetTableDataRequest\x1a\x1f.yamcs.protobuf.table.TableData\"0\x8a\x92\x03,\n*/api/archive/{instance}/tables/{name}/data\x12\x88\x01\n\x08ReadRows\x12%.yamcs.protobuf.table.ReadRowsRequest\x1a\x19.yamcs.protobuf.table.Row\"8\x8a\x92\x03\x34\x1a//api/archive/{instance}/tables/{table}:readRows:\x01*0\x01\x12\x9b\x01\n\tWriteRows\x12&.yamcs.protobuf.table.WriteRowsRequest\x1a\'.yamcs.protobuf.table.WriteRowsResponse\";\x8a\x92\x03\x37\x1a\x30/api/archive/{instance}/tables/{table}:writeRows:\x03row(\x01\x12\xb3\x01\n\x10RebuildHistogram\x12-.yamcs.protobuf.table.RebuildHistogramRequest\x1a..yamcs.protobuf.table.RebuildHistogramResponse\"@\x8a\x92\x03<\x1a\x37/api/archive/{instance}/tables/{table}:rebuildHistogram:\x01*B\x14\n\x12org.yamcs.protobuf')
+  serialized_pb=_b('\n yamcs/protobuf/table/table.proto\x12\x14yamcs.protobuf.table\x1a\x1byamcs/api/annotations.proto\x1a\x1ayamcs/protobuf/yamcs.proto\x1a\x34yamcs/protobuf/yamcsManagement/yamcsManagement.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xdd\x01\n\x03Row\x12\x35\n\x07\x63olumns\x18\x01 \x03(\x0b\x32$.yamcs.protobuf.table.Row.ColumnInfo\x12-\n\x05\x63\x65lls\x18\x02 \x03(\x0b\x32\x1e.yamcs.protobuf.table.Row.Cell\x1aH\n\nColumnInfo\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x12\n\nprotoClass\x18\x04 \x01(\t\x1a&\n\x04\x43\x65ll\x12\x10\n\x08\x63olumnId\x18\x01 \x01(\r\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"O\n\x0fReadRowsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x0c\n\x04\x63ols\x18\x03 \x03(\t\x12\r\n\x05query\x18\x04 \x01(\t\"[\n\x10WriteRowsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12&\n\x03row\x18\x03 \x01(\x0b\x32\x19.yamcs.protobuf.table.Row\"\"\n\x11WriteRowsResponse\x12\r\n\x05\x63ount\x18\x01 \x01(\r\")\n\x18WriteRowsExceptionDetail\x12\r\n\x05\x63ount\x18\x01 \x01(\r\"2\n\tListValue\x12%\n\x06values\x18\x01 \x03(\x0b\x32\x15.yamcs.protobuf.Value\"8\n\x11\x45xecuteSqlRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tstatement\x18\x02 \x01(\t\"m\n\tResultSet\x12\x31\n\x07\x63olumns\x18\x01 \x03(\x0b\x32 .yamcs.protobuf.table.ColumnInfo\x12-\n\x04rows\x18\x02 \x03(\x0b\x32\x1f.yamcs.protobuf.table.ListValue\"%\n\x11ListTablesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"E\n\x12ListTablesResponse\x12/\n\x06tables\x18\x01 \x03(\x0b\x32\x1f.yamcs.protobuf.table.TableInfo\"1\n\x0fGetTableRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"n\n\x13GetTableDataRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ols\x18\x03 \x03(\t\x12\x0b\n\x03pos\x18\x04 \x01(\x03\x12\r\n\x05limit\x18\x05 \x01(\x05\x12\r\n\x05order\x18\x06 \x01(\t\"&\n\x12ListStreamsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"H\n\x13ListStreamsResponse\x12\x31\n\x07streams\x18\x01 \x03(\x0b\x32 .yamcs.protobuf.table.StreamInfo\"2\n\x10GetStreamRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\":\n\x16SubscribeStreamRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0e\n\x06stream\x18\x02 \x01(\t\"@\n\nColumnData\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x15.yamcs.protobuf.Value\"N\n\nStreamData\x12\x0e\n\x06stream\x18\x01 \x01(\t\x12\x30\n\x06\x63olumn\x18\x02 \x03(\x0b\x32 .yamcs.protobuf.table.ColumnData\"4\n SubscribeStreamStatisticsRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"\x89\x01\n\tTableData\x12;\n\x06record\x18\x01 \x03(\x0b\x32+.yamcs.protobuf.table.TableData.TableRecord\x1a?\n\x0bTableRecord\x12\x30\n\x06\x63olumn\x18\x01 \x03(\x0b\x32 .yamcs.protobuf.table.ColumnData\"s\n\nColumnInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x32\n\tenumValue\x18\x03 \x03(\x0b\x32\x1f.yamcs.protobuf.table.EnumValue\x12\x15\n\rautoIncrement\x18\x04 \x01(\x08\")\n\tEnumValue\x12\r\n\x05value\x18\x01 \x01(\x05\x12\r\n\x05label\x18\x02 \x01(\t\"\xc6\x02\n\tTableInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x33\n\tkeyColumn\x18\x02 \x03(\x0b\x32 .yamcs.protobuf.table.ColumnInfo\x12\x35\n\x0bvalueColumn\x18\x03 \x03(\x0b\x32 .yamcs.protobuf.table.ColumnInfo\x12\x0e\n\x06script\x18\x04 \x01(\t\x12\x17\n\x0fhistogramColumn\x18\x05 \x03(\t\x12\x15\n\rstorageEngine\x18\x06 \x01(\t\x12\x15\n\rformatVersion\x18\x07 \x01(\x05\x12\x12\n\ntablespace\x18\x08 \x01(\t\x12\x12\n\ncompressed\x18\t \x01(\x08\x12@\n\x10partitioningInfo\x18\n \x01(\x0b\x32&.yamcs.protobuf.table.PartitioningInfo\"\xf5\x01\n\x10PartitioningInfo\x12\x45\n\x04type\x18\x01 \x01(\x0e\x32\x37.yamcs.protobuf.table.PartitioningInfo.PartitioningType\x12\x12\n\ntimeColumn\x18\x02 \x01(\t\x12\x1b\n\x13timePartitionSchema\x18\x03 \x01(\t\x12\x13\n\x0bvalueColumn\x18\x04 \x01(\t\x12\x17\n\x0fvalueColumnType\x18\x05 \x01(\t\";\n\x10PartitioningType\x12\x08\n\x04TIME\x10\x01\x12\t\n\x05VALUE\x10\x02\x12\x12\n\x0eTIME_AND_VALUE\x10\x03\"o\n\nStreamInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x30\n\x06\x63olumn\x18\x02 \x03(\x0b\x32 .yamcs.protobuf.table.ColumnInfo\x12\x0e\n\x06script\x18\x03 \x01(\t\x12\x11\n\tdataCount\x18\x04 \x01(\x03\"\x8f\x01\n\x17RebuildHistogramRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12)\n\x05start\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x04stop\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x1a\n\x18RebuildHistogramResponse2\xbf\r\n\x08TableApi\x12\x83\x01\n\nExecuteSql\x12\'.yamcs.protobuf.table.ExecuteSqlRequest\x1a\x1f.yamcs.protobuf.table.ResultSet\"+\x8a\x92\x03\'\x1a\"/api/archive/{instance}:executeSql:\x01*\x12\x97\x01\n\x13\x45xecuteStreamingSql\x12\'.yamcs.protobuf.table.ExecuteSqlRequest\x1a\x1f.yamcs.protobuf.table.ResultSet\"4\x8a\x92\x03\x30\x1a+/api/archive/{instance}:executeStreamingSql:\x01*0\x01\x12\x89\x01\n\x0bListStreams\x12(.yamcs.protobuf.table.ListStreamsRequest\x1a).yamcs.protobuf.table.ListStreamsResponse\"%\x8a\x92\x03!\n\x1f/api/archive/{instance}/streams\x12\x96\x01\n\x19SubscribeStreamStatistics\x12\x36.yamcs.protobuf.table.SubscribeStreamStatisticsRequest\x1a+.yamcs.protobuf.yamcsManagement.StreamEvent\"\x12\xda\x92\x03\x0e\n\x0cstream-stats0\x01\x12\x83\x01\n\tGetStream\x12&.yamcs.protobuf.table.GetStreamRequest\x1a .yamcs.protobuf.table.StreamInfo\",\x8a\x92\x03(\n&/api/archive/{instance}/streams/{name}\x12q\n\x0fSubscribeStream\x12,.yamcs.protobuf.table.SubscribeStreamRequest\x1a .yamcs.protobuf.table.StreamData\"\x0c\xda\x92\x03\x08\n\x06stream0\x01\x12\x85\x01\n\nListTables\x12\'.yamcs.protobuf.table.ListTablesRequest\x1a(.yamcs.protobuf.table.ListTablesResponse\"$\x8a\x92\x03 \n\x1e/api/archive/{instance}/tables\x12\x7f\n\x08GetTable\x12%.yamcs.protobuf.table.GetTableRequest\x1a\x1f.yamcs.protobuf.table.TableInfo\"+\x8a\x92\x03\'\n%/api/archive/{instance}/tables/{name}\x12\x8c\x01\n\x0cGetTableData\x12).yamcs.protobuf.table.GetTableDataRequest\x1a\x1f.yamcs.protobuf.table.TableData\"0\x8a\x92\x03,\n*/api/archive/{instance}/tables/{name}/data\x12\x88\x01\n\x08ReadRows\x12%.yamcs.protobuf.table.ReadRowsRequest\x1a\x19.yamcs.protobuf.table.Row\"8\x8a\x92\x03\x34\x1a//api/archive/{instance}/tables/{table}:readRows:\x01*0\x01\x12\x9b\x01\n\tWriteRows\x12&.yamcs.protobuf.table.WriteRowsRequest\x1a\'.yamcs.protobuf.table.WriteRowsResponse\";\x8a\x92\x03\x37\x1a\x30/api/archive/{instance}/tables/{table}:writeRows:\x03row(\x01\x12\xb3\x01\n\x10RebuildHistogram\x12-.yamcs.protobuf.table.RebuildHistogramRequest\x1a..yamcs.protobuf.table.RebuildHistogramResponse\"@\x8a\x92\x03<\x1a\x37/api/archive/{instance}/tables/{table}:rebuildHistogram:\x01*B\x14\n\x12org.yamcs.protobuf')
   ,
   dependencies=[yamcs_dot_api_dot_annotations__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_yamcs__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_yamcsManagement_dot_yamcsManagement__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,])
 
 
 
 _PARTITIONINGINFO_PARTITIONINGTYPE = _descriptor.EnumDescriptor(
   name='PartitioningType',
@@ -47,16 +47,16 @@
     _descriptor.EnumValueDescriptor(
       name='TIME_AND_VALUE', index=2, number=3,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2400,
-  serialized_end=2459,
+  serialized_start=2415,
+  serialized_end=2474,
 )
 _sym_db.RegisterEnumDescriptor(_PARTITIONINGINFO_PARTITIONINGTYPE)
 
 
 _ROW_COLUMNINFO = _descriptor.Descriptor(
   name='ColumnInfo',
   full_name='yamcs.protobuf.table.Row.ColumnInfo',
@@ -207,28 +207,35 @@
     _descriptor.FieldDescriptor(
       name='cols', full_name='yamcs.protobuf.table.ReadRowsRequest.cols', index=2,
       number=3, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='query', full_name='yamcs.protobuf.table.ReadRowsRequest.query', index=3,
+      number=4, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=426,
-  serialized_end=490,
+  serialized_end=505,
 )
 
 
 _WRITEROWSREQUEST = _descriptor.Descriptor(
   name='WriteRowsRequest',
   full_name='yamcs.protobuf.table.WriteRowsRequest',
   filename=None,
@@ -264,16 +271,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=492,
-  serialized_end=583,
+  serialized_start=507,
+  serialized_end=598,
 )
 
 
 _WRITEROWSRESPONSE = _descriptor.Descriptor(
   name='WriteRowsResponse',
   full_name='yamcs.protobuf.table.WriteRowsResponse',
   filename=None,
@@ -295,16 +302,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=585,
-  serialized_end=619,
+  serialized_start=600,
+  serialized_end=634,
 )
 
 
 _WRITEROWSEXCEPTIONDETAIL = _descriptor.Descriptor(
   name='WriteRowsExceptionDetail',
   full_name='yamcs.protobuf.table.WriteRowsExceptionDetail',
   filename=None,
@@ -326,16 +333,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=621,
-  serialized_end=662,
+  serialized_start=636,
+  serialized_end=677,
 )
 
 
 _LISTVALUE = _descriptor.Descriptor(
   name='ListValue',
   full_name='yamcs.protobuf.table.ListValue',
   filename=None,
@@ -357,16 +364,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=664,
-  serialized_end=714,
+  serialized_start=679,
+  serialized_end=729,
 )
 
 
 _EXECUTESQLREQUEST = _descriptor.Descriptor(
   name='ExecuteSqlRequest',
   full_name='yamcs.protobuf.table.ExecuteSqlRequest',
   filename=None,
@@ -395,16 +402,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=716,
-  serialized_end=772,
+  serialized_start=731,
+  serialized_end=787,
 )
 
 
 _RESULTSET = _descriptor.Descriptor(
   name='ResultSet',
   full_name='yamcs.protobuf.table.ResultSet',
   filename=None,
@@ -433,16 +440,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=774,
-  serialized_end=883,
+  serialized_start=789,
+  serialized_end=898,
 )
 
 
 _LISTTABLESREQUEST = _descriptor.Descriptor(
   name='ListTablesRequest',
   full_name='yamcs.protobuf.table.ListTablesRequest',
   filename=None,
@@ -464,16 +471,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=885,
-  serialized_end=922,
+  serialized_start=900,
+  serialized_end=937,
 )
 
 
 _LISTTABLESRESPONSE = _descriptor.Descriptor(
   name='ListTablesResponse',
   full_name='yamcs.protobuf.table.ListTablesResponse',
   filename=None,
@@ -495,16 +502,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=924,
-  serialized_end=993,
+  serialized_start=939,
+  serialized_end=1008,
 )
 
 
 _GETTABLEREQUEST = _descriptor.Descriptor(
   name='GetTableRequest',
   full_name='yamcs.protobuf.table.GetTableRequest',
   filename=None,
@@ -533,16 +540,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=995,
-  serialized_end=1044,
+  serialized_start=1010,
+  serialized_end=1059,
 )
 
 
 _GETTABLEDATAREQUEST = _descriptor.Descriptor(
   name='GetTableDataRequest',
   full_name='yamcs.protobuf.table.GetTableDataRequest',
   filename=None,
@@ -599,16 +606,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1046,
-  serialized_end=1156,
+  serialized_start=1061,
+  serialized_end=1171,
 )
 
 
 _LISTSTREAMSREQUEST = _descriptor.Descriptor(
   name='ListStreamsRequest',
   full_name='yamcs.protobuf.table.ListStreamsRequest',
   filename=None,
@@ -630,16 +637,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1158,
-  serialized_end=1196,
+  serialized_start=1173,
+  serialized_end=1211,
 )
 
 
 _LISTSTREAMSRESPONSE = _descriptor.Descriptor(
   name='ListStreamsResponse',
   full_name='yamcs.protobuf.table.ListStreamsResponse',
   filename=None,
@@ -661,16 +668,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1198,
-  serialized_end=1270,
+  serialized_start=1213,
+  serialized_end=1285,
 )
 
 
 _GETSTREAMREQUEST = _descriptor.Descriptor(
   name='GetStreamRequest',
   full_name='yamcs.protobuf.table.GetStreamRequest',
   filename=None,
@@ -699,16 +706,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1272,
-  serialized_end=1322,
+  serialized_start=1287,
+  serialized_end=1337,
 )
 
 
 _SUBSCRIBESTREAMREQUEST = _descriptor.Descriptor(
   name='SubscribeStreamRequest',
   full_name='yamcs.protobuf.table.SubscribeStreamRequest',
   filename=None,
@@ -737,16 +744,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1324,
-  serialized_end=1382,
+  serialized_start=1339,
+  serialized_end=1397,
 )
 
 
 _COLUMNDATA = _descriptor.Descriptor(
   name='ColumnData',
   full_name='yamcs.protobuf.table.ColumnData',
   filename=None,
@@ -775,16 +782,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1384,
-  serialized_end=1448,
+  serialized_start=1399,
+  serialized_end=1463,
 )
 
 
 _STREAMDATA = _descriptor.Descriptor(
   name='StreamData',
   full_name='yamcs.protobuf.table.StreamData',
   filename=None,
@@ -813,16 +820,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1450,
-  serialized_end=1528,
+  serialized_start=1465,
+  serialized_end=1543,
 )
 
 
 _SUBSCRIBESTREAMSTATISTICSREQUEST = _descriptor.Descriptor(
   name='SubscribeStreamStatisticsRequest',
   full_name='yamcs.protobuf.table.SubscribeStreamStatisticsRequest',
   filename=None,
@@ -844,16 +851,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1530,
-  serialized_end=1582,
+  serialized_start=1545,
+  serialized_end=1597,
 )
 
 
 _TABLEDATA_TABLERECORD = _descriptor.Descriptor(
   name='TableRecord',
   full_name='yamcs.protobuf.table.TableData.TableRecord',
   filename=None,
@@ -875,16 +882,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1659,
-  serialized_end=1722,
+  serialized_start=1674,
+  serialized_end=1737,
 )
 
 _TABLEDATA = _descriptor.Descriptor(
   name='TableData',
   full_name='yamcs.protobuf.table.TableData',
   filename=None,
   file=DESCRIPTOR,
@@ -905,16 +912,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1585,
-  serialized_end=1722,
+  serialized_start=1600,
+  serialized_end=1737,
 )
 
 
 _COLUMNINFO = _descriptor.Descriptor(
   name='ColumnInfo',
   full_name='yamcs.protobuf.table.ColumnInfo',
   filename=None,
@@ -957,16 +964,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1724,
-  serialized_end=1839,
+  serialized_start=1739,
+  serialized_end=1854,
 )
 
 
 _ENUMVALUE = _descriptor.Descriptor(
   name='EnumValue',
   full_name='yamcs.protobuf.table.EnumValue',
   filename=None,
@@ -995,16 +1002,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1841,
-  serialized_end=1882,
+  serialized_start=1856,
+  serialized_end=1897,
 )
 
 
 _TABLEINFO = _descriptor.Descriptor(
   name='TableInfo',
   full_name='yamcs.protobuf.table.TableInfo',
   filename=None,
@@ -1089,16 +1096,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1885,
-  serialized_end=2211,
+  serialized_start=1900,
+  serialized_end=2226,
 )
 
 
 _PARTITIONINGINFO = _descriptor.Descriptor(
   name='PartitioningInfo',
   full_name='yamcs.protobuf.table.PartitioningInfo',
   filename=None,
@@ -1149,16 +1156,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2214,
-  serialized_end=2459,
+  serialized_start=2229,
+  serialized_end=2474,
 )
 
 
 _STREAMINFO = _descriptor.Descriptor(
   name='StreamInfo',
   full_name='yamcs.protobuf.table.StreamInfo',
   filename=None,
@@ -1201,16 +1208,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2461,
-  serialized_end=2572,
+  serialized_start=2476,
+  serialized_end=2587,
 )
 
 
 _REBUILDHISTOGRAMREQUEST = _descriptor.Descriptor(
   name='RebuildHistogramRequest',
   full_name='yamcs.protobuf.table.RebuildHistogramRequest',
   filename=None,
@@ -1253,16 +1260,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2575,
-  serialized_end=2718,
+  serialized_start=2590,
+  serialized_end=2733,
 )
 
 
 _REBUILDHISTOGRAMRESPONSE = _descriptor.Descriptor(
   name='RebuildHistogramResponse',
   full_name='yamcs.protobuf.table.RebuildHistogramResponse',
   filename=None,
@@ -1277,16 +1284,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2720,
-  serialized_end=2746,
+  serialized_start=2735,
+  serialized_end=2761,
 )
 
 _ROW_COLUMNINFO.containing_type = _ROW
 _ROW_CELL.containing_type = _ROW
 _ROW.fields_by_name['columns'].message_type = _ROW_COLUMNINFO
 _ROW.fields_by_name['cells'].message_type = _ROW_CELL
 _WRITEROWSREQUEST.fields_by_name['row'].message_type = _ROW
@@ -1556,16 +1563,16 @@
 
 _TABLEAPI = _descriptor.ServiceDescriptor(
   name='TableApi',
   full_name='yamcs.protobuf.table.TableApi',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
-  serialized_start=2749,
-  serialized_end=4476,
+  serialized_start=2764,
+  serialized_end=4491,
   methods=[
   _descriptor.MethodDescriptor(
     name='ExecuteSql',
     full_name='yamcs.protobuf.table.TableApi.ExecuteSql',
     index=0,
     containing_service=None,
     input_type=_EXECUTESQLREQUEST,
```

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/tco/tco_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/tco/tco_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/time/time_service_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/time/time_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/timeline/timeline_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/timeline/timeline_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/web/auth_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/web/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/web/server_service_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/web/server_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='yamcs/protobuf/yamcsManagement/yamcsManagement.proto',
   package='yamcs.protobuf.yamcsManagement',
   syntax='proto2',
   serialized_options=_b('\n\022org.yamcs.protobufB\024YamcsManagementProtoP\001'),
-  serialized_pb=_b('\n4yamcs/protobuf/yamcsManagement/yamcsManagement.proto\x12\x1eyamcs.protobuf.yamcsManagement\x1a\x1egoogle/protobuf/duration.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1byamcs/api/annotations.proto\x1a\x1ayamcs/protobuf/yamcs.proto\x1a\x1cyamcs/protobuf/mdb/mdb.proto\"R\n\x0eYamcsInstances\x12@\n\tinstances\x18\x01 \x03(\x0b\x32-.yamcs.protobuf.yamcsManagement.YamcsInstance\"\x89\x06\n\rYamcsInstance\x12\x0c\n\x04name\x18\x01 \x01(\t\x12<\n\x0fmissionDatabase\x18\x03 \x01(\x0b\x32#.yamcs.protobuf.mdb.MissionDatabase\x12\x41\n\nprocessors\x18\x04 \x03(\x0b\x32-.yamcs.protobuf.yamcsManagement.ProcessorInfo\x12J\n\x05state\x18\x0b \x01(\x0e\x32;.yamcs.protobuf.yamcsManagement.YamcsInstance.InstanceState\x12\x14\n\x0c\x66\x61ilureCause\x18\t \x01(\t\x12/\n\x0bmissionTime\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x06labels\x18\x0c \x03(\x0b\x32\x39.yamcs.protobuf.yamcsManagement.YamcsInstance.LabelsEntry\x12\x14\n\x0c\x63\x61pabilities\x18\r \x03(\t\x12\x10\n\x08template\x18\x0e \x01(\t\x12U\n\x0ctemplateArgs\x18\x0f \x03(\x0b\x32?.yamcs.protobuf.yamcsManagement.YamcsInstance.TemplateArgsEntry\x12\x19\n\x11templateAvailable\x18\x10 \x01(\x08\x12\x17\n\x0ftemplateChanged\x18\x11 \x01(\x08\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x33\n\x11TemplateArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"t\n\rInstanceState\x12\x0b\n\x07OFFLINE\x10\x00\x12\x10\n\x0cINITIALIZING\x10\x01\x12\x0f\n\x0bINITIALIZED\x10\x02\x12\x0c\n\x08STARTING\x10\x03\x12\x0b\n\x07RUNNING\x10\x04\x12\x0c\n\x08STOPPING\x10\x05\x12\n\n\x06\x46\x41ILED\x10\x06\"z\n\x10InstanceTemplate\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x43\n\tvariables\x18\x02 \x03(\x0b\x32\x30.yamcs.protobuf.yamcsManagement.TemplateVariable\"\x7f\n\x10TemplateVariable\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05label\x18\x06 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x0c\n\x04help\x18\x02 \x01(\t\x12\x10\n\x08required\x18\x03 \x01(\x08\x12\x0f\n\x07\x63hoices\x18\x05 \x03(\t\x12\x0f\n\x07initial\x18\x07 \x01(\t\"\xf7\x03\n\rProcessorInfo\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04spec\x18\x04 \x01(\t\x12\x0f\n\x07\x63reator\x18\x05 \x01(\t\x12\x11\n\thasAlarms\x18\x06 \x01(\x08\x12\x15\n\rhasCommanding\x18\x07 \x01(\x08\x12;\n\x05state\x18\x08 \x01(\x0e\x32,.yamcs.protobuf.yamcsManagement.ServiceState\x12\x34\n\rreplayRequest\x18\t \x01(\x0b\x32\x1d.yamcs.protobuf.ReplayRequest\x12=\n\x0breplayState\x18\n \x01(\x0e\x32(.yamcs.protobuf.ReplayStatus.ReplayState\x12=\n\x08services\x18\x10 \x03(\x0b\x32+.yamcs.protobuf.yamcsManagement.ServiceInfo\x12\x12\n\npersistent\x18\x11 \x01(\x08\x12(\n\x04time\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06replay\x18\x13 \x01(\x08\x12\x1d\n\x15\x63heckCommandClearance\x18\x14 \x01(\x08\x12\x11\n\tprotected\x18\x15 \x01(\x08\"\x98\x02\n\x0cTmStatistics\x12\x12\n\npacketName\x18\x01 \x01(\t\x12\x15\n\rqualifiedName\x18\t \x01(\t\x12\x17\n\x0freceivedPackets\x18\x02 \x01(\x03\x12 \n\x18subscribedParameterCount\x18\x06 \x01(\x05\x12\x30\n\x0clastReceived\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0elastPacketTime\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\npacketRate\x18\x0c \x01(\x03\x12\x10\n\x08\x64\x61taRate\x18\r \x01(\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"\xb3\x01\n\nStatistics\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x07 \x01(\t\x12=\n\x07tmstats\x18\x03 \x03(\x0b\x32,.yamcs.protobuf.yamcsManagement.TmStatistics\x12/\n\x0blastUpdated\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampJ\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"\x8b\x02\n\x1aProcessorManagementRequest\x12W\n\toperation\x18\x01 \x01(\x0e\x32\x44.yamcs.protobuf.yamcsManagement.ProcessorManagementRequest.Operation\x12\x10\n\x08instance\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x0e\n\x06\x63onfig\x18\x05 \x01(\t\x12\x19\n\npersistent\x18\x07 \x01(\x08:\x05\x66\x61lse\";\n\tOperation\x12\x14\n\x10\x43REATE_PROCESSOR\x10\x00\x12\x18\n\x14\x43ONNECT_TO_PROCESSOR\x10\x01\"\x85\x02\n\x10ProcessorRequest\x12M\n\toperation\x18\x01 \x01(\x0e\x32:.yamcs.protobuf.yamcsManagement.ProcessorRequest.Operation\x12\x10\n\x08instance\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08seekTime\x18\x04 \x01(\x03\x12\x30\n\x0breplaySpeed\x18\x05 \x01(\x0b\x32\x1b.yamcs.protobuf.ReplaySpeed\">\n\tOperation\x12\t\n\x05PAUSE\x10\x02\x12\n\n\x06RESUME\x10\x03\x12\x08\n\x04SEEK\x10\x04\x12\x10\n\x0c\x43HANGE_SPEED\x10\x05\"\x90\x01\n\x0bServiceInfo\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12;\n\x05state\x18\x03 \x01(\x0e\x32,.yamcs.protobuf.yamcsManagement.ServiceState\x12\x11\n\tclassName\x18\x04 \x01(\t\x12\x11\n\tprocessor\x18\x05 \x01(\t\"\x9d\x01\n\x0bStreamEvent\x12>\n\x04type\x18\x01 \x01(\x0e\x32\x30.yamcs.protobuf.yamcsManagement.StreamEvent.Type\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\tdataCount\x18\x03 \x01(\x03\"-\n\x04Type\x12\x0b\n\x07\x43REATED\x10\x01\x12\x0b\n\x07\x44\x45LETED\x10\x02\x12\x0b\n\x07UPDATED\x10\x03\"\xbe\x04\n\nSystemInfo\x12\x14\n\x0cyamcsVersion\x18\x01 \x01(\t\x12\x10\n\x08revision\x18\x02 \x01(\t\x12\x10\n\x08serverId\x18\x03 \x01(\t\x12\x0e\n\x06uptime\x18\x05 \x01(\x03\x12\x0b\n\x03jvm\x18\x06 \x01(\t\x12\x18\n\x10workingDirectory\x18\x07 \x01(\t\x12\x17\n\x0f\x63onfigDirectory\x18\x08 \x01(\t\x12\x15\n\rdataDirectory\x18\t \x01(\t\x12\x16\n\x0e\x63\x61\x63heDirectory\x18\n \x01(\t\x12\n\n\x02os\x18\x0b \x01(\t\x12\x0c\n\x04\x61rch\x18\x0c \x01(\t\x12\x1b\n\x13\x61vailableProcessors\x18\r \x01(\x05\x12\x13\n\x0bloadAverage\x18\x0e \x01(\x01\x12\x12\n\nheapMemory\x18\x0f \x01(\x03\x12\x16\n\x0eusedHeapMemory\x18\x10 \x01(\x03\x12\x15\n\rmaxHeapMemory\x18\x11 \x01(\x03\x12\x15\n\rnonHeapMemory\x18\x12 \x01(\x03\x12\x19\n\x11usedNonHeapMemory\x18\x13 \x01(\x03\x12\x18\n\x10maxNonHeapMemory\x18\x14 \x01(\x03\x12\x16\n\x0ejvmThreadCount\x18\x15 \x01(\x03\x12\x46\n\x0frootDirectories\x18\x16 \x03(\x0b\x32-.yamcs.protobuf.yamcsManagement.RootDirectory\x12<\n\x07process\x18\x17 \x01(\x0b\x32+.yamcs.protobuf.yamcsManagement.ProcessInfo\"\xef\x01\n\x0bProcessInfo\x12\x0b\n\x03pid\x18\x01 \x01(\x03\x12\x0c\n\x04user\x18\x02 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\t\x12\x11\n\targuments\x18\x04 \x03(\t\x12-\n\tstartTime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x10totalCpuDuration\x18\x06 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x08\x63hildren\x18\x07 \x03(\x0b\x32+.yamcs.protobuf.yamcsManagement.ProcessInfo\"s\n\rRootDirectory\x12\x11\n\tdirectory\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x12\n\ntotalSpace\x18\x03 \x01(\x03\x12\x18\n\x10unallocatedSpace\x18\x04 \x01(\x03\x12\x13\n\x0busableSpace\x18\x05 \x01(\x03\"\'\n\x13ListServicesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"3\n\x11GetServiceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"5\n\x13StartServiceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"4\n\x12StopServiceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"U\n\x14ListServicesResponse\x12=\n\x08services\x18\x01 \x03(\x0b\x32+.yamcs.protobuf.yamcsManagement.ServiceInfo\"&\n\x14ListInstancesRequest\x12\x0e\n\x06\x66ilter\x18\x01 \x03(\t\"Y\n\x15ListInstancesResponse\x12@\n\tinstances\x18\x01 \x03(\x0b\x32-.yamcs.protobuf.yamcsManagement.YamcsInstance\"\xcd\x02\n\x15\x43reateInstanceRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08template\x18\x02 \x01(\t\x12]\n\x0ctemplateArgs\x18\x03 \x03(\x0b\x32G.yamcs.protobuf.yamcsManagement.CreateInstanceRequest.TemplateArgsEntry\x12Q\n\x06labels\x18\x04 \x03(\x0b\x32\x41.yamcs.protobuf.yamcsManagement.CreateInstanceRequest.LabelsEntry\x1a\x33\n\x11TemplateArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xce\x02\n\x1aReconfigureInstanceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x62\n\x0ctemplateArgs\x18\x02 \x03(\x0b\x32L.yamcs.protobuf.yamcsManagement.ReconfigureInstanceRequest.TemplateArgsEntry\x12V\n\x06labels\x18\x03 \x03(\x0b\x32\x46.yamcs.protobuf.yamcsManagement.ReconfigureInstanceRequest.LabelsEntry\x1a\x33\n\x11TemplateArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x1dListInstanceTemplatesResponse\x12\x43\n\ttemplates\x18\x01 \x03(\x0b\x32\x30.yamcs.protobuf.yamcsManagement.InstanceTemplate\"6\n\x13\x45\x64itInstanceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\r\n\x05state\x18\x02 \x01(\t\".\n\x1aGetInstanceTemplateRequest\x12\x10\n\x08template\x18\x01 \x01(\t\"&\n\x12GetInstanceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"(\n\x14StartInstanceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"\'\n\x13StopInstanceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"*\n\x16RestartInstanceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t*\\\n\x0cServiceState\x12\x07\n\x03NEW\x10\x00\x12\x0c\n\x08STARTING\x10\x01\x12\x0b\n\x07RUNNING\x10\x02\x12\x0c\n\x08STOPPING\x10\x03\x12\x0e\n\nTERMINATED\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x32\xa4\x12\n\rManagementApi\x12g\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a*.yamcs.protobuf.yamcsManagement.SystemInfo\"\x12\x8a\x92\x03\x0e\n\x0c/api/sysinfo\x12j\n\x13SubscribeSystemInfo\x12\x16.google.protobuf.Empty\x1a*.yamcs.protobuf.yamcsManagement.SystemInfo\"\r\xda\x92\x03\t\n\x07sysinfo0\x01\x12\x8d\x01\n\x15ListInstanceTemplates\x12\x16.google.protobuf.Empty\x1a=.yamcs.protobuf.yamcsManagement.ListInstanceTemplatesResponse\"\x1d\x8a\x92\x03\x19\n\x17/api/instance-templates\x12\xad\x01\n\x13GetInstanceTemplate\x12:.yamcs.protobuf.yamcsManagement.GetInstanceTemplateRequest\x1a\x30.yamcs.protobuf.yamcsManagement.InstanceTemplate\"(\x8a\x92\x03$\n\"/api/instance-templates/{template}\x12\x92\x01\n\rListInstances\x12\x34.yamcs.protobuf.yamcsManagement.ListInstancesRequest\x1a\x35.yamcs.protobuf.yamcsManagement.ListInstancesResponse\"\x14\x8a\x92\x03\x10\n\x0e/api/instances\x12n\n\x12SubscribeInstances\x12\x16.google.protobuf.Empty\x1a-.yamcs.protobuf.yamcsManagement.YamcsInstance\"\x0f\xda\x92\x03\x0b\n\tinstances0\x01\x12\x91\x01\n\x0bGetInstance\x12\x32.yamcs.protobuf.yamcsManagement.GetInstanceRequest\x1a-.yamcs.protobuf.yamcsManagement.YamcsInstance\"\x1f\x8a\x92\x03\x1b\n\x19/api/instances/{instance}\x12\x8f\x01\n\x0e\x43reateInstance\x12\x35.yamcs.protobuf.yamcsManagement.CreateInstanceRequest\x1a-.yamcs.protobuf.yamcsManagement.YamcsInstance\"\x17\x8a\x92\x03\x13\x1a\x0e/api/instances:\x01*\x12\xb0\x01\n\x13ReconfigureInstance\x12:.yamcs.protobuf.yamcsManagement.ReconfigureInstanceRequest\x1a-.yamcs.protobuf.yamcsManagement.YamcsInstance\".\x8a\x92\x03*\x1a%/api/instances/{instance}:reconfigure:\x01*\x12\x9b\x01\n\rStartInstance\x12\x34.yamcs.protobuf.yamcsManagement.StartInstanceRequest\x1a-.yamcs.protobuf.yamcsManagement.YamcsInstance\"%\x8a\x92\x03!\x1a\x1f/api/instances/{instance}:start\x12\x98\x01\n\x0cStopInstance\x12\x33.yamcs.protobuf.yamcsManagement.StopInstanceRequest\x1a-.yamcs.protobuf.yamcsManagement.YamcsInstance\"$\x8a\x92\x03 \x1a\x1e/api/instances/{instance}:stop\x12\xa1\x01\n\x0fRestartInstance\x12\x36.yamcs.protobuf.yamcsManagement.RestartInstanceRequest\x1a-.yamcs.protobuf.yamcsManagement.YamcsInstance\"\'\x8a\x92\x03#\x1a!/api/instances/{instance}:restart\x12\x99\x01\n\x0cListServices\x12\x33.yamcs.protobuf.yamcsManagement.ListServicesRequest\x1a\x34.yamcs.protobuf.yamcsManagement.ListServicesResponse\"\x1e\x8a\x92\x03\x1a\n\x18/api/services/{instance}\x12\x93\x01\n\nGetService\x12\x31.yamcs.protobuf.yamcsManagement.GetServiceRequest\x1a+.yamcs.protobuf.yamcsManagement.ServiceInfo\"%\x8a\x92\x03!\n\x1f/api/services/{instance}/{name}\x12\x88\x01\n\x0cStartService\x12\x33.yamcs.protobuf.yamcsManagement.StartServiceRequest\x1a\x16.google.protobuf.Empty\"+\x8a\x92\x03\'\x1a%/api/services/{instance}/{name}:start\x12\x85\x01\n\x0bStopService\x12\x32.yamcs.protobuf.yamcsManagement.StopServiceRequest\x1a\x16.google.protobuf.Empty\"*\x8a\x92\x03&\x1a$/api/services/{instance}/{name}:stopB,\n\x12org.yamcs.protobufB\x14YamcsManagementProtoP\x01')
+  serialized_pb=_b('\n4yamcs/protobuf/yamcsManagement/yamcsManagement.proto\x12\x1eyamcs.protobuf.yamcsManagement\x1a\x1egoogle/protobuf/duration.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1byamcs/api/annotations.proto\x1a\x1ayamcs/protobuf/yamcs.proto\x1a\x1cyamcs/protobuf/mdb/mdb.proto\"R\n\x0eYamcsInstances\x12@\n\tinstances\x18\x01 \x03(\x0b\x32-.yamcs.protobuf.yamcsManagement.YamcsInstance\"\x89\x06\n\rYamcsInstance\x12\x0c\n\x04name\x18\x01 \x01(\t\x12<\n\x0fmissionDatabase\x18\x03 \x01(\x0b\x32#.yamcs.protobuf.mdb.MissionDatabase\x12\x41\n\nprocessors\x18\x04 \x03(\x0b\x32-.yamcs.protobuf.yamcsManagement.ProcessorInfo\x12J\n\x05state\x18\x0b \x01(\x0e\x32;.yamcs.protobuf.yamcsManagement.YamcsInstance.InstanceState\x12\x14\n\x0c\x66\x61ilureCause\x18\t \x01(\t\x12/\n\x0bmissionTime\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x06labels\x18\x0c \x03(\x0b\x32\x39.yamcs.protobuf.yamcsManagement.YamcsInstance.LabelsEntry\x12\x14\n\x0c\x63\x61pabilities\x18\r \x03(\t\x12\x10\n\x08template\x18\x0e \x01(\t\x12U\n\x0ctemplateArgs\x18\x0f \x03(\x0b\x32?.yamcs.protobuf.yamcsManagement.YamcsInstance.TemplateArgsEntry\x12\x19\n\x11templateAvailable\x18\x10 \x01(\x08\x12\x17\n\x0ftemplateChanged\x18\x11 \x01(\x08\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x33\n\x11TemplateArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"t\n\rInstanceState\x12\x0b\n\x07OFFLINE\x10\x00\x12\x10\n\x0cINITIALIZING\x10\x01\x12\x0f\n\x0bINITIALIZED\x10\x02\x12\x0c\n\x08STARTING\x10\x03\x12\x0b\n\x07RUNNING\x10\x04\x12\x0c\n\x08STOPPING\x10\x05\x12\n\n\x06\x46\x41ILED\x10\x06\"z\n\x10InstanceTemplate\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x43\n\tvariables\x18\x02 \x03(\x0b\x32\x30.yamcs.protobuf.yamcsManagement.TemplateVariable\"\x7f\n\x10TemplateVariable\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05label\x18\x06 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x0c\n\x04help\x18\x02 \x01(\t\x12\x10\n\x08required\x18\x03 \x01(\x08\x12\x0f\n\x07\x63hoices\x18\x05 \x03(\t\x12\x0f\n\x07initial\x18\x07 \x01(\t\"\xc4\x04\n\rProcessorInfo\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04spec\x18\x04 \x01(\t\x12\x0f\n\x07\x63reator\x18\x05 \x01(\t\x12\x11\n\thasAlarms\x18\x06 \x01(\x08\x12\x15\n\rhasCommanding\x18\x07 \x01(\x08\x12;\n\x05state\x18\x08 \x01(\x0e\x32,.yamcs.protobuf.yamcsManagement.ServiceState\x12\x34\n\rreplayRequest\x18\t \x01(\x0b\x32\x1d.yamcs.protobuf.ReplayRequest\x12=\n\x0breplayState\x18\n \x01(\x0e\x32(.yamcs.protobuf.ReplayStatus.ReplayState\x12=\n\x08services\x18\x10 \x03(\x0b\x32+.yamcs.protobuf.yamcsManagement.ServiceInfo\x12\x12\n\npersistent\x18\x11 \x01(\x08\x12(\n\x04time\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06replay\x18\x13 \x01(\x08\x12\x1d\n\x15\x63heckCommandClearance\x18\x14 \x01(\x08\x12\x11\n\tprotected\x18\x15 \x01(\x08\x12K\n\x0f\x61\x63knowledgments\x18\x16 \x03(\x0b\x32\x32.yamcs.protobuf.yamcsManagement.AcknowledgmentInfo\"7\n\x12\x41\x63knowledgmentInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"\x98\x02\n\x0cTmStatistics\x12\x12\n\npacketName\x18\x01 \x01(\t\x12\x15\n\rqualifiedName\x18\t \x01(\t\x12\x17\n\x0freceivedPackets\x18\x02 \x01(\x03\x12 \n\x18subscribedParameterCount\x18\x06 \x01(\x05\x12\x30\n\x0clastReceived\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0elastPacketTime\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\npacketRate\x18\x0c \x01(\x03\x12\x10\n\x08\x64\x61taRate\x18\r \x01(\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\t\"\xb3\x01\n\nStatistics\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x11\n\tprocessor\x18\x07 \x01(\t\x12=\n\x07tmstats\x18\x03 \x03(\x0b\x32,.yamcs.protobuf.yamcsManagement.TmStatistics\x12/\n\x0blastUpdated\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampJ\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"\x8b\x02\n\x1aProcessorManagementRequest\x12W\n\toperation\x18\x01 \x01(\x0e\x32\x44.yamcs.protobuf.yamcsManagement.ProcessorManagementRequest.Operation\x12\x10\n\x08instance\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\x12\x0e\n\x06\x63onfig\x18\x05 \x01(\t\x12\x19\n\npersistent\x18\x07 \x01(\x08:\x05\x66\x61lse\";\n\tOperation\x12\x14\n\x10\x43REATE_PROCESSOR\x10\x00\x12\x18\n\x14\x43ONNECT_TO_PROCESSOR\x10\x01\"\x85\x02\n\x10ProcessorRequest\x12M\n\toperation\x18\x01 \x01(\x0e\x32:.yamcs.protobuf.yamcsManagement.ProcessorRequest.Operation\x12\x10\n\x08instance\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08seekTime\x18\x04 \x01(\x03\x12\x30\n\x0breplaySpeed\x18\x05 \x01(\x0b\x32\x1b.yamcs.protobuf.ReplaySpeed\">\n\tOperation\x12\t\n\x05PAUSE\x10\x02\x12\n\n\x06RESUME\x10\x03\x12\x08\n\x04SEEK\x10\x04\x12\x10\n\x0c\x43HANGE_SPEED\x10\x05\"\xbe\x01\n\x0bServiceInfo\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12;\n\x05state\x18\x03 \x01(\x0e\x32,.yamcs.protobuf.yamcsManagement.ServiceState\x12\x11\n\tclassName\x18\x04 \x01(\t\x12\x11\n\tprocessor\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x14\n\x0c\x66\x61ilureCause\x18\x07 \x01(\t\"\x9d\x01\n\x0bStreamEvent\x12>\n\x04type\x18\x01 \x01(\x0e\x32\x30.yamcs.protobuf.yamcsManagement.StreamEvent.Type\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\tdataCount\x18\x03 \x01(\x03\"-\n\x04Type\x12\x0b\n\x07\x43REATED\x10\x01\x12\x0b\n\x07\x44\x45LETED\x10\x02\x12\x0b\n\x07UPDATED\x10\x03\"\xbe\x04\n\nSystemInfo\x12\x14\n\x0cyamcsVersion\x18\x01 \x01(\t\x12\x10\n\x08revision\x18\x02 \x01(\t\x12\x10\n\x08serverId\x18\x03 \x01(\t\x12\x0e\n\x06uptime\x18\x05 \x01(\x03\x12\x0b\n\x03jvm\x18\x06 \x01(\t\x12\x18\n\x10workingDirectory\x18\x07 \x01(\t\x12\x17\n\x0f\x63onfigDirectory\x18\x08 \x01(\t\x12\x15\n\rdataDirectory\x18\t \x01(\t\x12\x16\n\x0e\x63\x61\x63heDirectory\x18\n \x01(\t\x12\n\n\x02os\x18\x0b \x01(\t\x12\x0c\n\x04\x61rch\x18\x0c \x01(\t\x12\x1b\n\x13\x61vailableProcessors\x18\r \x01(\x05\x12\x13\n\x0bloadAverage\x18\x0e \x01(\x01\x12\x12\n\nheapMemory\x18\x0f \x01(\x03\x12\x16\n\x0eusedHeapMemory\x18\x10 \x01(\x03\x12\x15\n\rmaxHeapMemory\x18\x11 \x01(\x03\x12\x15\n\rnonHeapMemory\x18\x12 \x01(\x03\x12\x19\n\x11usedNonHeapMemory\x18\x13 \x01(\x03\x12\x18\n\x10maxNonHeapMemory\x18\x14 \x01(\x03\x12\x16\n\x0ejvmThreadCount\x18\x15 \x01(\x03\x12\x46\n\x0frootDirectories\x18\x16 \x03(\x0b\x32-.yamcs.protobuf.yamcsManagement.RootDirectory\x12<\n\x07process\x18\x17 \x01(\x0b\x32+.yamcs.protobuf.yamcsManagement.ProcessInfo\"\xef\x01\n\x0bProcessInfo\x12\x0b\n\x03pid\x18\x01 \x01(\x03\x12\x0c\n\x04user\x18\x02 \x01(\t\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\t\x12\x11\n\targuments\x18\x04 \x03(\t\x12-\n\tstartTime\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x10totalCpuDuration\x18\x06 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x08\x63hildren\x18\x07 \x03(\x0b\x32+.yamcs.protobuf.yamcsManagement.ProcessInfo\"s\n\rRootDirectory\x12\x11\n\tdirectory\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x12\n\ntotalSpace\x18\x03 \x01(\x03\x12\x18\n\x10unallocatedSpace\x18\x04 \x01(\x03\x12\x13\n\x0busableSpace\x18\x05 \x01(\x03\"\'\n\x13ListServicesRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"3\n\x11GetServiceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"5\n\x13StartServiceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"4\n\x12StopServiceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"U\n\x14ListServicesResponse\x12=\n\x08services\x18\x01 \x03(\x0b\x32+.yamcs.protobuf.yamcsManagement.ServiceInfo\"&\n\x14ListInstancesRequest\x12\x0e\n\x06\x66ilter\x18\x01 \x03(\t\"Y\n\x15ListInstancesResponse\x12@\n\tinstances\x18\x01 \x03(\x0b\x32-.yamcs.protobuf.yamcsManagement.YamcsInstance\"\xcd\x02\n\x15\x43reateInstanceRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08template\x18\x02 \x01(\t\x12]\n\x0ctemplateArgs\x18\x03 \x03(\x0b\x32G.yamcs.protobuf.yamcsManagement.CreateInstanceRequest.TemplateArgsEntry\x12Q\n\x06labels\x18\x04 \x03(\x0b\x32\x41.yamcs.protobuf.yamcsManagement.CreateInstanceRequest.LabelsEntry\x1a\x33\n\x11TemplateArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xce\x02\n\x1aReconfigureInstanceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\x62\n\x0ctemplateArgs\x18\x02 \x03(\x0b\x32L.yamcs.protobuf.yamcsManagement.ReconfigureInstanceRequest.TemplateArgsEntry\x12V\n\x06labels\x18\x03 \x03(\x0b\x32\x46.yamcs.protobuf.yamcsManagement.ReconfigureInstanceRequest.LabelsEntry\x1a\x33\n\x11TemplateArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x1dListInstanceTemplatesResponse\x12\x43\n\ttemplates\x18\x01 \x03(\x0b\x32\x30.yamcs.protobuf.yamcsManagement.InstanceTemplate\"6\n\x13\x45\x64itInstanceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\x12\r\n\x05state\x18\x02 \x01(\t\".\n\x1aGetInstanceTemplateRequest\x12\x10\n\x08template\x18\x01 \x01(\t\"&\n\x12GetInstanceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"(\n\x14StartInstanceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"\'\n\x13StopInstanceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t\"*\n\x16RestartInstanceRequest\x12\x10\n\x08instance\x18\x01 \x01(\t*\\\n\x0cServiceState\x12\x07\n\x03NEW\x10\x00\x12\x0c\n\x08STARTING\x10\x01\x12\x0b\n\x07RUNNING\x10\x02\x12\x0c\n\x08STOPPING\x10\x03\x12\x0e\n\nTERMINATED\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x32\xa4\x12\n\rManagementApi\x12g\n\rGetSystemInfo\x12\x16.google.protobuf.Empty\x1a*.yamcs.protobuf.yamcsManagement.SystemInfo\"\x12\x8a\x92\x03\x0e\n\x0c/api/sysinfo\x12j\n\x13SubscribeSystemInfo\x12\x16.google.protobuf.Empty\x1a*.yamcs.protobuf.yamcsManagement.SystemInfo\"\r\xda\x92\x03\t\n\x07sysinfo0\x01\x12\x8d\x01\n\x15ListInstanceTemplates\x12\x16.google.protobuf.Empty\x1a=.yamcs.protobuf.yamcsManagement.ListInstanceTemplatesResponse\"\x1d\x8a\x92\x03\x19\n\x17/api/instance-templates\x12\xad\x01\n\x13GetInstanceTemplate\x12:.yamcs.protobuf.yamcsManagement.GetInstanceTemplateRequest\x1a\x30.yamcs.protobuf.yamcsManagement.InstanceTemplate\"(\x8a\x92\x03$\n\"/api/instance-templates/{template}\x12\x92\x01\n\rListInstances\x12\x34.yamcs.protobuf.yamcsManagement.ListInstancesRequest\x1a\x35.yamcs.protobuf.yamcsManagement.ListInstancesResponse\"\x14\x8a\x92\x03\x10\n\x0e/api/instances\x12n\n\x12SubscribeInstances\x12\x16.google.protobuf.Empty\x1a-.yamcs.protobuf.yamcsManagement.YamcsInstance\"\x0f\xda\x92\x03\x0b\n\tinstances0\x01\x12\x91\x01\n\x0bGetInstance\x12\x32.yamcs.protobuf.yamcsManagement.GetInstanceRequest\x1a-.yamcs.protobuf.yamcsManagement.YamcsInstance\"\x1f\x8a\x92\x03\x1b\n\x19/api/instances/{instance}\x12\x8f\x01\n\x0e\x43reateInstance\x12\x35.yamcs.protobuf.yamcsManagement.CreateInstanceRequest\x1a-.yamcs.protobuf.yamcsManagement.YamcsInstance\"\x17\x8a\x92\x03\x13\x1a\x0e/api/instances:\x01*\x12\xb0\x01\n\x13ReconfigureInstance\x12:.yamcs.protobuf.yamcsManagement.ReconfigureInstanceRequest\x1a-.yamcs.protobuf.yamcsManagement.YamcsInstance\".\x8a\x92\x03*\x1a%/api/instances/{instance}:reconfigure:\x01*\x12\x9b\x01\n\rStartInstance\x12\x34.yamcs.protobuf.yamcsManagement.StartInstanceRequest\x1a-.yamcs.protobuf.yamcsManagement.YamcsInstance\"%\x8a\x92\x03!\x1a\x1f/api/instances/{instance}:start\x12\x98\x01\n\x0cStopInstance\x12\x33.yamcs.protobuf.yamcsManagement.StopInstanceRequest\x1a-.yamcs.protobuf.yamcsManagement.YamcsInstance\"$\x8a\x92\x03 \x1a\x1e/api/instances/{instance}:stop\x12\xa1\x01\n\x0fRestartInstance\x12\x36.yamcs.protobuf.yamcsManagement.RestartInstanceRequest\x1a-.yamcs.protobuf.yamcsManagement.YamcsInstance\"\'\x8a\x92\x03#\x1a!/api/instances/{instance}:restart\x12\x99\x01\n\x0cListServices\x12\x33.yamcs.protobuf.yamcsManagement.ListServicesRequest\x1a\x34.yamcs.protobuf.yamcsManagement.ListServicesResponse\"\x1e\x8a\x92\x03\x1a\n\x18/api/services/{instance}\x12\x93\x01\n\nGetService\x12\x31.yamcs.protobuf.yamcsManagement.GetServiceRequest\x1a+.yamcs.protobuf.yamcsManagement.ServiceInfo\"%\x8a\x92\x03!\n\x1f/api/services/{instance}/{name}\x12\x88\x01\n\x0cStartService\x12\x33.yamcs.protobuf.yamcsManagement.StartServiceRequest\x1a\x16.google.protobuf.Empty\"+\x8a\x92\x03\'\x1a%/api/services/{instance}/{name}:start\x12\x85\x01\n\x0bStopService\x12\x32.yamcs.protobuf.yamcsManagement.StopServiceRequest\x1a\x16.google.protobuf.Empty\"*\x8a\x92\x03&\x1a$/api/services/{instance}/{name}:stopB,\n\x12org.yamcs.protobufB\x14YamcsManagementProtoP\x01')
   ,
   dependencies=[google_dot_protobuf_dot_duration__pb2.DESCRIPTOR,google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,yamcs_dot_api_dot_annotations__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_yamcs__pb2.DESCRIPTOR,yamcs_dot_protobuf_dot_mdb_dot_mdb__pb2.DESCRIPTOR,])
 
 _SERVICESTATE = _descriptor.EnumDescriptor(
   name='ServiceState',
   full_name='yamcs.protobuf.yamcsManagement.ServiceState',
   filename=None,
@@ -60,16 +60,16 @@
     _descriptor.EnumValueDescriptor(
       name='FAILED', index=5, number=5,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=5601,
-  serialized_end=5693,
+  serialized_start=5781,
+  serialized_end=5873,
 )
 _sym_db.RegisterEnumDescriptor(_SERVICESTATE)
 
 ServiceState = enum_type_wrapper.EnumTypeWrapper(_SERVICESTATE)
 NEW = 0
 STARTING = 1
 RUNNING = 2
@@ -133,16 +133,16 @@
     _descriptor.EnumValueDescriptor(
       name='CONNECT_TO_PROCESSOR', index=1, number=1,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2566,
-  serialized_end=2625,
+  serialized_start=2700,
+  serialized_end=2759,
 )
 _sym_db.RegisterEnumDescriptor(_PROCESSORMANAGEMENTREQUEST_OPERATION)
 
 _PROCESSORREQUEST_OPERATION = _descriptor.EnumDescriptor(
   name='Operation',
   full_name='yamcs.protobuf.yamcsManagement.ProcessorRequest.Operation',
   filename=None,
@@ -163,16 +163,16 @@
     _descriptor.EnumValueDescriptor(
       name='CHANGE_SPEED', index=3, number=5,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2827,
-  serialized_end=2889,
+  serialized_start=2961,
+  serialized_end=3023,
 )
 _sym_db.RegisterEnumDescriptor(_PROCESSORREQUEST_OPERATION)
 
 _STREAMEVENT_TYPE = _descriptor.EnumDescriptor(
   name='Type',
   full_name='yamcs.protobuf.yamcsManagement.StreamEvent.Type',
   filename=None,
@@ -189,16 +189,16 @@
     _descriptor.EnumValueDescriptor(
       name='UPDATED', index=2, number=3,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3151,
-  serialized_end=3196,
+  serialized_start=3331,
+  serialized_end=3376,
 )
 _sym_db.RegisterEnumDescriptor(_STREAMEVENT_TYPE)
 
 
 _YAMCSINSTANCES = _descriptor.Descriptor(
   name='YamcsInstances',
   full_name='yamcs.protobuf.yamcsManagement.YamcsInstances',
@@ -646,28 +646,73 @@
     _descriptor.FieldDescriptor(
       name='protected', full_name='yamcs.protobuf.yamcsManagement.ProcessorInfo.protected', index=15,
       number=21, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='acknowledgments', full_name='yamcs.protobuf.yamcsManagement.ProcessorInfo.acknowledgments', index=16,
+      number=22, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=1387,
-  serialized_end=1890,
+  serialized_end=1967,
+)
+
+
+_ACKNOWLEDGMENTINFO = _descriptor.Descriptor(
+  name='AcknowledgmentInfo',
+  full_name='yamcs.protobuf.yamcsManagement.AcknowledgmentInfo',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='name', full_name='yamcs.protobuf.yamcsManagement.AcknowledgmentInfo.name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='description', full_name='yamcs.protobuf.yamcsManagement.AcknowledgmentInfo.description', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto2',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1969,
+  serialized_end=2024,
 )
 
 
 _TMSTATISTICS = _descriptor.Descriptor(
   name='TmStatistics',
   full_name='yamcs.protobuf.yamcsManagement.TmStatistics',
   filename=None,
@@ -738,16 +783,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1893,
-  serialized_end=2173,
+  serialized_start=2027,
+  serialized_end=2307,
 )
 
 
 _STATISTICS = _descriptor.Descriptor(
   name='Statistics',
   full_name='yamcs.protobuf.yamcsManagement.Statistics',
   filename=None,
@@ -790,16 +835,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2176,
-  serialized_end=2355,
+  serialized_start=2310,
+  serialized_end=2489,
 )
 
 
 _PROCESSORMANAGEMENTREQUEST = _descriptor.Descriptor(
   name='ProcessorManagementRequest',
   full_name='yamcs.protobuf.yamcsManagement.ProcessorManagementRequest',
   filename=None,
@@ -857,16 +902,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2358,
-  serialized_end=2625,
+  serialized_start=2492,
+  serialized_end=2759,
 )
 
 
 _PROCESSORREQUEST = _descriptor.Descriptor(
   name='ProcessorRequest',
   full_name='yamcs.protobuf.yamcsManagement.ProcessorRequest',
   filename=None,
@@ -917,16 +962,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2628,
-  serialized_end=2889,
+  serialized_start=2762,
+  serialized_end=3023,
 )
 
 
 _SERVICEINFO = _descriptor.Descriptor(
   name='ServiceInfo',
   full_name='yamcs.protobuf.yamcsManagement.ServiceInfo',
   filename=None,
@@ -964,28 +1009,42 @@
     _descriptor.FieldDescriptor(
       name='processor', full_name='yamcs.protobuf.yamcsManagement.ServiceInfo.processor', index=4,
       number=5, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='failureMessage', full_name='yamcs.protobuf.yamcsManagement.ServiceInfo.failureMessage', index=5,
+      number=6, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='failureCause', full_name='yamcs.protobuf.yamcsManagement.ServiceInfo.failureCause', index=6,
+      number=7, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2892,
-  serialized_end=3036,
+  serialized_start=3026,
+  serialized_end=3216,
 )
 
 
 _STREAMEVENT = _descriptor.Descriptor(
   name='StreamEvent',
   full_name='yamcs.protobuf.yamcsManagement.StreamEvent',
   filename=None,
@@ -1022,16 +1081,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3039,
-  serialized_end=3196,
+  serialized_start=3219,
+  serialized_end=3376,
 )
 
 
 _SYSTEMINFO = _descriptor.Descriptor(
   name='SystemInfo',
   full_name='yamcs.protobuf.yamcsManagement.SystemInfo',
   filename=None,
@@ -1200,16 +1259,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3199,
-  serialized_end=3773,
+  serialized_start=3379,
+  serialized_end=3953,
 )
 
 
 _PROCESSINFO = _descriptor.Descriptor(
   name='ProcessInfo',
   full_name='yamcs.protobuf.yamcsManagement.ProcessInfo',
   filename=None,
@@ -1273,16 +1332,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3776,
-  serialized_end=4015,
+  serialized_start=3956,
+  serialized_end=4195,
 )
 
 
 _ROOTDIRECTORY = _descriptor.Descriptor(
   name='RootDirectory',
   full_name='yamcs.protobuf.yamcsManagement.RootDirectory',
   filename=None,
@@ -1332,16 +1391,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4017,
-  serialized_end=4132,
+  serialized_start=4197,
+  serialized_end=4312,
 )
 
 
 _LISTSERVICESREQUEST = _descriptor.Descriptor(
   name='ListServicesRequest',
   full_name='yamcs.protobuf.yamcsManagement.ListServicesRequest',
   filename=None,
@@ -1363,16 +1422,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4134,
-  serialized_end=4173,
+  serialized_start=4314,
+  serialized_end=4353,
 )
 
 
 _GETSERVICEREQUEST = _descriptor.Descriptor(
   name='GetServiceRequest',
   full_name='yamcs.protobuf.yamcsManagement.GetServiceRequest',
   filename=None,
@@ -1401,16 +1460,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4175,
-  serialized_end=4226,
+  serialized_start=4355,
+  serialized_end=4406,
 )
 
 
 _STARTSERVICEREQUEST = _descriptor.Descriptor(
   name='StartServiceRequest',
   full_name='yamcs.protobuf.yamcsManagement.StartServiceRequest',
   filename=None,
@@ -1439,16 +1498,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4228,
-  serialized_end=4281,
+  serialized_start=4408,
+  serialized_end=4461,
 )
 
 
 _STOPSERVICEREQUEST = _descriptor.Descriptor(
   name='StopServiceRequest',
   full_name='yamcs.protobuf.yamcsManagement.StopServiceRequest',
   filename=None,
@@ -1477,16 +1536,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4283,
-  serialized_end=4335,
+  serialized_start=4463,
+  serialized_end=4515,
 )
 
 
 _LISTSERVICESRESPONSE = _descriptor.Descriptor(
   name='ListServicesResponse',
   full_name='yamcs.protobuf.yamcsManagement.ListServicesResponse',
   filename=None,
@@ -1508,16 +1567,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4337,
-  serialized_end=4422,
+  serialized_start=4517,
+  serialized_end=4602,
 )
 
 
 _LISTINSTANCESREQUEST = _descriptor.Descriptor(
   name='ListInstancesRequest',
   full_name='yamcs.protobuf.yamcsManagement.ListInstancesRequest',
   filename=None,
@@ -1539,16 +1598,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4424,
-  serialized_end=4462,
+  serialized_start=4604,
+  serialized_end=4642,
 )
 
 
 _LISTINSTANCESRESPONSE = _descriptor.Descriptor(
   name='ListInstancesResponse',
   full_name='yamcs.protobuf.yamcsManagement.ListInstancesResponse',
   filename=None,
@@ -1570,16 +1629,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4464,
-  serialized_end=4553,
+  serialized_start=4644,
+  serialized_end=4733,
 )
 
 
 _CREATEINSTANCEREQUEST_TEMPLATEARGSENTRY = _descriptor.Descriptor(
   name='TemplateArgsEntry',
   full_name='yamcs.protobuf.yamcsManagement.CreateInstanceRequest.TemplateArgsEntry',
   filename=None,
@@ -1696,16 +1755,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4556,
-  serialized_end=4889,
+  serialized_start=4736,
+  serialized_end=5069,
 )
 
 
 _RECONFIGUREINSTANCEREQUEST_TEMPLATEARGSENTRY = _descriptor.Descriptor(
   name='TemplateArgsEntry',
   full_name='yamcs.protobuf.yamcsManagement.ReconfigureInstanceRequest.TemplateArgsEntry',
   filename=None,
@@ -1815,16 +1874,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4892,
-  serialized_end=5226,
+  serialized_start=5072,
+  serialized_end=5406,
 )
 
 
 _LISTINSTANCETEMPLATESRESPONSE = _descriptor.Descriptor(
   name='ListInstanceTemplatesResponse',
   full_name='yamcs.protobuf.yamcsManagement.ListInstanceTemplatesResponse',
   filename=None,
@@ -1846,16 +1905,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5228,
-  serialized_end=5328,
+  serialized_start=5408,
+  serialized_end=5508,
 )
 
 
 _EDITINSTANCEREQUEST = _descriptor.Descriptor(
   name='EditInstanceRequest',
   full_name='yamcs.protobuf.yamcsManagement.EditInstanceRequest',
   filename=None,
@@ -1884,16 +1943,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5330,
-  serialized_end=5384,
+  serialized_start=5510,
+  serialized_end=5564,
 )
 
 
 _GETINSTANCETEMPLATEREQUEST = _descriptor.Descriptor(
   name='GetInstanceTemplateRequest',
   full_name='yamcs.protobuf.yamcsManagement.GetInstanceTemplateRequest',
   filename=None,
@@ -1915,16 +1974,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5386,
-  serialized_end=5432,
+  serialized_start=5566,
+  serialized_end=5612,
 )
 
 
 _GETINSTANCEREQUEST = _descriptor.Descriptor(
   name='GetInstanceRequest',
   full_name='yamcs.protobuf.yamcsManagement.GetInstanceRequest',
   filename=None,
@@ -1946,16 +2005,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5434,
-  serialized_end=5472,
+  serialized_start=5614,
+  serialized_end=5652,
 )
 
 
 _STARTINSTANCEREQUEST = _descriptor.Descriptor(
   name='StartInstanceRequest',
   full_name='yamcs.protobuf.yamcsManagement.StartInstanceRequest',
   filename=None,
@@ -1977,16 +2036,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5474,
-  serialized_end=5514,
+  serialized_start=5654,
+  serialized_end=5694,
 )
 
 
 _STOPINSTANCEREQUEST = _descriptor.Descriptor(
   name='StopInstanceRequest',
   full_name='yamcs.protobuf.yamcsManagement.StopInstanceRequest',
   filename=None,
@@ -2008,16 +2067,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5516,
-  serialized_end=5555,
+  serialized_start=5696,
+  serialized_end=5735,
 )
 
 
 _RESTARTINSTANCEREQUEST = _descriptor.Descriptor(
   name='RestartInstanceRequest',
   full_name='yamcs.protobuf.yamcsManagement.RestartInstanceRequest',
   filename=None,
@@ -2039,16 +2098,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto2',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5557,
-  serialized_end=5599,
+  serialized_start=5737,
+  serialized_end=5779,
 )
 
 _YAMCSINSTANCES.fields_by_name['instances'].message_type = _YAMCSINSTANCE
 _YAMCSINSTANCE_LABELSENTRY.containing_type = _YAMCSINSTANCE
 _YAMCSINSTANCE_TEMPLATEARGSENTRY.containing_type = _YAMCSINSTANCE
 _YAMCSINSTANCE.fields_by_name['missionDatabase'].message_type = yamcs_dot_protobuf_dot_mdb_dot_mdb__pb2._MISSIONDATABASE
 _YAMCSINSTANCE.fields_by_name['processors'].message_type = _PROCESSORINFO
@@ -2059,14 +2118,15 @@
 _YAMCSINSTANCE_INSTANCESTATE.containing_type = _YAMCSINSTANCE
 _INSTANCETEMPLATE.fields_by_name['variables'].message_type = _TEMPLATEVARIABLE
 _PROCESSORINFO.fields_by_name['state'].enum_type = _SERVICESTATE
 _PROCESSORINFO.fields_by_name['replayRequest'].message_type = yamcs_dot_protobuf_dot_yamcs__pb2._REPLAYREQUEST
 _PROCESSORINFO.fields_by_name['replayState'].enum_type = yamcs_dot_protobuf_dot_yamcs__pb2._REPLAYSTATUS_REPLAYSTATE
 _PROCESSORINFO.fields_by_name['services'].message_type = _SERVICEINFO
 _PROCESSORINFO.fields_by_name['time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
+_PROCESSORINFO.fields_by_name['acknowledgments'].message_type = _ACKNOWLEDGMENTINFO
 _TMSTATISTICS.fields_by_name['lastReceived'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _TMSTATISTICS.fields_by_name['lastPacketTime'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _STATISTICS.fields_by_name['tmstats'].message_type = _TMSTATISTICS
 _STATISTICS.fields_by_name['lastUpdated'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _PROCESSORMANAGEMENTREQUEST.fields_by_name['operation'].enum_type = _PROCESSORMANAGEMENTREQUEST_OPERATION
 _PROCESSORMANAGEMENTREQUEST_OPERATION.containing_type = _PROCESSORMANAGEMENTREQUEST
 _PROCESSORREQUEST.fields_by_name['operation'].enum_type = _PROCESSORREQUEST_OPERATION
@@ -2092,14 +2152,15 @@
 _RECONFIGUREINSTANCEREQUEST.fields_by_name['labels'].message_type = _RECONFIGUREINSTANCEREQUEST_LABELSENTRY
 _LISTINSTANCETEMPLATESRESPONSE.fields_by_name['templates'].message_type = _INSTANCETEMPLATE
 DESCRIPTOR.message_types_by_name['YamcsInstances'] = _YAMCSINSTANCES
 DESCRIPTOR.message_types_by_name['YamcsInstance'] = _YAMCSINSTANCE
 DESCRIPTOR.message_types_by_name['InstanceTemplate'] = _INSTANCETEMPLATE
 DESCRIPTOR.message_types_by_name['TemplateVariable'] = _TEMPLATEVARIABLE
 DESCRIPTOR.message_types_by_name['ProcessorInfo'] = _PROCESSORINFO
+DESCRIPTOR.message_types_by_name['AcknowledgmentInfo'] = _ACKNOWLEDGMENTINFO
 DESCRIPTOR.message_types_by_name['TmStatistics'] = _TMSTATISTICS
 DESCRIPTOR.message_types_by_name['Statistics'] = _STATISTICS
 DESCRIPTOR.message_types_by_name['ProcessorManagementRequest'] = _PROCESSORMANAGEMENTREQUEST
 DESCRIPTOR.message_types_by_name['ProcessorRequest'] = _PROCESSORREQUEST
 DESCRIPTOR.message_types_by_name['ServiceInfo'] = _SERVICEINFO
 DESCRIPTOR.message_types_by_name['StreamEvent'] = _STREAMEVENT
 DESCRIPTOR.message_types_by_name['SystemInfo'] = _SYSTEMINFO
@@ -2171,14 +2232,21 @@
 ProcessorInfo = _reflection.GeneratedProtocolMessageType('ProcessorInfo', (_message.Message,), dict(
   DESCRIPTOR = _PROCESSORINFO,
   __module__ = 'yamcs.protobuf.yamcsManagement.yamcsManagement_pb2'
   # @@protoc_insertion_point(class_scope:yamcs.protobuf.yamcsManagement.ProcessorInfo)
   ))
 _sym_db.RegisterMessage(ProcessorInfo)
 
+AcknowledgmentInfo = _reflection.GeneratedProtocolMessageType('AcknowledgmentInfo', (_message.Message,), dict(
+  DESCRIPTOR = _ACKNOWLEDGMENTINFO,
+  __module__ = 'yamcs.protobuf.yamcsManagement.yamcsManagement_pb2'
+  # @@protoc_insertion_point(class_scope:yamcs.protobuf.yamcsManagement.AcknowledgmentInfo)
+  ))
+_sym_db.RegisterMessage(AcknowledgmentInfo)
+
 TmStatistics = _reflection.GeneratedProtocolMessageType('TmStatistics', (_message.Message,), dict(
   DESCRIPTOR = _TMSTATISTICS,
   __module__ = 'yamcs.protobuf.yamcsManagement.yamcsManagement_pb2'
   # @@protoc_insertion_point(class_scope:yamcs.protobuf.yamcsManagement.TmStatistics)
   ))
 _sym_db.RegisterMessage(TmStatistics)
 
@@ -2393,16 +2461,16 @@
 
 _MANAGEMENTAPI = _descriptor.ServiceDescriptor(
   name='ManagementApi',
   full_name='yamcs.protobuf.yamcsManagement.ManagementApi',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
-  serialized_start=5696,
-  serialized_end=8036,
+  serialized_start=5876,
+  serialized_end=8216,
   methods=[
   _descriptor.MethodDescriptor(
     name='GetSystemInfo',
     full_name='yamcs.protobuf.yamcsManagement.ManagementApi.GetSystemInfo',
     index=0,
     containing_service=None,
     input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
```

### Comparing `yamcs-client-1.8.8/src/yamcs/protobuf/yamcs_pb2.py` & `yamcs-client-1.9.0/src/yamcs/protobuf/yamcs_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs-client-1.8.8/src/yamcs/storage/client.py` & `yamcs-client-1.9.0/src/yamcs/storage/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,128 +1,152 @@
+from typing import IO, Iterable, Optional
+
+from yamcs.core.context import Context
 from yamcs.protobuf.buckets import buckets_pb2
 from yamcs.storage.model import Bucket, ObjectListing
 
 
 class StorageClient:
     """
     Client for working with buckets and objects managed by Yamcs.
     """
 
-    def __init__(self, ctx, instance="_global"):
+    def __init__(self, ctx: Context, instance: str = "_global"):
         super(StorageClient, self).__init__()
         self.ctx = ctx
         self._instance = instance
 
-    def list_buckets(self):
+    def list_buckets(self) -> Iterable[Bucket]:
         """
         List the buckets.
-
-        :rtype: ~collections.abc.Iterable[.Bucket]
         """
         # Server does not do pagination on listings of this resource.
         # Return an iterator anyway for similarity with other API methods
         response = self.ctx.get_proto(path="/buckets/" + self._instance)
         message = buckets_pb2.ListBucketsResponse()
         message.ParseFromString(response.content)
         buckets = getattr(message, "buckets")
         return iter([Bucket(bucket, self) for bucket in buckets])
 
-    def get_bucket(self, name):
+    def get_bucket(self, name: str) -> Bucket:
         """
         Get a specific bucket.
 
-        :param str name: The bucket name.
-        :rtype: .Bucket
+        :param name:
+            The bucket name.
         """
         # TODO should have an actual server-side operation for this
         # (added in Yamcs 5.6.1)
         for bucket in self.list_buckets():
             if bucket.name == name:
                 return bucket
         return None
 
-    def list_objects(self, bucket_name, prefix=None, delimiter=None):
+    def list_objects(
+        self,
+        bucket_name: str,
+        prefix: Optional[str] = None,
+        delimiter: Optional[str] = None,
+    ) -> ObjectListing:
         """
         List the objects for a bucket.
 
-        :param str bucket_name: The name of the bucket.
-        :param str prefix: If specified, only objects that start with this
-                           prefix are listed.
-        :param str delimiter: If specified, return only objects whose name
-                              do not contain the delimiter after the prefix.
-                              For the other objects, the response contains
-                              (in the prefix response parameter) the name
-                              truncated after the delimiter. Duplicates are
-                              omitted.
-        :rtype: .ObjectListing
+        :param bucket_name:
+            The name of the bucket.
+        :param prefix:
+            If specified, only objects that start with this
+            prefix are listed.
+        :param delimiter:
+            If specified, return only objects whose name
+            do not contain the delimiter after the prefix.
+            For the other objects, the response contains
+            (in the prefix response parameter) the name
+            truncated after the delimiter. Duplicates are
+            omitted.
         """
         url = f"/buckets/{self._instance}/{bucket_name}/objects"
         params = {}
         if prefix is not None:
             params["prefix"] = prefix
         if delimiter is not None:
             params["delimiter"] = delimiter
         response = self.ctx.get_proto(path=url, params=params)
         message = buckets_pb2.ListObjectsResponse()
         message.ParseFromString(response.content)
         return ObjectListing(message, bucket_name, self)
 
-    def create_bucket(self, bucket_name):
+    def create_bucket(self, bucket_name: str):
         """
         Create a new bucket.
 
-        :param str bucket_name: The name of the bucket.
+        :param bucket_name:
+            The name of the bucket.
         """
         req = buckets_pb2.CreateBucketRequest()
         req.name = bucket_name
         url = f"/buckets/{self._instance}"
         self.ctx.post_proto(url, data=req.SerializeToString())
 
-    def remove_bucket(self, bucket_name):
+    def remove_bucket(self, bucket_name: str):
         """
         Remove a bucket.
 
-        :param str bucket_name: The name of the bucket.
+        :param bucket_name:
+            The name of the bucket.
         """
         url = f"/buckets/{self._instance}/{bucket_name}"
         self.ctx.delete_proto(url)
 
-    def download_object(self, bucket_name, object_name):
+    def download_object(self, bucket_name: str, object_name: str):
         """
         Download an object.
 
-        :param str bucket_name: The name of the bucket.
-        :param str object_name: The object to fetch.
+        :param bucket_name:
+            The name of the bucket.
+        :param object_name:
+            The object to fetch.
         """
         url = f"/buckets/{self._instance}/{bucket_name}/objects/{object_name}"
         response = self.ctx.get_proto(path=url)
         return response.content
 
-    def upload_object(self, bucket_name, object_name, file_obj, content_type=None):
+    def upload_object(
+        self,
+        bucket_name: str,
+        object_name: str,
+        file_obj: IO,
+        content_type: Optional[str] = None,
+    ):
         """
         Upload an object to a bucket.
 
-        :param str bucket_name: The name of the bucket.
-        :param str object_name: The target name of the object.
-        :param file file_obj: The file (or file-like object) to upload.
-        :param str content_type: The content type associated to this object.
-                                 This is mainly useful when accessing an object
-                                 directly via a web browser. If unspecified, a
-                                 content type *may* be automatically derived
-                                 from the specified ``file_obj``.
+        :param bucket_name:
+            The name of the bucket.
+        :param object_name:
+            The target name of the object.
+        :param file_obj:
+            The file (or file-like object) to upload.
+        :param content_type:
+            The content type associated to this object.
+            This is mainly useful when accessing an object
+            directly via a web browser. If unspecified, a
+            content type *may* be automatically derived
+            from the specified ``file_obj``.
         """
         url = f"/buckets/{self._instance}/{bucket_name}/objects/{object_name}"
         if content_type:
             files = {object_name: (object_name, file_obj, content_type)}
         else:
             files = {object_name: (object_name, file_obj)}
         self.ctx.request(path=url, method="post", files=files)
 
-    def remove_object(self, bucket_name, object_name):
+    def remove_object(self, bucket_name: str, object_name: str):
         """
         Remove an object from a bucket.
 
-        :param str bucket_name: The name of the bucket.
-        :param str object_name: The object to remove.
+        :param bucket_name:
+            The name of the bucket.
+        :param object_name:
+            The object to remove.
         """
         url = f"/buckets/{self._instance}/{bucket_name}/objects/{object_name}"
         self.ctx.delete_proto(url)
```

### Comparing `yamcs-client-1.8.8/src/yamcs/storage/model.py` & `yamcs-client-1.9.0/src/yamcs/storage/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,211 +1,224 @@
+import datetime
+from typing import IO, List, Optional
+
 from yamcs.core.helpers import parse_server_time
 
 
 class Bucket:
     def __init__(self, proto, storage_client):
         self._proto = proto
         self._storage_client = storage_client
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Name of this bucket."""
         return self._proto.name
 
     @property
-    def created(self):
+    def created(self) -> datetime.datetime:
         """
         When this bucket was created.
 
-        :type: :class:`~datetime.datetime`
-
         .. versionadded:: 1.8.4
            Compatible with Yamcs 5.6.1 onwards
         """
         if self._proto.HasField("created"):
             return parse_server_time(self._proto.created)
         return None
 
     @property
-    def object_count(self):
+    def object_count(self) -> int:
         """Number of objects in this bucket."""
         return self._proto.numObjects
 
     @property
-    def max_object_count(self):
+    def max_object_count(self) -> int:
         """
         Maximum allowed number of objects.
 
         .. versionadded:: 1.8.4
            Compatible with Yamcs 5.6.1 onwards
         """
         if self._proto.HasField("maxObjects"):
             return self._proto.maxObjects
         return None
 
     @property
-    def size(self):
+    def size(self) -> int:
         """Total size in bytes of this bucket (excluding metadata)."""
         return self._proto.size
 
     @property
-    def max_size(self):
+    def max_size(self) -> int:
         """
         Maximum allowed total size of all objects.
 
         .. versionadded:: 1.8.4
            Compatible with Yamcs 5.6.1 onwards
         """
         if self._proto.HasField("maxSize"):
             return self._proto.maxSize
         return None
 
     @property
-    def directory(self):
+    def directory(self) -> str:
         """
         Bucket root directory. This field is only set when
         the bucket is mapped to the file system. Therefore
         it is not set for buckets that store objects in
         RocksDB.
 
         .. versionadded:: 1.8.4
            Compatible with Yamcs 5.6.1 onwards
         """
         if self._proto.HasField("directory"):
             return self._proto.directory
         return None
 
-    def list_objects(self, prefix=None, delimiter=None):
+    def list_objects(
+        self, prefix: Optional[str] = None, delimiter: Optional[str] = None
+    ):
         """
         List the objects for this bucket.
 
-        :param str prefix: If specified, only objects that start with this
-                           prefix are listed.
-        :param str delimiter: If specified, return only objects whose name
-                              do not contain the delimiter after the prefix.
-                              For the other objects, the response contains
-                              (in the prefix response parameter) the name
-                              truncated after the delimiter. Duplicates are
-                              omitted.
-        :rtype: .ObjectListing
+        :param prefix:
+            If specified, only objects that start with this prefix are listed.
+        :param delimiter:
+            If specified, return only objects whose name
+            do not contain the delimiter after the prefix.
+            For the other objects, the response contains
+            (in the prefix response parameter) the name
+            truncated after the delimiter. Duplicates are
+            omitted.
         """
         return self._storage_client.list_objects(
             bucket_name=self.name,
             prefix=prefix,
             delimiter=delimiter,
         )
 
-    def download_object(self, object_name):
+    def download_object(self, object_name: str):
         """
         Download an object.
 
-        :param str object_name: The object to fetch.
+        :param object_name:
+            The object to fetch.
         """
         return self._storage_client.download_object(self.name, object_name)
 
-    def upload_object(self, object_name, file_obj, content_type=None):
+    def upload_object(
+        self, object_name: str, file_obj: IO, content_type: Optional[str] = None
+    ):
         """
         Upload an object to this bucket.
 
-        :param str object_name: The target name of the object.
-        :param file file_obj: The file (or file-like object) to upload.
-        :param str content_type: The content type associated to this object.
-                                 This is mainly useful when accessing an object
-                                 directly via a web browser. If unspecified, a
-                                 content type *may* be automatically derived
-                                 from the specified ``file_obj``.
+        :param object_name:
+            The target name of the object.
+        :param file_obj:
+            The file (or file-like object) to upload.
+        :param content_type:
+            The content type associated to this object.
+            This is mainly useful when accessing an object
+            directly via a web browser. If unspecified, a
+            content type *may* be automatically derived
+            from the specified ``file_obj``.
         """
         return self._storage_client.upload_object(
             self.name, object_name, file_obj, content_type=content_type
         )
 
-    def delete_object(self, object_name):
+    def delete_object(self, object_name: str):
         """
         Remove an object from this bucket.
 
-        :param str object_name: The object to remove.
+        :param object_name:
+            The object to remove.
         """
         self._storage_client.remove_object(self.name, object_name)
 
     def delete(self):
         """
         Remove this bucket in its entirety.
         """
         self._storage_client.remove_bucket(self.name)
 
     def __str__(self):
         return self.name
 
 
-class ObjectListing:
+class ObjectInfo:
     def __init__(self, proto, bucket, storage_client):
         self._proto = proto
         self._bucket = bucket
         self._storage_client = storage_client
 
     @property
-    def prefixes(self):
+    def name(self) -> str:
         """
-        The prefixes in this listing.
-
-        :type: str[]
+        The name of this object.
         """
-        return [p for p in self._proto.prefixes]
+        return self._proto.name
 
     @property
-    def objects(self):
+    def size(self) -> int:
         """
-        The objects in this listing.
-
-        :type: List[:class:`.ObjectInfo`]
+        Size in bytes of this object (excluding metadata).
         """
-        return [
-            ObjectInfo(o, self._bucket, self._storage_client)
-            for o in self._proto.objects
-        ]
-
-
-class ObjectInfo:
-    def __init__(self, proto, bucket, storage_client):
-        self._proto = proto
-        self._bucket = bucket
-        self._storage_client = storage_client
-
-    @property
-    def name(self):
-        """The name of this object."""
-        return self._proto.name
-
-    @property
-    def size(self):
-        """Size in bytes of this object (excluding metadata)."""
         return self._proto.size
 
     @property
-    def created(self):
+    def created(self) -> datetime.datetime:
         """
         Return when this object was created (or re-created).
-
-        :type: :class:`~datetime.datetime`
         """
         if self._proto.HasField("created"):
             return parse_server_time(self._proto.created)
         return None
 
     def delete(self):
-        """Remove this object."""
+        """
+        Remove this object.
+        """
         self._storage_client.remove_object(self._bucket, self.name)
 
     def download(self):
-        """Download this object."""
+        """
+        Download this object.
+        """
         return self._storage_client.download_object(self._bucket, self.name)
 
-    def upload(self, file_obj):
+    def upload(self, file_obj: IO):
         """
         Replace the content of this object.
 
-        :param file file_obj: The file (or file-like object) to upload.
+        :param file_obj:
+            The file (or file-like object) to upload.
         """
         return self._storage_client.upload_object(self._bucket, self.name, file_obj)
 
     def __str__(self):
         return f"{self.name} ({self.size} bytes, created {self.created})"
+
+
+class ObjectListing:
+    def __init__(self, proto, bucket, storage_client):
+        self._proto = proto
+        self._bucket = bucket
+        self._storage_client = storage_client
+
+    @property
+    def prefixes(self) -> List[str]:
+        """
+        The prefixes in this listing.
+        """
+        return [p for p in self._proto.prefixes]
+
+    @property
+    def objects(self) -> List[ObjectInfo]:
+        """
+        The objects in this listing.
+        """
+        return [
+            ObjectInfo(o, self._bucket, self._storage_client)
+            for o in self._proto.objects
+        ]
```

### Comparing `yamcs-client-1.8.8/src/yamcs/tco/client.py` & `yamcs-client-1.9.0/src/yamcs/tco/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,112 @@
+import datetime
+from typing import List, Optional
+
+from yamcs.core.context import Context
 from yamcs.core.helpers import to_server_time
 from yamcs.protobuf.tco import tco_pb2
 from yamcs.tco.model import TCOStatus, TofInterval
 
 
 class TCOClient:
     """
     Client for interacting with a Time Correlation service managed by Yamcs.
     """
 
-    def __init__(self, ctx, instance, service):
+    def __init__(self, ctx: Context, instance: str, service: str):
         super(TCOClient, self).__init__()
         self.ctx = ctx
         self._instance = instance
         self._service = service
 
-    def get_status(self):
+    def get_status(self) -> TCOStatus:
         """
         Retrieve the TCO status.
-
-        :rtype: .TCOStatus
         """
         response = self.ctx.get_proto(f"/tco/{self._instance}/{self._service}/status")
         message = tco_pb2.TcoStatus()
         message.ParseFromString(response.content)
         return TCOStatus(message)
 
     def reconfigure(
-        self, accuracy=None, validity=None, ob_delay=None, default_tof=None
+        self,
+        accuracy: Optional[float] = None,
+        validity: Optional[float] = None,
+        ob_delay: Optional[float] = None,
+        default_tof: Optional[float] = None,
     ):
         """
         Updates one or more TCO options
 
-        :param Optional[float] accuracy: Accuracy in seconds.
-        :param Optional[float] validity: Validity in seconds.
-        :param Optional[float] ob_delay: Onboard delay in seconds.
-        :param Optional[float] default_tof: Default ToF in seconds. This value is used
-                                            if the ToF estimator does not find a
-                                            matching interval.
+        :param accuracy:
+            Accuracy in seconds.
+        :param validity:
+            Validity in seconds.
+        :param ob_delay:
+            Onboard delay in seconds.
+        :param default_tof:
+            Default ToF in seconds. This value is used if the ToF estimator
+            does not find a matching interval.
         """
         req = tco_pb2.TcoConfig()
         if accuracy is not None:
             req.accuracy = accuracy
         if validity is not None:
             req.validity = validity
         if ob_delay is not None:
             req.onboardDelay = ob_delay
         if default_tof is not None:
             req.defaultTof = default_tof
 
         url = f"/tco/{self._instance}/{self._service}/config"
         self.ctx.post_proto(url, data=req.SerializeToString())  # TODO should be patch
 
-    def add_tof_interval(self, start, stop, polynomial):
+    def add_tof_interval(
+        self, start: datetime.datetime, stop: datetime.datetime, polynomial: List[float]
+    ):
         """
         Defines a ToF interval for the ERT range ``[start, stop]``, specifying
         a polynomial function of the form: `tof = a + bx + cx^2 + ...` where `x`
         is ERT minus the provided start date.
 
-        :param ~datetime.datetime start: ERT start
-        :param ~datetime.datetime stop: ERT stop
-        :param float[] polynomial: Coefficients in the order ``[a, b, c, ...]``
+        :param start:
+            ERT start
+        :param stop:
+            ERT stop
+        :param polynomial:
+            Coefficients in the order ``[a, b, c, ...]``
         """
         self.add_tof_interval([TofInterval(start, stop, polynomial)])
 
-    def add_tof_intervals(self, intervals):
+    def add_tof_intervals(self, intervals: List[TofInterval]):
         """
         Adds multiple ToF intervals at once.
 
-        :param .TofInterval[] intervals: List of ToF intervals.
+        :param intervals:
+            List of ToF intervals.
         """
         req = tco_pb2.AddTimeOfFlightIntervalsRequest()
         for interval in intervals:
             tof = req.intervals.add()
             tof.ertStart.MergeFrom(to_server_time(interval.start))
             tof.ertStop.MergeFrom(to_server_time(interval.stop))
             tof.polCoef.extend(interval.polynomial)
 
         url = f"/tco/{self._instance}/{self._service}/tof:addIntervals"
         self.ctx.post_proto(url, data=req.SerializeToString())
 
-    def remove_tof_intervals(self, start, stop):
+    def remove_tof_intervals(self, start: datetime.datetime, stop: datetime.datetime):
         """
         Removes previously registered ToF intervals whose start date
         falls in the specified range ``[start, stop]``.
 
-        :param ~datetime.datetime start: ERT start
-        :param ~datetime.datetime stop: ERT stop
+        :param start:
+            ERT start
+        :param stop:
+            ERT stop
         """
         req = tco_pb2.DeleteTimeOfFlightIntervalsRequest()
         req.start.MergeFrom(to_server_time(start))
         req.stop.MergeFrom(to_server_time(stop))
 
         url = f"/tco/{self._instance}/{self._service}/tof:deleteIntervals"
         self.ctx.post_proto(url, data=req.SerializeToString())
@@ -98,27 +115,33 @@
         """
         Resets current TCO coefficients, as well as any
         collected samples.
         """
         url = f"/tco/{self._instance}/{self._service}:reset"
         self.ctx.post_proto(url)
 
-    def override_coefficients(self, utc, obt, gradient=0, offset=0):
+    def override_coefficients(
+        self, utc: datetime.datetime, obt: int, gradient: float = 0, offset: float = 0
+    ):
         """
         Manually override the assocation between UTC and
         onboard time.
 
         .. note::
             If later on you want to revert to automatically computed
             coefficients, use :meth:`reset_coefficients`.
 
-        :param ~datetime.datetime utc: UTC
-        :param int obt: Onboard time
-        :param Optional[float] gradient: Gradient
-        :param Optional[float] offset: Offset
+        :param utc:
+            UTC
+        :param obt:
+            Onboard time
+        :param gradient:
+            Gradient
+        :param offset:
+            Offset
         """
         req = tco_pb2.TcoCoefficients()
         req.utc.MergeFrom(to_server_time(utc))
         req.obt = obt
         req.gradient = gradient
         req.offset = offset
```

### Comparing `yamcs-client-1.8.8/src/yamcs/timeline/client.py` & `yamcs-client-1.9.0/src/yamcs/timeline/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,57 @@
+import datetime
+from typing import Iterable, Optional
+
 from yamcs.core import pagination
+from yamcs.core.context import Context
 from yamcs.core.helpers import to_isostring
 from yamcs.protobuf.timeline import timeline_pb2
 from yamcs.timeline.model import Band, Item, View
 
 
 class TimelineClient:
     """
     Client for working with Yamcs timeline.
     """
 
-    def __init__(self, ctx, instance):
+    def __init__(self, ctx: Context, instance: str):
         super(TimelineClient, self).__init__()
         self.ctx = ctx
         self._instance = instance
 
-    def list_views(self):
+    def list_views(self) -> Iterable[View]:
         """
         List the views.
-
-        :rtype: ~collections.abc.Iterable[.View]
         """
         # Server does not do pagination on listings of this resource.
         # Return an iterator anyway for similarity with other API methods
         response = self.ctx.get_proto(f"/timeline/{self._instance}/views")
         message = timeline_pb2.ListViewsResponse()
         message.ParseFromString(response.content)
-        return [View(proto) for proto in getattr(message, "views")]
+        return iter([View(proto) for proto in getattr(message, "views")])
 
-    def get_view(self, id):
+    def get_view(self, id: str) -> View:
         """
         Fetch a view by its identifier.
 
-        :param str id: View identifier
-        :rtype: .View
+        :param id:
+            View identifier
         """
         url = f"/timeline/{self._instance}/views/{id}"
         response = self.ctx.get_proto(url)
         message = timeline_pb2.TimelineView()
         message.ParseFromString(response.content)
         return View(message)
 
-    def save_view(self, view):
+    def save_view(self, view: View):
         """
         Save or update a view.
 
-        :param .View view: View object
+        :param view:
+            View object
         """
         if view.id:
             url = f"/timeline/{self._instance}/views/{view.id}"
             req = timeline_pb2.UpdateViewRequest()
         else:
             url = f"/timeline/{self._instance}/views"
             req = timeline_pb2.AddViewRequest()
@@ -62,54 +65,54 @@
         else:
             response = self.ctx.post_proto(url, data=req.SerializeToString())
 
         message = timeline_pb2.TimelineView()
         message.ParseFromString(response.content)
         view._proto = message
 
-    def delete_view(self, view):
+    def delete_view(self, view: str):
         """
         Delete a view.
 
-        :param string view: View identifier.
+        :param view:
+            View identifier.
         """
         url = f"/timeline/{self._instance}/views/{view}"
         self.ctx.delete_proto(url)
 
-    def list_bands(self):
+    def list_bands(self) -> Iterable[Band]:
         """
         List the bands.
-
-        :rtype: ~collections.abc.Iterable[.Band]
         """
         # Server does not do pagination on listings of this resource.
         # Return an iterator anyway for similarity with other API methods
         response = self.ctx.get_proto(f"/timeline/{self._instance}/bands")
         message = timeline_pb2.ListBandsResponse()
         message.ParseFromString(response.content)
-        return [Band._as_subclass(proto) for proto in getattr(message, "bands")]
+        return iter([Band._as_subclass(proto) for proto in getattr(message, "bands")])
 
-    def get_band(self, id):
+    def get_band(self, id: str) -> Band:
         """
         Fetch a band by its identifier.
 
-        :param str id: Band identifier
-        :rtype: .Band
+        :param id:
+            Band identifier
         """
         url = f"/timeline/{self._instance}/bands/{id}"
         response = self.ctx.get_proto(url)
         message = timeline_pb2.TimelineBand()
         message.ParseFromString(response.content)
         return Band._as_subclass(message)
 
-    def save_band(self, band):
+    def save_band(self, band: Band):
         """
         Save or update a band.
 
-        :param .Band band: Band object
+        :param band:
+            Band object
         """
         if band.id:
             url = f"/timeline/{self._instance}/bands/{band.id}"
             req = timeline_pb2.UpdateBandRequest()
         else:
             url = f"/timeline/{self._instance}/bands"
             req = timeline_pb2.AddBandRequest()
@@ -129,36 +132,43 @@
         else:
             response = self.ctx.post_proto(url, data=req.SerializeToString())
 
         message = timeline_pb2.TimelineBand()
         message.ParseFromString(response.content)
         band._proto = message
 
-    def delete_band(self, band):
+    def delete_band(self, band: str):
         """
         Delete a band.
 
-        :param string band: Band identifier.
+        :param band:
+            Band identifier.
         """
         url = f"/timeline/{self._instance}/bands/{band}"
         self.ctx.delete_proto(url)
 
-    def list_items(self, band=None, start=None, stop=None, page_size=500):
+    def list_items(
+        self,
+        band: Optional[str] = None,
+        start: Optional[datetime.datetime] = None,
+        stop: Optional[datetime.datetime] = None,
+        page_size: int = 500,
+    ) -> Iterable[Item]:
         """
         List the items.
 
-        :param str band: Return only items matching the specified band
-        :param ~datetime.datetime start: Minimum stop time of the returned
-                                         items (exclusive)
-        :param ~datetime.datetime stop: Maximum start time of the returned
-                                        items (exclusive)
-        :param int page_size: Page size of underlying requests. Higher values imply
-                              less overhead, but risk hitting the maximum message size
-                              limit.
-        :rtype: ~collections.abc.Iterable[.Item]
+        :param band:
+            Return only items matching the specified band
+        :param start:
+            Minimum stop time of the returned items (exclusive)
+        :param stop:
+            Maximum start time of the returned items (exclusive)
+        :param page_size:
+            Page size of underlying requests. Higher values imply less
+            overhead, but risk hitting the maximum message size limit.
         """
         params = {}
         if band is not None:
             params["band"] = band
         if page_size is not None:
             params["limit"] = page_size
         if start is not None:
@@ -171,32 +181,33 @@
             path=f"/timeline/{self._instance}/items",
             params=params,
             response_class=timeline_pb2.ListItemsResponse,
             items_key="items",
             item_mapper=Item,
         )
 
-    def get_item(self, id):
+    def get_item(self, id: str) -> Item:
         """
         Fetch an item by its identifier.
 
-        :param str id: Item identifier
-        :rtype: .Item
+        :param id:
+            Item identifier
         """
         url = f"/timeline/{self._instance}/items/{id}"
         response = self.ctx.get_proto(url)
         message = timeline_pb2.TimelineItem()
         message.ParseFromString(response.content)
         return Item(message)
 
-    def save_item(self, item):
+    def save_item(self, item: Item):
         """
         Save or update an item.
 
-        :param .Item item: Item object
+        :param item:
+            Item object
         """
         if item.id:
             url = f"/timeline/{self._instance}/items/{item.id}"
             req = timeline_pb2.UpdateItemRequest()
         else:
             url = f"/timeline/{self._instance}/items"
             req = timeline_pb2.CreateItemRequest()
@@ -212,15 +223,16 @@
         else:
             response = self.ctx.post_proto(url, data=req.SerializeToString())
 
         message = timeline_pb2.TimelineItem()
         message.ParseFromString(response.content)
         item._proto = message
 
-    def delete_item(self, item):
+    def delete_item(self, item: str):
         """
         Delete an item.
 
-        :param string item: Item identifier.
+        :param item:
+            Item identifier.
         """
         url = f"/timeline/{self._instance}/items/{item}"
         self.ctx.delete_proto(url)
```

### Comparing `yamcs-client-1.8.8/src/yamcs/timeline/model.py` & `yamcs-client-1.9.0/src/yamcs/timeline/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,136 +1,79 @@
 import abc
-from xmlrpc.client import boolean
+import datetime
+from typing import List
 
 from yamcs.core.helpers import ProtoList, parse_server_time, to_server_time
 from yamcs.protobuf.timeline import timeline_pb2
 
 
-class View:
-    def __init__(self, proto=None):
-        merged = timeline_pb2.TimelineView()
-        if proto:
-            merged.MergeFrom(proto)
-        self._proto = merged
-
-        self._bands = ProtoList(self._proto, "bands", lambda x: Band._as_subclass(x))
-
-    @property
-    def id(self):
-        """View identifier."""
-        if self._proto.HasField("id"):
-            return self._proto.id
-        return None
-
-    @property
-    def name(self):
-        """Name of this view."""
-        return self._proto.name
-
-    @name.setter
-    def name(self, value):
-        self._proto.name = value
-
-    @property
-    def description(self):
-        """Description of this view."""
-        return self._proto.description
-
-    @description.setter
-    def description(self, value):
-        self._proto.name = value
-
-    @property
-    def bands(self):
-        """
-        Bands included in this view.
-
-        :type: List[:class:`.Band`]
-        """
-        return self._bands
-
-    @bands.setter
-    def bands(self, value):
-        self._bands.clear()
-        self._bands.extend(value)
-
-    def __str__(self):
-        return self.name
-
-
 class Item:
     def __init__(self, proto=None):
         merged = timeline_pb2.TimelineItem()
         merged.type = timeline_pb2.TimelineItemType.EVENT
         if proto:
             merged.MergeFrom(proto)
         self._proto = merged
 
     @property
-    def id(self):
+    def id(self) -> str:
         """Item identifier."""
         if self._proto.HasField("id"):
             return self._proto.id
         return None
 
     @property
-    def item_type(self):
+    def item_type(self) -> str:
         """Type of item."""
         return timeline_pb2.TimelineItemType.Name(self._proto.type)
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Name of this item."""
         return self._proto.name
 
     @name.setter
-    def name(self, value):
+    def name(self, value: str):
         self._proto.name = value
 
     @property
-    def tags(self):
+    def tags(self) -> List[str]:
         """
         Item tags. Used by bands to filter what is visible.
-
-        :type: str[]
         """
         return self._proto.tags
 
     @tags.setter
-    def tags(self, value):
+    def tags(self, value: List[str]):
         self._proto.tags[:] = value
 
     @property
-    def start(self):
+    def start(self) -> datetime.datetime:
         """
         Item start time.
-
-        :type: :class:`~datetime.datetime`
         """
         if self._proto.HasField("start"):
             return parse_server_time(self._proto.start)
         return None
 
     @start.setter
-    def start(self, value):
+    def start(self, value: datetime.datetime):
         self._proto.start.MergeFrom(to_server_time(value))
 
     @property
-    def duration(self):
+    def duration(self) -> datetime.timedelta:
         """
         Item duration.
-
-        :type: :class:`~datetime.timedelta`
         """
         if self._proto.HasField("duration"):
             return self._proto.duration.ToTimedelta()
         return None
 
     @duration.setter
-    def duration(self, value):
+    def duration(self, value: datetime.timedelta):
         self._proto.duration.FromTimedelta(value)
 
     def __str__(self):
         return self.name
 
 
 class Band(abc.ABC):
@@ -143,57 +86,57 @@
     * :class:`.CommandBand`
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def id(self):
+    def id(self) -> str:
         """Band identifier."""
         if self._proto.HasField("id"):
             return self._proto.id
         return None
 
     @property
-    def band_type(self):
+    def band_type(self) -> str:
         """Type of band."""
         return timeline_pb2.TimelineBandType.Name(self._proto.type)
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Name of this band."""
         return self._proto.name
 
     @name.setter
-    def name(self, value):
+    def name(self, value) -> str:
         self._proto.name = value
 
     @property
-    def description(self):
+    def description(self) -> str:
         """Description of this band."""
         return self._proto.description
 
     @description.setter
-    def description(self, value):
+    def description(self, value: str):
         self._proto.description = value
 
-    def _set_integer_property(self, key, value):
+    def _set_integer_property(self, key: str, value: int):
         if not isinstance(value, int):
             raise ValueError("Provided value is not integer")
         self._proto.properties[key] = str(value)
 
-    def _get_integer_property(self, key):
+    def _get_integer_property(self, key: str):
         return int(self._proto.properties[key])
 
-    def _set_boolean_property(self, key, value):
-        if not isinstance(value, boolean):
+    def _set_boolean_property(self, key: str, value: bool):
+        if not isinstance(value, bool):
             raise ValueError("Provided value is not boolean")
         self._proto.properties[key] = "true" if value else "false"
 
-    def _get_boolean_property(self, key):
+    def _get_boolean_property(self, key: str):
         return self._proto.properties[key] == "true"
 
     @staticmethod
     def _as_subclass(proto):
         if proto.type == timeline_pb2.TimelineBandType.TIME_RULER:
             return TimeRuler(proto)
         elif proto.type == timeline_pb2.TimelineBandType.ITEM_BAND:
@@ -219,27 +162,27 @@
         merged.type = timeline_pb2.TimelineBandType.TIME_RULER
         merged.properties["timezone"] = "UTC"
         if proto:
             merged.MergeFrom(proto)
         super(TimeRuler, self).__init__(merged)
 
     @property
-    def timezone(self):
+    def timezone(self) -> str:
         """
         IANA timezone name.
 
         Corresponds with the third column of the following table:
         https://data.iana.org/time-zones/data/zone1970.tab
 
         In addition, the name `UTC` is supported.
         """
         return self._proto.properties["timezone"]
 
     @timezone.setter
-    def timezone(self, value):
+    def timezone(self, value: str):
         self._proto.properties["timezone"] = value
 
 
 class Spacer(Band):
     """
     Insert empty vertical space.
     """
@@ -249,20 +192,20 @@
         merged.type = timeline_pb2.TimelineBandType.SPACER
         merged.properties["height"] = "34"
         if proto:
             merged.MergeFrom(proto)
         super(Spacer, self).__init__(merged)
 
     @property
-    def height(self):
+    def height(self) -> int:
         """Spacer height"""
         return self._get_integer_property("height")
 
     @height.setter
-    def height(self, value):
+    def height(self, value: int):
         self._set_integer_property("height", value)
 
 
 class CommandBand(Band):
     """
     Display issued commands.
     """
@@ -299,158 +242,206 @@
         merged.properties["spaceBetweenItems"] = "0"
         merged.properties["spaceBetweenLines"] = "2"
         if proto:
             merged.MergeFrom(proto)
         super(ItemBand, self).__init__(merged)
 
     @property
-    def frozen(self):
+    def frozen(self) -> bool:
         """
         Fix this line to the top of the view. Frozen bands are always
         rendered above other bands.
         """
         return self._get_boolean_property("frozen")
 
     @frozen.setter
-    def frozen(self, value):
+    def frozen(self, value: bool):
         self._set_boolean_property("frozen", value)
 
     @property
-    def tags(self):
+    def tags(self) -> List[str]:
         """
         Item tags that this band filters on.
-
-        :type: str[]
         """
         return self._proto.tags
 
     @tags.setter
-    def tags(self, value):
+    def tags(self, value: List[str]):
         self._proto.tags[:] = value
 
     @property
-    def item_background_color(self):
+    def item_background_color(self) -> str:
         """CSS color string."""
         return self._proto.properties["itemBackgroundColor"]
 
     @item_background_color.setter
-    def item_background_color(self, value):
+    def item_background_color(self, value: str):
         self._proto.properties["itemBackgroundColor"] = value
 
     @property
-    def item_border_color(self):
+    def item_border_color(self) -> str:
         """CSS color string."""
         return self._proto.properties["itemBorderColor"]
 
     @item_border_color.setter
-    def item_border_color(self, value):
+    def item_border_color(self, value: str):
         self._proto.properties["itemBorderColor"] = value
 
     @property
-    def item_border_width(self):
+    def item_border_width(self) -> int:
         return self._get_integer_property("itemBorderWidth")
 
     @item_border_width.setter
-    def item_border_width(self, value):
+    def item_border_width(self, value: int):
         self._set_integer_property("itemBorderWidth", value)
 
     @property
-    def item_corner_radius(self):
+    def item_corner_radius(self) -> int:
         return self._get_integer_property("itemCornerRadius")
 
     @item_corner_radius.setter
-    def item_corner_radius(self, value):
+    def item_corner_radius(self, value: int):
         self._set_integer_property("itemCornerRadius", value)
 
     @property
-    def item_height(self):
+    def item_height(self) -> int:
         return self._get_integer_property("itemHeight")
 
     @item_height.setter
-    def item_height(self, value):
+    def item_height(self, value: int):
         self._set_integer_property("itemHeight", value)
 
     @property
-    def item_margin_left(self):
+    def item_margin_left(self) -> int:
         return self._get_integer_property("itemMarginLeft")
 
     @item_margin_left.setter
-    def item_margin_left(self, value):
+    def item_margin_left(self, value: int):
         self._set_integer_property("itemMarginLeft", value)
 
     @property
-    def item_text_color(self):
+    def item_text_color(self) -> str:
         """CSS color string."""
         return self._proto.properties["itemTextColor"]
 
     @item_text_color.setter
-    def item_text_color(self, value):
+    def item_text_color(self, value: str):
         self._proto.properties["itemTextColor"] = value
 
     @property
-    def item_text_overflow(self):
+    def item_text_overflow(self) -> str:
         """One of ``show``, ``clip``, or ``hide``."""
         return self._proto.properties["itemTextOverflow"]
 
     @item_text_overflow.setter
-    def item_text_overflow(self, value):
+    def item_text_overflow(self, value: str):
         self._proto.properties["itemTextOverflow"] = value
 
     @property
-    def item_text_size(self):
+    def item_text_size(self) -> int:
         return self._get_integer_property("itemTextSize")
 
     @item_text_size.setter
-    def item_text_size(self, value):
+    def item_text_size(self, value: int):
         self._set_integer_property("itemTextSize", value)
 
     @property
-    def margin_bottom(self):
+    def margin_bottom(self) -> int:
         return self._get_integer_property("marginBottom")
 
     @margin_bottom.setter
-    def margin_bottom(self, value):
+    def margin_bottom(self, value: int):
         self._set_integer_property("marginBottom", value)
 
     @property
-    def margin_top(self):
+    def margin_top(self) -> int:
         return self._get_integer_property("marginTop")
 
     @margin_top.setter
-    def margin_top(self, value):
+    def margin_top(self, value: int):
         self._set_integer_property("marginTop", value)
 
     @property
-    def multiline(self):
+    def multiline(self) -> bool:
         """
         Draw items on multiple lines if otherwise there would be collisions.
         """
         return self._get_boolean_property("multiline")
 
     @multiline.setter
-    def multiline(self, value):
+    def multiline(self, value: bool):
         self._set_boolean_property("multiline", value)
 
     @property
-    def space_between_items(self):
+    def space_between_items(self) -> int:
         """
         In case of multilining, this indicates the minimum horizontal space
         between items. If an item does not meet this treshold, it gets
         rendered on a different line.
         """
         return self._get_integer_property("spaceBetweenItems")
 
     @space_between_items.setter
-    def space_between_items(self, value):
+    def space_between_items(self, value: int):
         self._set_integer_property("spaceBetweenItems", value)
 
     @property
-    def space_between_lines(self):
+    def space_between_lines(self) -> int:
         """
         In case of multilining, this indicates the vertical space between
         lines.
         """
         return self._get_integer_property("spaceBetweenLines")
 
     @space_between_lines.setter
-    def space_between_lines(self, value):
+    def space_between_lines(self, value: int):
         self._set_integer_property("spaceBetweenLines", value)
+
+
+class View:
+    def __init__(self, proto=None):
+        merged = timeline_pb2.TimelineView()
+        if proto:
+            merged.MergeFrom(proto)
+        self._proto = merged
+
+        self._bands = ProtoList(self._proto, "bands", lambda x: Band._as_subclass(x))
+
+    @property
+    def id(self) -> str:
+        """View identifier."""
+        if self._proto.HasField("id"):
+            return self._proto.id
+        return None
+
+    @property
+    def name(self) -> str:
+        """Name of this view."""
+        return self._proto.name
+
+    @name.setter
+    def name(self, value: str):
+        self._proto.name = value
+
+    @property
+    def description(self) -> str:
+        """Description of this view."""
+        return self._proto.description
+
+    @description.setter
+    def description(self, value: str):
+        self._proto.name = value
+
+    @property
+    def bands(self) -> List[Band]:
+        """
+        Bands included in this view.
+        """
+        return self._bands
+
+    @bands.setter
+    def bands(self, value: List[Band]):
+        self._bands.clear()
+        self._bands.extend(value)
+
+    def __str__(self):
+        return self.name
```

### Comparing `yamcs-client-1.8.8/src/yamcs/tmtc/client.py` & `yamcs-client-1.9.0/src/yamcs/tmtc/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import binascii
 import collections.abc
 import datetime
 import functools
 import json
 import threading
+from typing import Any, Callable, Dict, Iterable, List, Mapping, Optional, Tuple, Union
 
+from yamcs.core.context import Context
 from yamcs.core.exceptions import YamcsError
 from yamcs.core.futures import WebSocketSubscriptionFuture
 from yamcs.core.helpers import (
     adapt_name_for_rest,
     to_isostring,
     to_named_object_id,
     to_named_object_ids,
@@ -19,24 +21,27 @@
 from yamcs.protobuf.alarms import alarms_pb2, alarms_service_pb2
 from yamcs.protobuf.commanding import commanding_pb2, commands_service_pb2
 from yamcs.protobuf.mdb import mdb_pb2
 from yamcs.protobuf.packets import packets_pb2, packets_service_pb2
 from yamcs.protobuf.processing import mdb_override_service_pb2, processing_pb2
 from yamcs.protobuf.pvalue import pvalue_pb2
 from yamcs.tmtc.model import (
+    Alarm,
     AlarmUpdate,
     Calibrator,
     CommandHistory,
     ContainerData,
     IssuedCommand,
     MonitoredCommand,
     Packet,
     ParameterData,
     ParameterValue,
+    RangeSet,
     ValueUpdate,
+    VerificationConfig,
     _parse_alarm,
 )
 
 
 class SequenceGenerator:
     """Static atomic counter."""
 
@@ -243,37 +248,36 @@
 
     .. warning::
         If command history updates are received for commands
         that are not currently in the local cache, the returned
         information may be incomplete.
     """
 
-    def __init__(self, manager):
+    def __init__(self, manager: WebSocketSubscriptionManager):
         super(CommandHistorySubscription, self).__init__(manager)
-        self._cache = {}
+        self._cache: Dict[str, CommandHistory] = {}
 
     def clear_cache(self):
         """
         Clears local command history cache.
         """
         self._cache = {}
 
-    def get_command_history(self, issued_command):
+    def get_command_history(self, issued_command: IssuedCommand) -> CommandHistory:
         """
         Gets locally cached CommandHistory for the specified command.
 
-        :param .IssuedCommand issued_command: object representing a
-                                              previously issued command.
-        :rtype: .CommandHistory
+        :param issued_command:
+            object representing a previously issued command.
         """
         if issued_command.id in self._cache:
             return self._cache[issued_command.id]
         return None
 
-    def _process(self, entry):
+    def _process(self, entry) -> CommandHistory:
         if entry.id in self._cache:
             cmdhist = self._cache[entry.id]
             cmdhist._update(entry.attr)
         else:
             cmdhist = CommandHistory(entry)
             self._cache[entry.id] = cmdhist
 
@@ -281,109 +285,111 @@
 
 
 class ContainerSubscription(WebSocketSubscriptionFuture):
     """
     Local object providing access to container updates
     """
 
-    def __init__(self, manager):
+    def __init__(self, manager: WebSocketSubscriptionManager):
         super(ContainerSubscription, self).__init__(manager)
-        self._cache = {}
+        self._cache: Dict[str, ContainerData] = {}
         """Container cache keyed by container name."""
 
-    def get_container(self, name):
+    def get_container(self, name: str) -> ContainerData:
         """
         Returns the latest container of a specific name.
 
-        :param str name: Container name
-        :rtype: .ContainerData
+        :param name:
+            Container name
         """
         return self._cache[name]
 
-    def list_containers(self):
+    def list_containers(self) -> List[ContainerData]:
         """
         Returns the latest container for each name.
-
-        :rtype: .ContainerData[]
         """
         return [self._cache[k] for k in self._cache]
 
-    def _process(self, proto):
+    def _process(self, proto) -> ContainerData:
         container = ContainerData(proto)
         self._cache[container.name] = container
         return container
 
 
 class ParameterSubscription(WebSocketSubscriptionFuture):
     """
     Local object representing a subscription of zero or more parameters.
 
     A subscription object stores the last received value of each
     subscribed parameter.
     """
 
-    def __init__(self, manager):
+    def __init__(self, manager: WebSocketSubscriptionManager):
         super(ParameterSubscription, self).__init__(manager)
         self._mapping = {}
         """Mapping from server-assigned identifier, to requested parameter"""
 
-        self.value_cache = {}
+        self.value_cache: Dict[str, ParameterValue] = {}
         """Value cache keyed by parameter name."""
 
-        self.delivery_count = 0
+        self.delivery_count: int = 0
         """The number of parameter deliveries."""
 
-    def add(self, parameters, abort_on_invalid=True, send_from_cache=True):
+    def add(
+        self,
+        parameters: Union[str, List[str]],
+        abort_on_invalid: bool = True,
+        send_from_cache: bool = True,
+    ):
         """
         Add one or more parameters to this subscription.
 
-        :param parameters: Parameter(s) to be added
-        :type parameters: Union[str, str[]]
-        :param bool abort_on_invalid: If ``True`` one invalid parameter
-                                      means any other parameter in the
-                                      request will also not be added
-                                      to the subscription.
-        :param bool send_from_cache: If ``True`` the last processed parameter
-                                     value is sent from parameter cache.
-                                     When ``False`` only newly processed
-                                     parameters are received.
+        :param parameters:
+            Parameter(s) to be added
+        :param abort_on_invalid:
+            If ``True`` one invalid parameter means any other parameter in the
+            request will also not be added to the subscription.
+        :param send_from_cache:
+            If ``True`` the last processed parameter value is sent from
+            parameter cache. When ``False`` only newly processed parameters
+            are received.
         """
         if not parameters:
             return
 
         options = processing_pb2.SubscribeParametersRequest()
         options.action = processing_pb2.SubscribeParametersRequest.ADD
         options.abortOnInvalid = abort_on_invalid
         options.sendFromCache = send_from_cache
         options.id.extend(to_named_object_ids(parameters))
 
         self._manager.send(options)
 
-    def remove(self, parameters):
+    def remove(self, parameters: Union[str, List[str]]):
         """
         Remove one or more parameters from this subscription.
 
-        :param parameters: Parameter(s) to be removed
-        :type parameters: Union[str, str[]]
+        :param parameters:
+            Parameter(s) to be removed
         """
         if not parameters:
             return
 
         options = processing_pb2.SubscribeParametersRequest()
         options.action = processing_pb2.SubscribeParametersRequest.REMOVE
         options.id.extend(to_named_object_ids(parameters))
 
         self._manager.send(options)
 
-    def get_value(self, parameter):
+    def get_value(self, parameter: str):
         """
         Returns the last value of a specific parameter from local cache.
 
-        :param string parameter: Parameter name.
-        :rtype: .ParameterValue
+        :param parameter:
+            Parameter name.
         """
         return self.value_cache[parameter]
 
     def _process(self, pb):
         # Mapping is only set on the first reply, or whenever
         # the subscription is modifed. Store it in an internal
         # reference, so that we can find it back when receiving
@@ -411,48 +417,63 @@
         super(CommandConnection, self).__init__(manager)
         self._cmdhist_cache = {}
         self._command_cache = {}
         self._tmtc_client = tmtc_client
 
     def issue(
         self,
-        command,
-        args=None,
-        dry_run=False,
-        comment=None,
-        verification=None,
-        extra=None,
-        beta_args_v2=False,
-    ):
+        command: str,
+        args: Optional[Mapping[str, Any]] = None,
+        dry_run: bool = False,
+        comment: Optional[str] = None,
+        verification: Optional[VerificationConfig] = None,
+        extra: Optional[Mapping[str, Any]] = None,
+        sequence_number: Optional[int] = None,
+    ) -> MonitoredCommand:
         """
         Issue the given command
 
-        :param str command: Either a fully-qualified XTCE name or an alias in the
-                            format ``NAMESPACE/NAME``.
-        :param dict args: Named arguments (if the command requires these)
-        :param bool dry_run: If ``True`` the command is not actually issued. This
-                             can be used to test if the server would generate
-                             errors when preparing the command (for example
-                             because an argument is missing).
-        :param str comment: Comment attached to the command.
-        :param .VerificationConfig verification: Overrides to the default
-                                                 verification handling of this
-                                                 command.
-        :param dict extra: Extra command options for interpretation by non-core
-                           extensions (custom preprocessor, datalinks, command
-                           listeners).
-                           Note that Yamcs will refuse command options that it
-                           does now know about. Extensions should therefore
-                           register available options.
-        :return: An object providing access to properties of the newly issued
-                 command and updated according to command history updates.
-        :rtype: .MonitoredCommand
+        :param command:
+            Either a fully-qualified XTCE name or an alias in the
+            format ``NAMESPACE/NAME``.
+        :param args:
+            Named arguments (if the command requires these).
+        :param dry_run:
+            If ``True`` the command is not actually issued. This can be used
+            to test if the server would generate errors when preparing the
+            command (for example because an argument is missing).
+        :param comment:
+            Comment attached to the command.
+        :param verification:
+            Overrides to the default verification handling of this command.
+        :param extra:
+            Extra command options for interpretation by non-core extensions
+            (custom preprocessor, datalinks, command listeners). Note that
+            Yamcs will refuse command options that it does now know about.
+            Extensions should therefore register available options.
+        :param sequence_number:
+            Sequence number of this command. This is used to determine unicity
+            of commands at the same time and coming from the same origin. If
+            not set Yamcs will automatically assign a sequential number as if
+            every submitted command is unique.
+
+            .. versionadded:: 1.9.0
+
+        :return:
+            An object providing access to properties of the newly issued
+            command and updated according to command history updates.
         """
         issued_command = self._tmtc_client.issue_command(
-            command, args, dry_run, comment, verification, extra, beta_args_v2
+            command,
+            args,
+            dry_run,
+            comment,
+            verification,
+            extra,
+            sequence_number=sequence_number,
         )
         command = MonitoredCommand(issued_command._proto)
 
         self._command_cache[command.id] = command
 
         # It may be that we already received some cmdhist updates
         # before the http response returned.
@@ -487,62 +508,64 @@
 
     def __init__(self, manager):
         super(AlarmSubscription, self).__init__(manager)
 
         self._cache = {}
         """Value cache keyed by alarm name."""
 
-    def get_alarm(self, name):
+    def get_alarm(self, name: str) -> Alarm:
         """
         Returns the alarm state associated with a specific named
         alarm from local cache.
 
-        :param str name: Fully-qualified name
-        :rtype: .Alarm
+        :param name:
+            Fully-qualified name
         """
         return self._cache[name]
 
-    def list_alarms(self):
+    def list_alarms(self) -> List[Alarm]:
         """
         Returns a snapshot of all active alarms.
-
-        :rtype: .Alarm[]
         """
         return [self._cache[k] for k in self._cache]
 
     def _process(self, alarm_update):
         alarm = alarm_update.alarm
         if alarm.is_process_ok and not alarm.is_ok and alarm.is_acknowledged:
             del self._cache[alarm.name]
         else:
             self._cache[alarm.name] = alarm
 
 
 class ProcessorClient:
     """Client object that groups operations linked to a specific processor."""
 
-    def __init__(self, ctx, instance, processor):
+    def __init__(self, ctx: Context, instance: str, processor: str):
         super(ProcessorClient, self).__init__()
         self.ctx = ctx
         self._instance = instance
         self._processor = processor
 
-    def get_parameter_value(self, parameter, from_cache=True, timeout=10):
+    def get_parameter_value(
+        self, parameter: str, from_cache: bool = True, timeout: float = 10
+    ) -> Optional[ParameterValue]:
         """
         Retrieve the current value of the specified parameter.
 
-        :param str parameter: Either a fully-qualified XTCE name or an alias in the
-                              format ``NAMESPACE/NAME``.
-        :param bool from_cache: If ``False`` this call will block until a
-                                fresh value is received on the processor.
-                                If ``True`` the server returns the latest
-                                value instead (which may be ``None``).
-        :param float timeout: The amount of seconds to wait for a fresh value.
-                              (ignored if ``from_cache=True``).
-        :rtype: .ParameterValue
+        :param parameter:
+            Either a fully-qualified XTCE name or an alias in the
+            format ``NAMESPACE/NAME``.
+        :param from_cache:
+            If ``False`` this call will block until a
+            fresh value is received on the processor.
+            If ``True`` the server returns the latest
+            value instead (which may be ``None``).
+        :param timeout:
+            The amount of seconds to wait for a fresh value.
+            (ignored if ``from_cache=True``).
         """
         params = {
             "fromCache": from_cache,
             "timeout": int(timeout * 1000),
         }
         parameter = adapt_name_for_rest(parameter)
         url = f"/processors/{self._instance}/{self._processor}/parameters{parameter}"
@@ -552,31 +575,36 @@
 
         # Server returns ParameterValue with only 'id' set if no
         # value existed. Convert this to ``None``.
         if proto.HasField("rawValue") or proto.HasField("engValue"):
             return ParameterValue(proto)
         return None
 
-    def get_parameter_values(self, parameters, from_cache=True, timeout=10):
+    def get_parameter_values(
+        self, parameters: List[str], from_cache: bool = True, timeout: float = 10
+    ) -> List[Optional[ParameterValue]]:
         """
         Retrieve the current value of the specified parameter.
 
-        :param str[] parameters: List of parameter names. These may be
-                                 fully-qualified XTCE name or an alias
-                                 in the format ``NAMESPACE/NAME``.
-        :param bool from_cache: If ``False`` this call will block until
-                                fresh values are received on the processor.
-                                If ``True`` the server returns the latest
-                                value instead (which may be ``None``).
-        :param float timeout: The amount of seconds to wait for a fresh
-                              values (ignored if ``from_cache=True``).
-        :return: A list that matches the length and order of the requested
-                 list of parameters. Each entry contains either the
-                 returned parameter value, or ``None``.
-        :rtype: .ParameterValue[]
+        :param parameters:
+            List of parameter names. These may be
+            fully-qualified XTCE name or an alias
+            in the format ``NAMESPACE/NAME``.
+        :param from_cache:
+            If ``False`` this call will block until
+            fresh values are received on the processor.
+            If ``True`` the server returns the latest
+            value instead (which may be ``None``).
+        :param timeout:
+            The amount of seconds to wait for a fresh
+            values (ignored if ``from_cache=True``).
+        :return:
+            A list that matches the length and order of the requested
+            list of parameters. Each entry contains either the
+            returned parameter value, or ``None``.
         """
         req = processing_pb2.BatchGetParameterValuesRequest()
         req.id.extend(to_named_object_ids(parameters))
         req.fromCache = from_cache
         req.timeout = int(timeout * 1000)
         url = f"/processors/{self._instance}/{self._processor}/parameters:batchGet"
         response = self.ctx.post_proto(url, data=req.SerializeToString())
@@ -589,46 +617,58 @@
             for pval in proto.value:
                 if pval.id == parameter_id:
                     match = pval
                     break
             pvals.append(ParameterValue(match) if match else None)
         return pvals
 
-    def set_parameter_value(self, parameter, value, generation_time=None):
+    def set_parameter_value(
+        self,
+        parameter: str,
+        value: Any,
+        generation_time: Optional[datetime.datetime] = None,
+    ):
         """
         Sets the value of the specified parameter.
 
-        :param str parameter: Either a fully-qualified XTCE name or an alias in the
-                              format ``NAMESPACE/NAME``.
-        :param value: The value to set
-        :param generation_time: Generation time of the values. If unset, Yamcs will
-                                assign the generation time.
-        :type generation_time: Optional[~datetime.datetime]
+        :param parameter:
+            Either a fully-qualified XTCE name or an alias in the format
+            ``NAMESPACE/NAME``.
+        :param value:
+            The value to set.
+        :param generation_time:
+            Generation time of the value. If unset, Yamcs will assign the
+            generation time.
         """
         self.set_parameter_values({parameter: value}, generation_time)
 
-    def set_parameter_values(self, values, generation_time=None):
+    def set_parameter_values(
+        self,
+        values: Mapping[str, Any],
+        generation_time: Optional[datetime.datetime] = None,
+    ):
         """
         Sets the value of multiple parameters.
 
         Values are specified with their native Python types. If you need
-        to customize individual value generation times, use :class:`.ValueUpdate`
-        instead.
+        to customize individual value generation times, use
+        :class:`.ValueUpdate` instead.
 
         The method argument ``generation_time`` can be used to specify a custom
         generation time for all values at once. This has lower priority than
         a value-specific generation time.
 
         If no generation time is specified at all, Yamcs will determine one.
 
-        :param dict values: Values keyed by parameter name. This name can be either
-                            a fully-qualified XTCE name or an alias in the format
-                            ``NAMESPACE/NAME``.
-        :param generation_time: Generation time of the values.
-        :type generation_time: Optional[~datetime.datetime]
+        :param values:
+            Values keyed by parameter name. This name can be either a
+            fully-qualified XTCE name or an alias in the format
+            ``NAMESPACE/NAME``.
+        :param generation_time:
+            Generation time of the values.
         """
         req = processing_pb2.BatchSetParameterValuesRequest()
         for key in values:
             item = req.request.add()
             item.id.MergeFrom(to_named_object_id(key))
 
             value = values[key]
@@ -642,61 +682,65 @@
             if value_time:
                 item.generationTime.MergeFrom(to_server_time(value_time))
         url = f"/processors/{self._instance}/{self._processor}/parameters:batchSet"
         self.ctx.post_proto(url, data=req.SerializeToString())
 
     def issue_command(
         self,
-        command,
-        args=None,
-        dry_run=False,
-        comment=None,
-        verification=None,
-        extra=None,
-        beta_args_v2=False,
-    ):
+        command: str,
+        args: Optional[Mapping[str, Any]] = None,
+        dry_run: bool = False,
+        comment: Optional[str] = None,
+        verification: Optional[VerificationConfig] = None,
+        extra: Optional[Mapping[str, Any]] = None,
+        sequence_number: Optional[int] = None,
+    ) -> IssuedCommand:
         """
         Issue the given command
 
-        :param str command: Either a fully-qualified XTCE name or an alias in the
-                            format ``NAMESPACE/NAME``.
-        :param dict args: named arguments (if the command requires these)
-        :param bool dry_run: If ``True`` the command is not actually issued. This
-                             can be used to test if the server would generate
-                             errors when preparing the command (for example
-                             because an argument is missing).
-        :param str comment: Comment attached to the command.
-        :param .VerificationConfig verification: Overrides to the default
-                                                 verification handling of this
-                                                 command.
-        :param dict extra: Extra command options for interpretation by non-core
-                           extensions (custom preprocessor, datalinks, command
-                           listeners).
-                           Note that Yamcs will refuse command options that it
-                           does now know about. Extensions should therefore
-                           register available options.
-        :return: An object providing access to properties of the newly issued
-                 command.
-        :rtype: .IssuedCommand
+        :param command:
+            Either a fully-qualified XTCE name or an alias in the format
+            ``NAMESPACE/NAME``.
+        :param args:
+            Named arguments (if the command requires any).
+        :param dry_run:
+            If ``True`` the command is not actually issued. This can be used
+            to test if the server would generate errors when preparing the
+            command (for example because an argument is missing).
+        :param comment:
+            Comment attached to the command.
+        :param verification:
+            Overrides to the default verification handling of this command.
+        :param extra:
+            Extra command options for interpretation by non-core
+            extensions (custom preprocessor, datalinks, command listeners).
+            Note that Yamcs will refuse command options that it does now know
+            about. Extensions should therefore register available options.
+        :param sequence_number:
+            Sequence number of this command. This is used
+            to determine unicity of commands at the same time and coming from
+            the same origin. If not set Yamcs will automatically assign a
+            sequential number as if every submitted command is unique.
+
+            .. versionadded:: 1.9.0
+
+        :return:
+            An object providing access to properties of the newly issued
+            command.
         """
         req = commands_service_pb2.IssueCommandRequest()
         req.sequenceNumber = SequenceGenerator.next()
         req.dryRun = dry_run
         if comment:
             req.comment = comment
-        if beta_args_v2:
-            for key in beta_args_v2:
-                req.args[key] = _to_argument_value(
-                    beta_args_v2[key], force_string=False
-                )
-        elif args:
+        if sequence_number is not None:
+            req.sequenceNumber = sequence_number
+        if args:
             for key in args:
-                assignment = req.assignment.add()
-                assignment.name = key
-                assignment.value = _to_argument_value(args[key], force_string=True)
+                req.args[key] = _to_argument_value(args[key], force_string=True)
 
         if verification:
             if verification._disable_all:
                 req.disableVerifiers = True
             else:
                 for verifier in verification._disabled:
                     req.verifierConfig[verifier].disable = True
@@ -720,26 +764,29 @@
         command = adapt_name_for_rest(command)
         url = f"/processors/{self._instance}/{self._processor}/commands{command}"
         response = self.ctx.post_proto(url, data=req.SerializeToString())
         proto = commands_service_pb2.IssueCommandResponse()
         proto.ParseFromString(response.content)
         return IssuedCommand(proto)
 
-    def list_alarms(self, start=None, stop=None):
+    def list_alarms(
+        self,
+        start: Optional[datetime.datetime] = None,
+        stop: Optional[datetime.datetime] = None,
+    ) -> Iterable[Alarm]:
         """
         Lists the active alarms.
 
         Remark that this does not query the archive. Only active alarms on the
         current processor are returned.
 
-        :param ~datetime.datetime start: Minimum trigger time of the returned alarms
-                                         (inclusive)
-        :param ~datetime.datetime stop: Maximum trigger time of the returned alarms
-                                        (exclusive)
-        :rtype: ~collections.abc.Iterable[.Alarm]
+        :param start:
+            Minimum trigger time of the returned alarms (inclusive)
+        :param stop:
+            Maximum trigger time of the returned alarms (exclusive)
         """
         # TODO implement continuation token on server
         params = {"order": "asc"}
         if start is not None:
             params["start"] = to_isostring(start)
         if stop is not None:
             params["stop"] = to_isostring(stop)
@@ -748,15 +795,15 @@
         url = f"/processors/{self._instance}/{self._processor}/alarms"
         response = self.ctx.get_proto(path=url, params=params)
         message = alarms_service_pb2.ListAlarmsResponse()
         message.ParseFromString(response.content)
         alarms = getattr(message, "alarms")
         return iter([_parse_alarm(alarm) for alarm in alarms])
 
-    def set_default_calibrator(self, parameter, type, data):
+    def set_default_calibrator(self, parameter: str, type: str, data):
         """
         Apply a calibrator while processing raw values of the specified
         parameter. If there is already a default calibrator associated
         to this parameter, that calibrator gets replaced.
 
         .. note::
 
@@ -771,47 +818,51 @@
           The `data` argument must be an array of floats ``[a, b, c, ...]``.
 
         * Spline calibrators interpolate the raw value between a set of points
           which represent a linear curve.
 
           The `data` argument must be an array of ``[x, y]`` points.
 
-        :param str parameter: Either a fully-qualified XTCE name or an alias
-                              in the format ``NAMESPACE/NAME``.
-        :param str type: One of ``polynomial`` or ``spline``.
-        :param data: Calibration definition for the selected type.
+        :param parameter:
+            Either a fully-qualified XTCE name or an alias in the format
+            ``NAMESPACE/NAME``.
+        :param type:
+            One of ``polynomial`` or ``spline``.
+        :param data:
+            Calibration definition for the selected type.
         """
         req = mdb_override_service_pb2.UpdateParameterRequest()
         req.action = (
             mdb_override_service_pb2.UpdateParameterRequest.SET_DEFAULT_CALIBRATOR
         )
         if type:
             _add_calib(req.defaultCalibrator, type, data)
 
         parameter = adapt_name_for_rest(parameter)
         url = f"/mdb/{self._instance}/{self._processor}/parameters{parameter}"
         self.ctx.patch_proto(url, data=req.SerializeToString())
 
-    def set_calibrators(self, parameter, calibrators):
+    def set_calibrators(self, parameter: str, calibrators: List[Calibrator]):
         """
         Apply an ordered set of calibrators for the specified parameter.
         This replaces existing calibrators (if any).
 
         Each calibrator may have a context, which indicates when it its
         effects may be applied. Only the first matching calibrator is
         applied.
 
         A calibrator with context ``None`` is the *default* calibrator.
         There can be only one such calibrator, and is always applied at
         the end when no other contextual calibrator was applicable.
 
-        :param str parameter: Either a fully-qualified XTCE name or an alias
-                              in the format ``NAMESPACE/NAME``.
-        :param .Calibrator[] calibrators: List of calibrators (either contextual or
-                                          not)
+        :param parameter:
+            Either a fully-qualified XTCE name or an alias in the format
+            ``NAMESPACE/NAME``.
+        :param calibrators:
+            List of calibrators (either contextual or not)
         """
         req = mdb_override_service_pb2.UpdateParameterRequest()
         req.action = mdb_override_service_pb2.UpdateParameterRequest.SET_CALIBRATORS
         for c in calibrators:
             if c.context:
                 context_calib = req.contextCalibrator.add()
                 context_calib.context = c.context
@@ -821,68 +872,74 @@
 
             _add_calib(calib_info, c.type, c.data)
 
         parameter = adapt_name_for_rest(parameter)
         url = f"/mdb/{self._instance}/{self._processor}/parameters{parameter}"
         self.ctx.patch_proto(url, data=req.SerializeToString())
 
-    def clear_calibrators(self, parameter):
+    def clear_calibrators(self, parameter: str):
         """
         Removes all calibrators for the specified parameter.
         """
         self.set_default_calibrator(parameter, None, None)
         self.set_calibrators(parameter, [])
 
-    def reset_calibrators(self, parameter):
+    def reset_calibrators(self, parameter: str):
         """
         Reset all calibrators for the specified parameter to their original MDB value.
         """
         req = mdb_override_service_pb2.UpdateParameterRequest()
         req.action = mdb_override_service_pb2.UpdateParameterRequest.RESET_CALIBRATORS
 
         parameter = adapt_name_for_rest(parameter)
         url = f"/mdb/{self._instance}/{self._processor}/parameters{parameter}"
         self.ctx.patch_proto(url, data=req.SerializeToString())
 
     def set_default_alarm_ranges(
         self,
-        parameter,
-        watch=None,
-        warning=None,
-        distress=None,
-        critical=None,
-        severe=None,
-        min_violations=1,
+        parameter: str,
+        watch: Optional[Tuple[float, float]] = None,
+        warning: Optional[Tuple[float, float]] = None,
+        distress: Optional[Tuple[float, float]] = None,
+        critical: Optional[Tuple[float, float]] = None,
+        severe: Optional[Tuple[float, float]] = None,
+        min_violations: int = 1,
     ):
         """
         Generate out-of-limit alarms for a parameter using the specified
         alarm ranges.
 
         This replaces any previous default alarms on this parameter.
 
         .. note::
 
             Contextual range sets take precedence over the default alarm
             ranges. See :meth:`set_alarm_range_sets` for setting contextual
             range sets.
 
-        :param str parameter: Either a fully-qualified XTCE name or an alias
-                              in the format ``NAMESPACE/NAME``.
-        :param (float,float) watch: Range expressed as a tuple ``(lo, hi)``
-                                    where lo and hi are assumed exclusive.
-        :param (float,float) warning: Range expressed as a tuple ``(lo, hi)``
-                                      where lo and hi are assumed exclusive.
-        :param (float,float) distress: Range expressed as a tuple ``(lo, hi)``
-                                       where lo and hi are assumed exclusive.
-        :param (float,float) critical: Range expressed as a tuple ``(lo, hi)``
-                                       where lo and hi are assumed exclusive.
-        :param (float,float) severe: Range expressed as a tuple ``(lo, hi)``
-                                     where lo and hi are assumed exclusive.
-        :param int min_violations: Minimum violations before an alarm is
-                                   generated.
+        :param parameter:
+            Either a fully-qualified XTCE name or an alias in the format
+            ``NAMESPACE/NAME``.
+        :param watch:
+            Range expressed as a tuple ``(lo, hi)`` where lo and hi are
+            assumed exclusive.
+        :param warning:
+            Range expressed as a tuple ``(lo, hi)`` where lo and hi are
+            assumed exclusive.
+        :param distress:
+            Range expressed as a tuple ``(lo, hi)`` where lo and hi are
+            assumed exclusive.
+        :param critical:
+            Range expressed as a tuple ``(lo, hi)`` where lo and hi are
+            assumed exclusive.
+        :param severe:
+            Range expressed as a tuple ``(lo, hi)`` where lo and hi are
+            assumed exclusive.
+        :param min_violations:
+            Minimum violations before an alarm is generated.
         """
         req = mdb_override_service_pb2.UpdateParameterRequest()
         req.action = mdb_override_service_pb2.UpdateParameterRequest.SET_DEFAULT_ALARMS
         if watch or warning or distress or critical or severe:
             _add_alarms(
                 req.defaultAlarm,
                 watch,
@@ -893,31 +950,33 @@
                 min_violations,
             )
 
         parameter = adapt_name_for_rest(parameter)
         url = f"/mdb/{self._instance}/{self._processor}/parameters{parameter}"
         self.ctx.patch_proto(url, data=req.SerializeToString())
 
-    def set_alarm_range_sets(self, parameter, sets):
+    def set_alarm_range_sets(self, parameter: str, sets: List[RangeSet]):
         """
         Apply an ordered list of alarm range sets for the specified parameter.
         This replaces existing alarm sets (if any).
 
         Each RangeSet may have a context, which indicates when
         its effects may be applied. Only the first matching set is
         applied.
 
         A RangeSet with context ``None`` represents the *default* set of
         alarm ranges.  There can be only one such set, and it is always
         applied at the end when no other set of contextual ranges is
         applicable.
 
-        :param str parameter: Either a fully-qualified XTCE name or an alias
-                              in the format ``NAMESPACE/NAME``.
-        :param .RangeSet[] sets: List of range sets (either contextual or not)
+        :param parameter:
+            Either a fully-qualified XTCE name or an alias in the format
+            ``NAMESPACE/NAME``.
+        :param sets:
+            List of range sets (either contextual or not)
         """
         req = mdb_override_service_pb2.UpdateParameterRequest()
         req.action = mdb_override_service_pb2.UpdateParameterRequest.SET_ALARMS
         for rs in sets:
             if rs.context:
                 context_alarm = req.contextAlarm.add()
                 context_alarm.context = rs.context
@@ -935,121 +994,143 @@
                 rs.min_violations,
             )
 
         parameter = adapt_name_for_rest(parameter)
         url = f"/mdb/{self._instance}/{self._processor}/parameters{parameter}"
         self.ctx.patch_proto(url, data=req.SerializeToString())
 
-    def clear_alarm_ranges(self, parameter):
+    def clear_alarm_ranges(self, parameter: str):
         """
         Removes all alarm limits for the specified parameter.
         """
         self.set_default_alarm_ranges(parameter)
         self.set_alarm_range_sets(parameter, [])
 
-    def reset_alarm_ranges(self, parameter):
+    def reset_alarm_ranges(self, parameter: str):
         """
-        Reset all alarm limits for the specified parameter to their original MDB value.
+        Reset all alarm limits for the specified parameter to their original
+        MDB value.
         """
         req = mdb_override_service_pb2.UpdateParameterRequest()
         req.action = mdb_override_service_pb2.UpdateParameterRequest.RESET_ALARMS
 
         parameter = adapt_name_for_rest(parameter)
         url = f"/mdb/{self._instance}/{self._processor}/parameters{parameter}"
         self.ctx.patch_proto(url, data=req.SerializeToString())
 
-    def acknowledge_alarm(self, alarm, comment=None):
+    def acknowledge_alarm(
+        self, alarm: str, sequence_number: int, comment: Optional[str] = None
+    ):
         """
         Acknowledges a specific alarm.
 
-        :param alarm: Alarm instance
-        :type alarm: :class:`.Alarm`
-        :param str comment: Optional comment to associate with the state
-                            change.
+        :param alarm:
+            Alarm name
+        :param sequence_number:
+            Sequence number
+        :param comment:
+            Optional comment to associate with the state change.
         """
-        name = adapt_name_for_rest(alarm.name)
+        name = adapt_name_for_rest(alarm)
         url = f"/processors/{self._instance}/{self._processor}"
-        url += f"/alarms{name}/{alarm.sequence_number}:acknowledge"
+        url += f"/alarms{name}/{sequence_number}:acknowledge"
         req = alarms_service_pb2.AcknowledgeAlarmRequest()
         if comment is not None:
             req.comment = comment
         self.ctx.post_proto(url, data=req.SerializeToString())
 
-    def unshelve_alarm(self, alarm, comment=None):
+    def unshelve_alarm(
+        self, alarm: str, sequence_number: int, comment: Optional[str] = None
+    ):
         """
         Unshelve an alarm.
 
-        :param alarm: Alarm instance
-        :type alarm: :class:`.Alarm`
-        :param str comment: Optional comment to associate with the state
-                            change.
+        :param alarm:
+            Alarm name
+        :param sequence_number:
+            Sequence number
+        :param comment:
+            Optional comment to associate with the state change.
         """
-        name = adapt_name_for_rest(alarm.name)
+        name = adapt_name_for_rest(alarm)
         url = f"/processors/{self._instance}/{self._processor}"
-        url += f"/alarms{name}/{alarm.sequence_number}:unshelve"
+        url += f"/alarms{name}/{sequence_number}:unshelve"
         req = alarms_service_pb2.UnshelveAlarmRequest()
         self.ctx.post_proto(url, data=req.SerializeToString())
 
-    def shelve_alarm(self, alarm, comment=None):
+    def shelve_alarm(
+        self, alarm: str, sequence_number: int, comment: Optional[str] = None
+    ):
         """
         Shelve an alarm.
 
-        :param alarm: Alarm instance
-        :type alarm: :class:`.Alarm`
-        :param str comment: Optional comment to associate with the state
-                            change.
+        :param alarm:
+            Alarm name
+        :param sequence_number:
+            Sequence number
+        :param comment:
+            Optional comment to associate with the state change.
         """
-        name = adapt_name_for_rest(alarm.name)
+        name = adapt_name_for_rest(alarm)
         url = f"/processors/{self._instance}/{self._processor}"
-        url += f"/alarms{name}/{alarm.sequence_number}:shelve"
+        url += f"/alarms{name}/{sequence_number}:shelve"
         req = alarms_service_pb2.ShelveAlarmRequest()
         if comment is not None:
             req.comment = comment
         self.ctx.post_proto(url, data=req.SerializeToString())
 
-    def clear_alarm(self, alarm, comment=None):
+    def clear_alarm(
+        self, alarm: str, sequence_number: int, comment: Optional[str] = None
+    ):
         """
         Clear an alarm.
 
         .. note::
             If the reason that caused the alarm is still present, a new
             alarm instance will be generated.
 
-        :param alarm: Alarm instance
-        :type alarm: :class:`.Alarm`
-        :param str comment: Optional comment to associate with the state
-                            change.
+        :param alarm:
+            Alarm name
+        :param sequence_number:
+            Sequence number
+        :param comment:
+            Optional comment to associate with the state change.
         """
-        name = adapt_name_for_rest(alarm.name)
+        name = adapt_name_for_rest(alarm)
         url = f"/processors/{self._instance}/{self._processor}"
-        url += f"/alarms{name}/{alarm.sequence_number}:clear"
+        url += f"/alarms{name}/{sequence_number}:clear"
         req = alarms_service_pb2.ClearAlarmRequest()
         if comment is not None:
             req.comment = comment
         self.ctx.post_proto(url, data=req.SerializeToString())
 
-    def create_command_connection(self, on_data=None, timeout=60):
+    def create_command_connection(
+        self,
+        on_data: Optional[Callable[[CommandHistory], None]] = None,
+        timeout: float = 60,
+    ) -> CommandConnection:
         """
         Creates a connection for issuing multiple commands and
         following up on their acknowledgment progress.
 
         .. note::
             This is a convenience method that merges the functionalities
             of :meth:`create_command_history_subscription` with those of
             :meth:`issue_command`.
 
-        :param on_data: Function that gets called with  :class:`.CommandHistory`
-                        updates. Only commands issued from this connection are
-                        reported.
-        :param timeout: The amount of seconds to wait for the request to
-                        complete.
-        :type timeout: float
-        :return: Future that can be used to manage the background websocket
-                 subscription
-        :rtype: .CommandConnection
+        :param on_data:
+            Function that gets called with  :class:`.CommandHistory`
+            updates. Only commands issued from this connection are
+            reported.
+        :param timeout:
+            The amount of seconds to wait for the request to complete.
+
+        :return:
+            Future that can be used to manage the background websocket
+            subscription
         """
         options = commands_service_pb2.SubscribeCommandsRequest()
         options.instance = self._instance
         options.processor = self._processor
         options.ignorePastCommands = True
 
         manager = WebSocketSubscriptionManager(
@@ -1066,26 +1147,29 @@
         manager.open(wrapped_callback)
 
         # Wait until a reply or exception is received
         subscription.reply(timeout=timeout)
 
         return subscription
 
-    def create_command_history_subscription(self, on_data=None, timeout=60):
+    def create_command_history_subscription(
+        self,
+        on_data: Optional[Callable[[CommandHistory], None]] = None,
+        timeout: float = 60,
+    ) -> CommandHistorySubscription:
         """
         Create a new command history subscription.
 
-        :param on_data: (Optional) Function that gets called with
-                        :class:`.CommandHistory` updates.
-        :param timeout: The amount of seconds to wait for the request to
-                        complete.
-        :type timeout: float
-        :return: Future that can be used to manage the background websocket
-                 subscription
-        :rtype: .CommandHistorySubscription
+        :param on_data:
+            Function that gets called with :class:`.CommandHistory` updates.
+        :param timeout:
+            The amount of seconds to wait for the request to complete.
+        :return:
+            Future that can be used to manage the background websocket
+            subscription.
         """
         options = commands_service_pb2.SubscribeCommandsRequest()
         options.instance = self._instance
         options.processor = self._processor
         options.ignorePastCommands = True
 
         manager = WebSocketSubscriptionManager(
@@ -1102,41 +1186,42 @@
         manager.open(wrapped_callback)
 
         # Wait until a reply or exception is received
         subscription.reply(timeout=timeout)
 
         return subscription
 
-    def create_packet_subscription(self, on_data, stream="tm_realtime", timeout=60):
+    def create_packet_subscription(
+        self,
+        on_data: Callable[[Packet], None],
+        stream: Optional[str] = None,
+        timeout: float = 60,
+    ) -> WebSocketSubscriptionFuture:
         """
         Create a new packet subscription.
 
         .. versionadded:: 1.6.6
 
-        :param on_data: Function that gets called with :class:`.Packet`
-                        updates.
-        :type on_data: Optional[Callable[.Packet]]
-        :param stream: Stream to subscribe to.
-        :type stream: str
-        :param timeout: The amount of seconds to wait for the request
-                        to complete.
-        :type timeout: Optional[float]
-        :return: A Future that can be used to manage the background websocket
-                 subscription.
-        :rtype: .WebSocketSubscriptionFuture
+        :param on_data:
+            Function that gets called with :class:`.Packet` updates.
+        :param stream:
+            Stream to subscribe to.
+        :param timeout:
+            The amount of seconds to wait for the request to complete.
+        :return:
+            A Future that can be used to manage the background websocket
+            subscription.
         """
         options = packets_service_pb2.SubscribePacketsRequest()
         options.instance = self._instance
 
-        # TODO remove stream default to tm_realtime within a few releases.
-        # (processor option only added as of Yamcs 5.5.x)
-        # if stream:
-        options.stream = stream
-        # else:
-        #    options.processor = self._processor
+        if stream:
+            options.stream = stream
+        else:
+            options.processor = self._processor
 
         manager = WebSocketSubscriptionManager(
             self.ctx, topic="packets", options=options
         )
 
         # Represent subscription as a future
         subscription = WebSocketSubscriptionFuture(manager)
@@ -1146,32 +1231,35 @@
         manager.open(wrapped_callback)
 
         # Wait until a reply or exception is received
         subscription.reply(timeout=timeout)
 
         return subscription
 
-    def create_container_subscription(self, containers, on_data=None, timeout=60):
+    def create_container_subscription(
+        self,
+        containers: Union[str, List[str]],
+        on_data: Optional[Callable[[ContainerData], None]] = None,
+        timeout: float = 60,
+    ) -> ContainerSubscription:
         """
         Create a new container subscription.
 
         .. versionadded:: 1.7.0
            Compatible with Yamcs 5.5.0 onwards
 
-        :param containers: Container names.
-        :type containers: Union[str, str[]]
-        :param on_data: Function that gets called with :class:`.ContainerData`
-                        updates.
-        :type on_data: Optional[Callable[.ContainerData]]
-        :param timeout: The amount of seconds to wait for the request
-                        to complete.
-        :type timeout: Optional[float]
-        :return: A Future that can be used to manage the background websocket
-                 subscription.
-        :rtype: .ContainerSubscription
+        :param containers:
+            Container names.
+        :param on_data:
+            Function that gets called with :class:`.ContainerData` updates.
+        :param timeout:
+            The amount of seconds to wait for the request to complete.
+        :return:
+            A Future that can be used to manage the background websocket
+            subscription.
         """
         options = packets_service_pb2.SubscribeContainersRequest()
         options.instance = self._instance
         options.processor = self._processor
         if isinstance(containers, str):
             options.names.extend([containers])
         else:
@@ -1193,45 +1281,45 @@
         # Wait until a reply or exception is received
         subscription.reply(timeout=timeout)
 
         return subscription
 
     def create_parameter_subscription(
         self,
-        parameters,
-        on_data=None,
-        abort_on_invalid=True,
-        update_on_expiration=False,
-        send_from_cache=True,
-        timeout=60,
-    ):
+        parameters: Union[str, List[str]],
+        on_data: Optional[Callable[[ParameterData], None]] = None,
+        abort_on_invalid: bool = True,
+        update_on_expiration: bool = False,
+        send_from_cache: bool = True,
+        timeout: float = 60,
+    ) -> ParameterSubscription:
         """
         Create a new parameter subscription.
 
-        :param str[] parameters: Parameter names (or aliases).
-        :param on_data: (Optional) Function that gets called with
-                        :class:`.ParameterData` updates.
-        :param bool abort_on_invalid: If ``True`` an error is generated when
-                                      invalid parameters are specified.
-        :param bool update_on_expiration: If ``True`` an update is received
-                                          when a parameter value has become
-                                          expired. This update holds the
-                                          same value as the last known valid
-                                          value, but with status set to
-                                          ``EXPIRED``.
-        :param bool send_from_cache: If ``True`` the last processed parameter
-                                     value is sent from parameter cache.
-                                     When ``False`` only newly processed
-                                     parameters are received.
-        :param float timeout: The amount of seconds to wait for the request
-                              to complete.
-
-        :return: A Future that can be used to manage the background websocket
-                 subscription.
-        :rtype: .ParameterSubscription
+        :param parameters:
+            Parameter names (or aliases).
+        :param on_data:
+            Function that gets called with :class:`.ParameterData` updates.
+        :param abort_on_invalid:
+            If ``True`` an error is generated when invalid parameters are
+            specified.
+        :param update_on_expiration:
+            If ``True`` an update is received when a parameter value has
+            become expired. This update holds the same value as the last
+            known valid value, but with status set to ``EXPIRED``.
+        :param send_from_cache:
+            If ``True`` the last processed parameter value is sent from
+            parameter cache. When ``False`` only newly processed parameters
+            are received.
+        :param timeout:
+            The amount of seconds to wait for the request to complete.
+
+        :return:
+            A Future that can be used to manage the background websocket
+            subscription.
         """
         options = processing_pb2.SubscribeParametersRequest()
         options.instance = self._instance
         options.processor = self._processor
         options.abortOnInvalid = abort_on_invalid
         options.updateOnExpiration = update_on_expiration
         options.sendFromCache = send_from_cache
@@ -1251,26 +1339,30 @@
         manager.open(wrapped_callback)
 
         # Wait until a reply or exception is received
         subscription.reply(timeout=timeout)
 
         return subscription
 
-    def create_alarm_subscription(self, on_data=None, timeout=60):
+    def create_alarm_subscription(
+        self,
+        on_data: Optional[Callable[[AlarmUpdate], None]] = None,
+        timeout: float = 60,
+    ) -> AlarmSubscription:
         """
         Create a new alarm subscription.
 
-        :param on_data: (Optional) Function that gets called with
-                        :class:`.AlarmUpdate` updates.
-        :param float timeout: The amount of seconds to wait for the request
-                              to complete.
-
-        :return: A Future that can be used to manage the background websocket
-                 subscription.
-        :rtype: .AlarmSubscription
+        :param on_data:
+            Function that gets called with :class:`.AlarmUpdate` updates.
+        :param timeout:
+            The amount of seconds to wait for the request to complete.
+
+        :return:
+            A Future that can be used to manage the background websocket
+            subscription.
         """
         options = alarms_service_pb2.SubscribeAlarmsRequest()
         options.instance = self._instance
         options.processor = self._processor
         manager = WebSocketSubscriptionManager(
             self.ctx, topic="alarms", options=options
         )
@@ -1285,37 +1377,40 @@
         manager.open(wrapped_callback)
 
         # Wait until a reply or exception is received
         subscription.reply(timeout=timeout)
 
         return subscription
 
-    def set_algorithm(self, parameter, text):
+    def set_algorithm(self, parameter: str, text: str):
         """
         Change an algorithm text. Can only be peformed on JavaScript or Python
         algorithms.
 
-        :param string text: new algorithm text (as it would appear in excel or XTCE)
-        :param str parameter: Either a fully-qualified XTCE name or an alias
-                              in the format ``NAMESPACE/NAME``.
+        :param text:
+            New algorithm text (as it would appear in excel or XTCE)
+        :param parameter:
+            Either a fully-qualified XTCE name or an alias in the format
+            ``NAMESPACE/NAME``.
         """
         req = mdb_override_service_pb2.UpdateAlgorithmRequest()
         req.action = mdb_override_service_pb2.UpdateAlgorithmRequest.SET
         req.algorithm.text = text
 
         parameter = adapt_name_for_rest(parameter)
         url = f"/mdb/{self._instance}/{self._processor}/algorithms{parameter}"
         self.ctx.patch_proto(url, data=req.SerializeToString())
 
-    def reset_algorithm(self, parameter):
+    def reset_algorithm(self, parameter: str):
         """
         Reset the algorithm text to its original definition from MDB
 
-        :param str parameter: Either a fully-qualified XTCE name or an alias
-                              in the format ``NAMESPACE/NAME``.
+        :param parameter:
+            Either a fully-qualified XTCE name or an alias in the format
+            ``NAMESPACE/NAME``.
         """
         req = mdb_override_service_pb2.UpdateAlgorithmRequest()
         req.action = mdb_override_service_pb2.UpdateAlgorithmRequest.RESET
 
         parameter = adapt_name_for_rest(parameter)
         url = f"/mdb/{self._instance}/{self._processor}/algorithms{parameter}"
         self.ctx.patch_proto(url, data=req.SerializeToString())
```

### Comparing `yamcs-client-1.8.8/src/yamcs/tmtc/model.py` & `yamcs-client-1.9.0/src/yamcs/tmtc/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import binascii
 import threading
+from abc import ABC
 from collections import OrderedDict
-from datetime import timedelta
+from datetime import datetime, timedelta
+from typing import Any, List, Optional, Tuple
 
 from yamcs.core.exceptions import TimeoutError, YamcsError
-from yamcs.core.helpers import parse_server_time, parse_value
+from yamcs.core.helpers import parse_server_time, parse_value, to_isostring
 from yamcs.model import Event
 from yamcs.protobuf.alarms import alarms_pb2
 from yamcs.protobuf.pvalue import pvalue_pb2
 
 
 def _parse_alarm(proto):
     """Converts a protobuf alarm to a specific Alarm implementation."""
     if proto.type == alarms_pb2.PARAMETER:
         return ParameterAlarm(proto)
     if proto.type == alarms_pb2.EVENT:
         return EventAlarm(proto)
-    raise YamcsError("Unexpected type " + proto.type)
+    raise YamcsError("Unexpected type " + str(proto.type))
 
 
 class Acknowledgment:
     def __init__(self, name, time, status, message):
         self.name = name
         """Name of this acknowledgment."""
 
@@ -41,123 +43,138 @@
 
     def __str__(self):
         return self.__repr__()
 
 
 class CommandHistory:
     def __init__(self, proto):
-
-        self.generation_time = parse_server_time(proto.generationTime)
-        """
-        The generation time as set by Yamcs
-
-        :type: :class:`~datetime.datetime`
-        """
+        self.generation_time: datetime = parse_server_time(proto.generationTime)
+        """The generation time as set by Yamcs"""
 
         self._proto = proto
         self.attributes = OrderedDict()
         self._update(proto.attr)
 
     @property
-    def name(self):
+    def id(self) -> str:
+        """
+        A unique identifier for this command.
+        """
+        return self._proto.id
+
+    @property
+    def name(self) -> str:
         """Name of the command."""
         return self._proto.commandName
 
     @property
-    def origin(self):
+    def origin(self) -> str:
         """
-        The origin of this command. This is often empty, but may
-        also be a hostname.
+        The origin of this command. Usually the IP address of the issuer.
         """
         if self._proto.HasField("origin"):
             return self._proto.origin
         return None
 
     @property
-    def sequence_number(self):
+    def sequence_number(self) -> int:
         """
         The sequence number of this command. This is the sequence
         number assigned by the issuing client.
         """
         if self._proto.HasField("sequenceNumber"):
             return self._proto.sequenceNumber
         return None
 
     @property
-    def username(self):
+    def username(self) -> str:
         """Username of the issuer."""
         return self.attributes.get("username")
 
     @property
-    def source(self):
+    def source(self) -> str:
         """String representation of the command."""
-        return self.attributes.get("source")
+        result = self.name + "("
+        args = []
+        for assignment in self._proto.assignments:
+            if assignment.userInput:
+                value = parse_value(assignment.value)
+                if isinstance(value, str):
+                    value = '"' + value + '"'
+                elif isinstance(value, bytes) or isinstance(value, bytearray):
+                    value = '"' + binascii.hexlify(value) + '"'
+                elif isinstance(value, datetime):
+                    value = '"' + to_isostring(value) + '"'
+                args.append(assignment.name + ": " + str(value))
+        result += ", ".join(args)
+        result += ")"
+        return result
 
     @property
     def binary(self):
         """Binary representation of the command."""
         return self.attributes.get("binary")
 
-    def is_complete(self):
+    def is_complete(self) -> bool:
         """
         Returns whether this command is complete. A command
         can be completed, yet still failed.
         """
         ack = self._assemble_ack("CommandComplete")
         return (ack is not None) and (ack.status == "OK" or ack.status == "NOK")
 
-    def is_success(self):
+    def is_success(self) -> bool:
         """
         Returns True if the command has completed successfully.
         """
         ack = self._assemble_ack("CommandComplete")
         return ack and ack.status == "OK"
 
-    def is_failure(self):
+    def is_failure(self) -> bool:
         """
         Returns True if the command has completed, but failed.
         """
         ack = self._assemble_ack("CommandComplete")
         return ack and ack.status == "NOK"
 
     @property
-    def error(self):
+    def error(self) -> Optional[str]:
         """Error message in case the command failed."""
         ack = self._assemble_ack("CommandComplete")
         if ack and ack.status == "NOK":
             return ack.message
         return None
 
     @property
-    def comment(self):
+    def comment(self) -> Optional[str]:
         """Optional user comment attached when issuing the command."""
         return self.attributes.get("comment")
 
     @property
-    def acknowledgments(self):
+    def acknowledgments(self) -> OrderedDict:
         """
         All acknowledgments by name.
 
-        :return: Acknowledgments keyed by name.
-        :rtype: ~collections.OrderedDict
+        :return:
+            Acknowledgments keyed by name.
         """
         acks = OrderedDict()
         for name, _ in self.attributes.items():
             if name.startswith("CommandComplete"):
                 continue
             if name.startswith("TransmissionConstraints"):
                 continue
             if name.endswith("_Status"):
                 ack = self._assemble_ack(name[:-7])
                 if ack:
                     acks[ack.name] = ack
 
         return acks
 
-    def _assemble_ack(self, name):
+    def _assemble_ack(self, name: str) -> Optional[Acknowledgment]:
         time = self.attributes.get(name + "_Time")
         status = self.attributes.get(name + "_Status")
         message = self.attributes.get(name + "_Message")
         if time and status:
             return Acknowledgment(name, time, status, message)
         return None
 
@@ -175,56 +192,54 @@
 
 
 class IssuedCommand:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def id(self):
+    def id(self) -> str:
         """
         A unique identifier for this command.
         """
         return self._proto.id
 
     @property
-    def name(self):
+    def name(self) -> str:
         """
         The fully-qualified name of this command.
         """
         if self._proto.HasField("commandName"):
             return self._proto.commandName
         return None
 
     @property
-    def generation_time(self):
+    def generation_time(self) -> datetime:
         """
         The generation time as set by Yamcs.
-
-        :type: :class:`~datetime.datetime`
         """
         if self._proto.HasField("generationTime"):
             return parse_server_time(self._proto.generationTime)
         return None
 
     @property
-    def username(self):
+    def username(self) -> str:
         """The username of the issuer."""
         if self._proto.HasField("username"):
             return self._proto.username
         return None
 
     @property
-    def queue(self):
+    def queue(self) -> str:
         """The name of the queue that this command was assigned to."""
         if self._proto.HasField("queue"):
             return self._proto.queue
         return None
 
     @property
-    def origin(self):
+    def origin(self) -> str:
         """
         The origin of this command. Usually the IP address of the issuer.
         """
         if self._proto.HasField("origin"):
             return self._proto.origin
         return None
 
@@ -237,17 +252,32 @@
         if self._proto.HasField("sequenceNumber"):
             return self._proto.sequenceNumber
         return None
 
     @property
     def source(self):
         """String representation of this command."""
-        if self._proto.HasField("source"):
-            return self._proto.source
-        return None
+        result = None
+        if self.name:
+            result = self.name + "("
+            args = []
+            for assignment in self._proto.assignments:
+                if assignment.userInput:
+                    value = parse_value(assignment.value)
+                    if isinstance(value, str):
+                        value = '"' + value + '"'
+                    elif isinstance(value, bytes) or isinstance(value, bytearray):
+                        value = '"' + binascii.hexlify(value) + '"'
+                    elif isinstance(value, datetime):
+                        value = '"' + to_isostring(value) + '"'
+                    args.append(assignment.name + ": " + str(value))
+            result += ", ".join(args)
+            result += ")"
+
+        return result
 
     @property
     def hex(self):
         """Hexadecimal string representation of this command."""
         if self._proto.HasField("binary"):
             return binascii.hexlify(self._proto.binary)
         return None
@@ -281,37 +311,43 @@
     """
 
     def __init__(self):
         self._disabled = []
         self._disable_all = False
         self._check_windows = {}
 
-    def disable(self, verifier=None):
+    def disable(self, verifier: Optional[str] = None):
         """
         Disable verification.
 
-        :param str verifier: Name of a specific verifier to disable. If unspecified
-                             all verifiers are disabled.
+        :param verifier:
+            Name of a specific verifier to disable. If unspecified
+            all verifiers are disabled.
         """
         if verifier:
             self._disabled.append(verifier)
         else:
             self._disable_all = True
 
-    def modify_check_window(self, verifier, start=None, stop=None):
+    def modify_check_window(
+        self, verifier: str, start: Optional[float] = None, stop: Optional[float] = None
+    ):
         """
         Set or override the check window.
 
         Depending on the Mission Database configuration,
         the time may be relative to either the command release
         or a preceding verifier.
 
-        :param str verifier: Name of the verifier
-        :param float start: Window start time (relative, in seconds)
-        :param float stop: Window stop time (relative, in seconds)
+        :param verifier:
+            Name of the verifier
+        :param start:
+            Window start time (relative, in seconds)
+        :param stop:
+            Window stop time (relative, in seconds)
         """
         self._check_windows[verifier] = {"start": start, "stop": stop}
 
 
 class MonitoredCommand(IssuedCommand):
     """
     Represent an instance of an issued command that is updated
@@ -332,132 +368,135 @@
             self._completed.set()
         for name, ack in self.acknowledgments.items():
             event = self._ack_events.setdefault(name, threading.Event())
             if ack.is_terminated():
                 event.set()
 
     @property
-    def attributes(self):
+    def attributes(self) -> OrderedDict:
         if self._cmdhist:
             return self._cmdhist.attributes
         return OrderedDict()
 
-    def is_complete(self):
+    def is_complete(self) -> bool:
         """
         Returns whether this command is complete. A command
         can be completed, yet still failed.
 
         Use :meth:`await_complete` to wait until this information
         is available.
         """
         ack = self._assemble_ack("CommandComplete")
         return (ack is not None) and (ack.status == "OK" or ack.status == "NOK")
 
-    def is_success(self):
+    def is_success(self) -> bool:
         """
         Returns True if this command was completed successfully.
 
         Use :meth:`await_complete` to wait until this information
         is available.
         """
         ack = self._assemble_ack("CommandComplete")
         return ack and ack.status == "OK"
 
-    def is_failure(self):
+    def is_failure(self) -> bool:
         """
         Returns True if the command has completed, but failed.
 
         Use :meth:`await_complete` to wait until this information
         is available.
 
         .. versionadded:: 1.8.6
         """
         ack = self._assemble_ack("CommandComplete")
         return ack and ack.status == "NOK"
 
-    def await_complete(self, timeout=None):
+    def await_complete(self, timeout: Optional[float] = None):
         """
         Wait for the command to be `completed`. Afterwards use
         :meth:`is_success` or :meth:`is_failure` to determine
         whether the command was successful or not.
 
         .. note::
 
             Yamcs cannot determine completion unless the command has
             an appropriate verifier configured in the Yamcs MDB.
 
             When no such verifier is present, this method will never
             return (or timeout).
 
-        :param float timeout: The amount of seconds to wait.
+        :param timeout:
+            The amount of seconds to wait.
         """
         self._wait_on_signal(self._completed, timeout)
 
-    def await_acknowledgment(self, name, timeout=None):
+    def await_acknowledgment(
+        self, name: str, timeout: Optional[float] = None
+    ) -> Acknowledgment:
         """
         Waits for the result of a specific acknowledgment.
 
-        :param str name: The name of the acknowledgment. Standard names are
-                         ``Acknowledge_Queued``, ``Acknowledge_Released``
-                         and ``Acknowledge_Sent``. Others depend on
-                         specific link types.
-        :param float timeout: The amount of seconds to wait.
-
-        :rtype: .Acknowledgment
+        :param name:
+            The name of the acknowledgment. Standard names are
+            ``Acknowledge_Queued``, ``Acknowledge_Released``
+            and ``Acknowledge_Sent``. Others depend on
+            specific link types.
+        :param timeout:
+            The amount of seconds to wait.
         """
         event = self._ack_events.setdefault(name, threading.Event())
         self._wait_on_signal(event, timeout)
         return self.acknowledgments.get(name)
 
-    def _wait_on_signal(self, event, timeout=None):
+    def _wait_on_signal(self, event: threading.Event, timeout: Optional[float] = None):
         if not event.wait(timeout=timeout):
             # Remark that a timeout does *not* mean that the underlying
             # work is canceled.
             raise TimeoutError("Timed out.")
 
     @property
-    def error(self):
+    def error(self) -> Optional[str]:
         """
         Error message in case the command failed.
 
         This information is only available when the command has failed
         to complete. (:meth:`is_failure` returns `True`).
         """
         ack = self._assemble_ack("CommandComplete")
         if ack and ack.status == "NOK":
             return ack.message
         return None
 
     @property
-    def comment(self):
+    def comment(self) -> Optional[str]:
         """Optional user comment attached when issuing the command."""
         return self.attributes.get("comment")
 
     @property
-    def acknowledgments(self):
+    def acknowledgments(self) -> OrderedDict:
         """
         All acknowledgments by name.
 
-        :return: Acknowledgments keyed by name.
-        :rtype: ~collections.OrderedDict
+        :return:
+            Acknowledgments keyed by name.
         """
         acks = OrderedDict()
         for name, _ in self.attributes.items():
             if name.startswith("CommandComplete"):
                 continue
             if name.startswith("TransmissionConstraints"):
                 continue
             if name.endswith("_Status"):
                 ack = self._assemble_ack(name[:-7])
                 if ack:
                     acks[ack.name] = ack
 
         return acks
 
-    def _assemble_ack(self, name):
+    def _assemble_ack(self, name: str) -> Optional[Acknowledgment]:
         time = self.attributes.get(name + "_Time")
         status = self.attributes.get(name + "_Status")
         message = self.attributes.get(name + "_Message")
         if time and status:
             return Acknowledgment(name, time, status, message)
         return None
 
@@ -479,169 +518,161 @@
     Object received through callbacks when subscribing to alarm updates.
     """
 
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def update_type(self):
+    def update_type(self) -> str:
         """Type of update."""
         return alarms_pb2.AlarmNotificationType.Name(self._proto.type)
 
     @property
-    def alarm(self):
+    def alarm(self) -> "Alarm":
         """
         Latest alarm state.
-
-        :type: :class:`.Alarm`
         """
         return _parse_alarm(self._proto)
 
     def __str__(self):
         return f"[{self.update_type}] {self.alarm}"
 
 
-class Alarm:
+class Alarm(ABC):
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Fully-qualified name of the source of this alarm."""
         if self._proto.id.HasField("namespace"):
             return self._proto.id.namespace + "/" + self._proto.id.name
         return self._proto.id.name
 
     @property
-    def trigger_time(self):
+    def trigger_time(self) -> datetime:
         """
         Processor time when the alarm was triggered.
-
-        :type: :class:`~datetime.datetime`
         """
         if self._proto.HasField("triggerTime"):
             return parse_server_time(self._proto.triggerTime)
         return None
 
     @property
-    def update_time(self):
+    def update_time(self) -> datetime:
         """
         Processor time when the alarm was last updated.
-
-        :type: :class:`~datetime.datetime`
         """
         if self._proto.HasField("updateTime"):
             return parse_server_time(self._proto.updateTime)
         return None
 
     @property
-    def severity(self):
+    def severity(self) -> str:
         if self._proto.HasField("severity"):
             return alarms_pb2.AlarmSeverity.Name(self._proto.severity)
         return None
 
     @property
-    def sequence_number(self):
+    def sequence_number(self) -> int:
         """
         Sequence number for this specific alarm instance. This allows ensuring
         that operations (such as acknowledgment) are done on the expected alarm
         instance.
         """
         if self._proto.HasField("seqNum"):
             return self._proto.seqNum
         return None
 
     @property
-    def is_ok(self):
+    def is_ok(self) -> bool:
         """
         True if this alarm is currently 'inactive'.
 
         For a non-latching alarm this is identical to :meth:`is_process_ok`. A
         latching alarm is only OK if it has returned to normal and was
         acknowledged.
         """
         return not self._proto.triggered
 
     @property
-    def is_process_ok(self):
+    def is_process_ok(self) -> bool:
         """
         True if the process that caused this alarm is OK. For example:
         parameter back within limits.
 
         For a non-latching alarm this is identical to :meth:`is_ok`.
         """
         return self._proto.processOK
 
     @property
-    def is_latching(self):
+    def is_latching(self) -> bool:
         """
         True if this is a latching alarm. A latching alarm returns to
         normal only when the operator resets it
         """
         return self._proto.HasField("latching") and self._proto.latching
 
     @property
-    def is_latched(self):
+    def is_latched(self) -> bool:
         """
         True if this alarm is currently latched.
         """
         return self.is_latching and self.is_process_ok and not self.is_ok
 
     @property
-    def is_acknowledged(self):
+    def is_acknowledged(self) -> bool:
         """True if this alarm has been acknowledged."""
         return self._proto.acknowledged
 
     @property
-    def acknowledged_by(self):
+    def acknowledged_by(self) -> Optional[str]:
         """Username of the acknowledger."""
         if self.is_acknowledged and self._proto.acknowledgeInfo.HasField(
             "acknowledgedBy"
         ):
             return self._proto.acknowledgeInfo.acknowledgedBy
         return None
 
     @property
-    def acknowledge_message(self):
+    def acknowledge_message(self) -> Optional[str]:
         """Comment provided when acknowledging the alarm."""
         if self.is_acknowledged and self._proto.acknowledgeInfo.HasField(
             "acknowledgeMessage"
         ):
             return self._proto.acknowledgeInfo.acknowledgeMessage
         return None
 
     @property
-    def acknowledge_time(self):
+    def acknowledge_time(self) -> Optional[datetime]:
         """
         Processor time when the alarm was acknowledged.
-
-        :type: :class:`~datetime.datetime`
         """
         if self.is_acknowledged and self._proto.acknowledgeInfo.HasField(
             "acknowledgeTime"
         ):
             return parse_server_time(self._proto.acknowledgeInfo.acknowledgeTime)
         return None
 
     @property
-    def is_shelved(self):
+    def is_shelved(self) -> bool:
         """True if this alarm has been shelved."""
         return self._proto.HasField("shelveInfo")
 
     @property
-    def violation_count(self):
+    def violation_count(self) -> int:
         """
         Number of violating samples while this alarm is active.
         """
         if self._proto.HasField("violations"):
             return self._proto.violations
         return None
 
     @property
-    def count(self):
+    def count(self) -> int:
         """
         Total number of samples while this alarm is active.
         """
         if self._proto.HasField("count"):
             return self._proto.count
         return None
 
@@ -651,136 +682,118 @@
 
 class ParameterAlarm(Alarm):
     """
     An alarm triggered by a parameter that went out of limits.
     """
 
     @property
-    def trigger_value(self):
+    def trigger_value(self) -> "ParameterValue":
         """
         Parameter value that originally triggered the alarm
-
-        :type: :class:`.ParameterValue`
         """
         if self._proto.parameterDetail.HasField("triggerValue"):
             return ParameterValue(self._proto.parameterDetail.triggerValue)
         return None
 
     @property
-    def most_severe_value(self):
+    def most_severe_value(self) -> "ParameterValue":
         """
         First parameter value that invoked the highest severity
         level of this alarm.
-
-        :type: :class:`.ParameterValue`
         """
         if self._proto.parameterDetail.HasField("mostSevereValue"):
             return ParameterValue(self._proto.parameterDetail.mostSevereValue)
         return None
 
     @property
-    def current_value(self):
+    def current_value(self) -> "ParameterValue":
         """
         Latest parameter value for this alarm.
-
-        :type: :class:`.ParameterValue`
         """
         if self._proto.parameterDetail.HasField("currentValue"):
             return ParameterValue(self._proto.parameterDetail.currentValue)
         return None
 
 
 class EventAlarm(Alarm):
     """
     An alarm triggered by an event.
     """
 
     @property
-    def trigger_event(self):
+    def trigger_event(self) -> Event:
         """
         Event that originally triggered the alarm
-
-        :type: :class:`.Event`
         """
         if self._proto.eventDetail.HasField("triggerEvent"):
             return Event(self._proto.eventDetail.triggerEvent)
         return None
 
     @property
-    def most_severe_event(self):
+    def most_severe_event(self) -> Event:
         """
         First event that invoked the highest severity level
         of this alarm
-
-        :type: :class:`.Event`
         """
         if self._proto.eventDetail.HasField("mostSevereEvent"):
             return Event(self._proto.eventDetail.mostSevereEvent)
         return None
 
     @property
-    def current_event(self):
+    def current_event(self) -> Event:
         """
         Latest event for this alarm
-
-        :type: :class:`.Event`
         """
         if self._proto.eventDetail.HasField("currentEvent"):
             return Event(self._proto.eventDetail.currentEvent)
         return None
 
 
 class ParameterValue:
     def __init__(self, proto, id=None):
         self._proto = proto
         self._id = id or proto.id
 
     @property
-    def name(self):
+    def name(self) -> str:
         """
         An identifying name for the parameter value. Typically this is the
         fully-qualified XTCE name, but it may also be an alias depending
         on how the parameter update was requested.
         """
         if self._id.namespace:
             return self._id.namespace + "/" + self._id.name
         return self._id.name
 
     @property
-    def generation_time(self):
+    def generation_time(self) -> datetime:
         """
         The time when the parameter was generated. If the parameter
         was extracted from a packet, this usually returns the packet time.
-
-        :type: :class:`~datetime.datetime`
         """
         if self._proto.HasField("generationTime"):
             return parse_server_time(self._proto.generationTime)
         return None
 
     @property
-    def reception_time(self):
+    def reception_time(self) -> Optional[datetime]:
         """
         The time when the parameter value was received by Yamcs.
-
-        :type: :class:`~datetime.datetime`
         """
         if self._proto.HasField("acquisitionTime"):
             return parse_server_time(self._proto.acquisitionTime)
         return None
 
     @property
-    def validity_duration(self):
+    def validity_duration(self) -> Optional[timedelta]:
         """
         How long this parameter value is valid.
 
         .. note: There is also an option when subscribing to get updated when
                  the parameter values expire.
-
-        :type: :class:`~datetime.timedelta`
         """
         if self._proto.HasField("expireMillis"):
             return timedelta(milliseconds=self._proto.expireMillis)
         return None
 
     @property
     def raw_value(self):
@@ -797,36 +810,36 @@
         The engineering (calibrated) value.
         """
         if self._proto.HasField("engValue"):
             return parse_value(self._proto.engValue)
         return None
 
     @property
-    def monitoring_result(self):
+    def monitoring_result(self) -> str:
         if self._proto.HasField("monitoringResult"):
             return pvalue_pb2.MonitoringResult.Name(self._proto.monitoringResult)
         return None
 
     @property
-    def range_condition(self):
+    def range_condition(self) -> Optional[str]:
         """
         If the value is out of limits, this indicates ``LOW`` or ``HIGH``.
         """
         if self._proto.HasField("rangeCondition"):
             return pvalue_pb2.RangeCondition.Name(self._proto.rangeCondition)
         return None
 
     @property
-    def validity_status(self):
+    def validity_status(self) -> str:
         if self._proto.HasField("acquisitionStatus"):
             return pvalue_pb2.AcquisitionStatus.Name(self._proto.acquisitionStatus)
         return None
 
     @property
-    def processing_status(self):
+    def processing_status(self) -> bool:
         return self._proto.processingStatus
 
     def __str__(self):
         line = f"{self.generation_time} {self.name} {self.raw_value} {self.eng_value}"
         if self.monitoring_result:
             line += " [" + self.monitoring_result + "]"
         return line
@@ -848,30 +861,27 @@
                 pval = ParameterValue(pval_pb, id=id)
                 self._pvals[pval.name] = pval
 
     def __iter__(self):
         for pval in self._pvals.values():
             yield pval
 
-    def get_value(self, parameter):
+    def get_value(self, parameter: str) -> ParameterValue:
         """
         Returns the value of a specific parameter.
         Or ``None`` if the parameter is not included in
         this update.
 
-        :param string parameter: Parameter name.
-        :rtype: .ParameterValue
+        :param parameter:
+            Parameter name.
         """
         return self._pvals.get(parameter)
 
     @property
-    def parameters(self):
-        """
-        :type: List[:class:`.ParameterValue`]
-        """
+    def parameters(self) -> List[ParameterValue]:
         return list(self._pvals.values())
 
     def __str__(self):
         return self.parameters.__str__()
 
 
 class Calibrator:
@@ -890,58 +900,57 @@
 
         The `data` argument must be an array of ``[x, y]`` points.
     """
 
     POLYNOMIAL = "polynomial"
     SPLINE = "spline"
 
-    def __init__(self, context, type, data):
+    def __init__(self, context: str, type: str, data):
         """
-        :param str context: Condition under which this calibrator may be
-                            applied. The value ``None`` indicates the
-                            default calibrator which is only applied if
-                            no contextual calibrators match.
-        :param str type: One of ``polynomial`` or ``spline``.
-        :param data: Calibration definition for the selected type.
+        :param context:
+            Condition under which this calibrator may be
+            applied. The value ``None`` indicates the
+            default calibrator which is only applied if
+            no contextual calibrators match.
+        :param type:
+            One of ``polynomial`` or ``spline``.
+        :param data:
+            Calibration definition for the selected type.
         """
         self.context = context
         self.type = type
         self.data = data
 
 
 class ContainerData:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """
         The name of the container.
         """
         if self._proto.HasField("name"):
             return self._proto.name
         return None
 
     @property
-    def generation_time(self):
+    def generation_time(self) -> datetime:
         """
         The time when this container's packet was generated (packet time).
-
-        :type: :class:`~datetime.datetime`
         """
         if self._proto.HasField("generationTime"):
             return parse_server_time(self._proto.generationTime)
         return None
 
     @property
-    def reception_time(self):
+    def reception_time(self) -> datetime:
         """
         The time when this container's packet was received by Yamcs.
-
-        :type: :class:`~datetime.datetime`
         """
         if self._proto.HasField("receptionTime"):
             return parse_server_time(self._proto.receptionTime)
         return None
 
     @property
     def binary(self):
@@ -957,48 +966,44 @@
 
 
 class Packet:
     def __init__(self, proto):
         self._proto = proto
 
     @property
-    def name(self):
+    def name(self) -> str:
         """
         The name of the packet. When using XTCE extraction this is the
         fully-qualified name of the first container in the hierarchy that
         this packet maps to.
         """
         if self._proto.HasField("id"):
             return self._proto.id.name
         return None
 
     @property
-    def generation_time(self):
+    def generation_time(self) -> datetime:
         """
         The time when the packet was generated (packet time).
-
-        :type: :class:`~datetime.datetime`
         """
         if self._proto.HasField("generationTime"):
             return parse_server_time(self._proto.generationTime)
         return None
 
     @property
-    def reception_time(self):
+    def reception_time(self) -> datetime:
         """
         The time when the packet was received by Yamcs.
-
-        :type: :class:`~datetime.datetime`
         """
         if self._proto.HasField("receptionTime"):
             return parse_server_time(self._proto.receptionTime)
         return None
 
     @property
-    def sequence_number(self):
+    def sequence_number(self) -> int:
         """
         The sequence number of the packet. This is usually decoded from
         the packet.
         """
         if self._proto.HasField("sequenceNumber"):
             return self._proto.sequenceNumber
         return None
@@ -1019,39 +1024,46 @@
 class RangeSet:
     """
     A set of alarm range that apply in a specific context.
     """
 
     def __init__(
         self,
-        context,
-        watch=None,
-        warning=None,
-        distress=None,
-        critical=None,
-        severe=None,
-        min_violations=1,
+        context: str,
+        watch: Optional[Tuple[float, float]] = None,
+        warning: Optional[Tuple[float, float]] = None,
+        distress: Optional[Tuple[float, float]] = None,
+        critical: Optional[Tuple[float, float]] = None,
+        severe: Optional[Tuple[float, float]] = None,
+        min_violations: int = 1,
     ):
         """
-        :param str context: Condition under which this range set is
-                            applicable. The value ``None`` indicates the
-                            default range set which is only applicable if
-                            no contextual sets match.
-        :param (float,float) watch: Range expressed as a tuple ``(lo, hi)``
-                                where lo and hi are assumed exclusive.
-        :param (float,float) warning: Range expressed as a tuple ``(lo, hi)``
-                                  where lo and hi are assumed exclusive.
-        :param (float,float) distress: Range expressed as a tuple ``(lo, hi)``
-                                   where lo and hi are assumed exclusive.
-        :param (float,float) critical: Range expressed as a tuple ``(lo, hi)``
-                                   where lo and hi are assumed exclusive.
-        :param (float,float) severe: Range expressed as a tuple ``(lo, hi)``
-                                 where lo and hi are assumed exclusive.
-        :param int min_violations: Minimum violations before an alarm is
-                                   generated.
+        :param context:
+            Condition under which this range set is
+            applicable. The value ``None`` indicates the
+            default range set which is only applicable if
+            no contextual sets match.
+        :param watch:
+            Range expressed as a tuple ``(lo, hi)``
+            where lo and hi are assumed exclusive.
+        :param warning:
+            Range expressed as a tuple ``(lo, hi)``
+            where lo and hi are assumed exclusive.
+        :param distress:
+            Range expressed as a tuple ``(lo, hi)``
+            where lo and hi are assumed exclusive.
+        :param critical:
+            Range expressed as a tuple ``(lo, hi)``
+            where lo and hi are assumed exclusive.
+        :param severe:
+            Range expressed as a tuple ``(lo, hi)``
+            where lo and hi are assumed exclusive.
+        :param min_violations:
+            Minimum violations before an alarm is
+            generated.
         """
         self.context = context
         self.watch = watch
         self.warning = warning
         self.distress = distress
         self.critical = critical
         self.severe = severe
@@ -1060,16 +1072,17 @@
 
 class ValueUpdate:
     """
     Data holder for passing a value along with its generation time when
     updating a software parameter.
     """
 
-    def __init__(self, value, generation_time=None):
+    def __init__(self, value: Any, generation_time: Optional[datetime] = None):
         """
-        :param value: The value to set
-        :param generation_time: Generation time of the value. If unset, Yamcs will
-                                assign the generation time.
-        :type generation_time: Optional[~datetime.datetime]
+        :param value:
+            The value to set
+        :param generation_time:
+            Generation time of the value. If unset, Yamcs will
+            assign the generation time.
         """
         self.value = value
         self.generation_time = generation_time
```

### Comparing `yamcs-client-1.8.8/src/yamcs_client.egg-info/PKG-INFO` & `yamcs-client-1.9.0/src/yamcs_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-client
-Version: 1.8.8
+Version: 1.9.0
 Summary: Yamcs API client library
 Home-page: https://github.com/yamcs/python-yamcs-client
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `yamcs-client-1.8.8/src/yamcs_client.egg-info/SOURCES.txt` & `yamcs-client-1.9.0/src/yamcs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

