# Comparing `tmp/fintekkers-ledger-models-0.1.46.tar.gz` & `tmp/fintekkers-ledger-models-0.1.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fintekkers-ledger-models-0.1.46.tar", last modified: Thu Apr 27 21:40:07 2023, max compression
+gzip compressed data, was "fintekkers-ledger-models-0.1.47.tar", last modified: Sun Apr 30 22:17:07 2023, max compression
```

## Comparing `fintekkers-ledger-models-0.1.46.tar` & `fintekkers-ledger-models-0.1.47.tar`

### file list

```diff
@@ -1,258 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.626417 fintekkers-ledger-models-0.1.46/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-27 21:40:07.626417 fintekkers-ledger-models-0.1.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.598417 fintekkers-ledger-models-0.1.46/fintekkers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.598417 fintekkers-ledger-models-0.1.46/fintekkers/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.598417 fintekkers-ledger-models-0.1.46/fintekkers/models/portfolio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/portfolio/portfolio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/portfolio/portfolio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/portfolio/portfolio_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.598417 fintekkers-ledger-models-0.1.46/fintekkers/models/position/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/field_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/field_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/field_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/measure_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/measure_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/measure_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_filter_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_filter_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_filter_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_util_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_util_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_util_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.602417 fintekkers-ledger-models-0.1.46/fintekkers/models/price/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/price/price_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/price/price_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/price/price_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.602417 fintekkers-ledger-models-0.1.46/fintekkers/models/security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/coupon_frequency_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/coupon_frequency_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/coupon_frequency_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/coupon_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/coupon_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/coupon_type_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.606417 fintekkers-ledger-models-0.1.46/fintekkers/models/security/identifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/identifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/identifier/identifier_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/identifier/identifier_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/identifier/identifier_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/identifier/identifier_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/identifier/identifier_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/identifier/identifier_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/security_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/security_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/security_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/security_quantity_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/security_quantity_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/security_quantity_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/security_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/security_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/security_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/tenor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/tenor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/tenor_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/tenor_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/tenor_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/security/tenor_type_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.606417 fintekkers-ledger-models-0.1.46/fintekkers/models/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/strategy/strategy_allocation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/strategy/strategy_allocation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/strategy/strategy_allocation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/strategy/strategy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/strategy/strategy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/strategy/strategy_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.606417 fintekkers-ledger-models-0.1.46/fintekkers/models/transaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/transaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/transaction/transaction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/transaction/transaction_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/transaction/transaction_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/transaction/transaction_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/transaction/transaction_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/transaction/transaction_type_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.610417 fintekkers-ledger-models-0.1.46/fintekkers/models/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/decimal_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/decimal_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/decimal_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/endpoint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/endpoint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/endpoint_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/local_date_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/local_date_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/local_date_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/local_timestamp_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/local_timestamp_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/local_timestamp_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.610417 fintekkers-ledger-models-0.1.46/fintekkers/models/util/lock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/lock/node_partition_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/lock/node_partition_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/lock/node_partition_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/lock/node_state_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/lock/node_state_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/lock/node_state_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/uuid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/uuid_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/models/util/uuid_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.610417 fintekkers-ledger-models-0.1.46/fintekkers/requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.614417 fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/create_portfolio_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/create_portfolio_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/create_portfolio_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/create_portfolio_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/create_portfolio_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/create_portfolio_response_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/query_portfolio_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/query_portfolio_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/query_portfolio_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/query_portfolio_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/query_portfolio_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/query_portfolio_response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.614417 fintekkers-ledger-models-0.1.46/fintekkers/requests/position/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/position/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/position/query_position_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/position/query_position_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/position/query_position_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/position/query_position_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/position/query_position_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/position/query_position_response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.614417 fintekkers-ledger-models-0.1.46/fintekkers/requests/security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/security/create_security_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/security/create_security_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/security/create_security_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/security/create_security_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/security/create_security_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/security/create_security_response_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/security/query_security_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/security/query_security_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/security/query_security_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/security/query_security_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/security/query_security_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/security/query_security_response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.618417 fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/create_transaction_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/create_transaction_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/create_transaction_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/create_transaction_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/create_transaction_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/create_transaction_response_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/query_transaction_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/query_transaction_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/query_transaction_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/query_transaction_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/query_transaction_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/query_transaction_response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.618417 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.618417 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/error_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/error_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/error_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/message_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/message_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/summary_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/summary_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/summary_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.618417 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/lock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/lock/lock_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/lock/lock_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/lock/lock_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/lock/lock_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/lock/lock_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/lock/lock_response_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/operation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/operation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/util/operation_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.618417 fintekkers-ledger-models-0.1.46/fintekkers/requests/valuation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/valuation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/valuation/valuation_request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/valuation/valuation_request_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/valuation/valuation_request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/valuation/valuation_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/valuation/valuation_response_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/requests/valuation/valuation_response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.618417 fintekkers-ledger-models-0.1.46/fintekkers/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.618417 fintekkers-ledger-models-0.1.46/fintekkers/services/lock_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/lock_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/lock_service/lock_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/lock_service/lock_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/lock_service/lock_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.622417 fintekkers-ledger-models-0.1.46/fintekkers/services/portfolio_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/portfolio_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/portfolio_service/portfolio_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/portfolio_service/portfolio_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/portfolio_service/portfolio_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.622417 fintekkers-ledger-models-0.1.46/fintekkers/services/position_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/position_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/position_service/position_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/position_service/position_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/position_service/position_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.622417 fintekkers-ledger-models-0.1.46/fintekkers/services/security_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/security_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/security_service/security_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/security_service/security_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/security_service/security_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.622417 fintekkers-ledger-models-0.1.46/fintekkers/services/transaction_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/transaction_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/transaction_service/transaction_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/transaction_service/transaction_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/transaction_service/transaction_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.622417 fintekkers-ledger-models-0.1.46/fintekkers/services/valuation_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/valuation_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/valuation_service/valuation_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/valuation_service/valuation_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/services/valuation_service/valuation_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.622417 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.622417 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/security_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/tenor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.626417 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/util/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/util/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/util/fintekkers_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/util/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.626417 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/requests/security.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/requests/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.626417 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/fintekkers/wrappers/services/security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 21:40:07.626417 fintekkers-ledger-models-0.1.46/fintekkers_ledger_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-27 21:40:07.000000 fintekkers-ledger-models-0.1.46/fintekkers_ledger_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-04-27 21:40:07.000000 fintekkers-ledger-models-0.1.46/fintekkers_ledger_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 21:40:07.000000 fintekkers-ledger-models-0.1.46/fintekkers_ledger_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 21:40:07.000000 fintekkers-ledger-models-0.1.46/fintekkers_ledger_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-27 21:40:07.626417 fintekkers-ledger-models-0.1.46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-27 21:40:06.000000 fintekkers-ledger-models-0.1.46/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.618435 fintekkers-ledger-models-0.1.47/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-30 22:17:07.618435 fintekkers-ledger-models-0.1.47/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.586435 fintekkers-ledger-models-0.1.47/fintekkers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.586435 fintekkers-ledger-models-0.1.47/fintekkers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.586435 fintekkers-ledger-models-0.1.47/fintekkers/models/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/portfolio/portfolio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/portfolio/portfolio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/portfolio/portfolio_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.590435 fintekkers-ledger-models-0.1.47/fintekkers/models/position/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/field_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/field_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/field_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/measure_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/measure_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/measure_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_filter_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_filter_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_filter_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_util_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_util_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_util_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.594435 fintekkers-ledger-models-0.1.47/fintekkers/models/price/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/price/price_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/price/price_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/price/price_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.598435 fintekkers-ledger-models-0.1.47/fintekkers/models/security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/coupon_frequency_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/coupon_frequency_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/coupon_frequency_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/coupon_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/coupon_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/coupon_type_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.598435 fintekkers-ledger-models-0.1.47/fintekkers/models/security/identifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/identifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/identifier/identifier_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/identifier/identifier_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/identifier/identifier_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/identifier/identifier_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/identifier/identifier_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/identifier/identifier_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/security_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/security_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/security_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/security_quantity_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/security_quantity_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/security_quantity_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/security_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/security_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/security_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/tenor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/tenor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/tenor_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/tenor_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/tenor_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/security/tenor_type_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.602435 fintekkers-ledger-models-0.1.47/fintekkers/models/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/strategy/strategy_allocation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/strategy/strategy_allocation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/strategy/strategy_allocation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/strategy/strategy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/strategy/strategy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/strategy/strategy_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.602435 fintekkers-ledger-models-0.1.47/fintekkers/models/transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/transaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/transaction/transaction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/transaction/transaction_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/transaction/transaction_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/transaction/transaction_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/transaction/transaction_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/transaction/transaction_type_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.606435 fintekkers-ledger-models-0.1.47/fintekkers/models/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/decimal_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/decimal_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/decimal_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/endpoint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/endpoint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/endpoint_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/local_date_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/local_date_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/local_date_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/local_timestamp_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/local_timestamp_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/local_timestamp_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.610435 fintekkers-ledger-models-0.1.47/fintekkers/models/util/lock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/lock/node_partition_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/lock/node_partition_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/lock/node_partition_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/lock/node_state_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/lock/node_state_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/lock/node_state_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/uuid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/uuid_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/models/util/uuid_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.610435 fintekkers-ledger-models-0.1.47/fintekkers/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.610435 fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/create_portfolio_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/create_portfolio_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/create_portfolio_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/create_portfolio_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/create_portfolio_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/create_portfolio_response_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/query_portfolio_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/query_portfolio_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/query_portfolio_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/query_portfolio_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/query_portfolio_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/query_portfolio_response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.610435 fintekkers-ledger-models-0.1.47/fintekkers/requests/position/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/position/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/position/query_position_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/position/query_position_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/position/query_position_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/position/query_position_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/position/query_position_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/position/query_position_response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.610435 fintekkers-ledger-models-0.1.47/fintekkers/requests/security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/security/create_security_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/security/create_security_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/security/create_security_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/security/create_security_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/security/create_security_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/security/create_security_response_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/security/query_security_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/security/query_security_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/security/query_security_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/security/query_security_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/security/query_security_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/security/query_security_response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.614435 fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/create_transaction_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/create_transaction_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/create_transaction_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/create_transaction_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/create_transaction_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/create_transaction_response_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/query_transaction_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/query_transaction_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/query_transaction_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/query_transaction_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/query_transaction_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/query_transaction_response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.614435 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.614435 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/error_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/error_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/error_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/message_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/message_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/summary_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/summary_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/summary_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.614435 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/lock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/lock/lock_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/lock/lock_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/lock/lock_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/lock/lock_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/lock/lock_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/lock/lock_response_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/operation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/operation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/util/operation_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.614435 fintekkers-ledger-models-0.1.47/fintekkers/requests/valuation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/valuation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/valuation/valuation_request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/valuation/valuation_request_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/valuation/valuation_request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/valuation/valuation_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/valuation/valuation_response_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/requests/valuation/valuation_response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.614435 fintekkers-ledger-models-0.1.47/fintekkers/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.614435 fintekkers-ledger-models-0.1.47/fintekkers/services/lock_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/lock_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/lock_service/lock_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/lock_service/lock_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/lock_service/lock_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.614435 fintekkers-ledger-models-0.1.47/fintekkers/services/portfolio_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/portfolio_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/portfolio_service/portfolio_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/portfolio_service/portfolio_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/portfolio_service/portfolio_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.618435 fintekkers-ledger-models-0.1.47/fintekkers/services/position_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/position_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/position_service/position_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/position_service/position_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/position_service/position_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.618435 fintekkers-ledger-models-0.1.47/fintekkers/services/security_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/security_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/security_service/security_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/security_service/security_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/security_service/security_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.618435 fintekkers-ledger-models-0.1.47/fintekkers/services/transaction_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/transaction_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/transaction_service/transaction_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/transaction_service/transaction_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/transaction_service/transaction_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.618435 fintekkers-ledger-models-0.1.47/fintekkers/services/valuation_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/valuation_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/valuation_service/valuation_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/valuation_service/valuation_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/services/valuation_service/valuation_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.618435 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.618435 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/security_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/tenor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.618435 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/util/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/util/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/util/fintekkers_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/util/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.618435 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/requests/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/requests/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.618435 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers/wrappers/services/security.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:17:07.618435 fintekkers-ledger-models-0.1.47/fintekkers_ledger_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers_ledger_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers_ledger_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers_ledger_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/fintekkers_ledger_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-30 22:17:07.618435 fintekkers-ledger-models-0.1.47/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-30 22:17:07.000000 fintekkers-ledger-models-0.1.47/setup.py
```

### Comparing `fintekkers-ledger-models-0.1.46/PKG-INFO` & `fintekkers-ledger-models-0.1.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fintekkers-ledger-models
-Version: 0.1.46
+Version: 0.1.47
 Summary: Fintekkers Ledger Models python package
 Home-page: https://github.com/fintekkers/ledger-models
 Author: David Doherty
 Author-email: dave@fintekkers.org
 License: MIT
 Keywords: fintekkers ledger models
 Platform: UNKNOWN
```

### Comparing `fintekkers-ledger-models-0.1.46/README.rst` & `fintekkers-ledger-models-0.1.47/README.rst`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/portfolio/portfolio_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/portfolio/portfolio_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/portfolio/portfolio_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/portfolio/portfolio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/position/field_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/position/field_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/position/field_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/position/field_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/position/measure_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/position/measure_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/position/measure_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/position/measure_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_filter_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_filter_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/query_portfolio_request_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: fintekkers/models/position/position.proto
+# source: fintekkers/requests/portfolio/query_portfolio_request.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from fintekkers.models.util import decimal_value_pb2 as fintekkers_dot_models_dot_util_dot_decimal__value__pb2
-from fintekkers.models.position import measure_pb2 as fintekkers_dot_models_dot_position_dot_measure__pb2
-from fintekkers.models.position import position_util_pb2 as fintekkers_dot_models_dot_position_dot_position__util__pb2
+from fintekkers.models.util import uuid_pb2 as fintekkers_dot_models_dot_util_dot_uuid__pb2
+from fintekkers.models.util import local_timestamp_pb2 as fintekkers_dot_models_dot_util_dot_local__timestamp__pb2
+from fintekkers.models.position import position_filter_pb2 as fintekkers_dot_models_dot_position_dot_position__filter__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)fintekkers/models/position/position.proto\x12\x1a\x66intekkers.models.position\x1a*fintekkers/models/util/decimal_value.proto\x1a(fintekkers/models/position/measure.proto\x1a.fintekkers/models/position/position_util.proto\"\x9b\x01\n\x14MeasureMapFieldEntry\x12\x39\n\x07measure\x18\x01 \x01(\x0e\x32(.fintekkers.models.position.MeasureProto\x12H\n\x15measure_decimal_value\x18\x02 \x01(\x0b\x32).fintekkers.models.util.DecimalValueProto\"\xc1\x02\n\rPositionProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x44\n\rposition_view\x18\n \x01(\x0e\x32-.fintekkers.models.position.PositionViewProto\x12\x44\n\rposition_type\x18\x0b \x01(\x0e\x32-.fintekkers.models.position.PositionTypeProto\x12\x42\n\x08measures\x18\x14 \x03(\x0b\x32\x30.fintekkers.models.position.MeasureMapFieldEntry\x12\x39\n\x06\x66ields\x18\x15 \x03(\x0b\x32).fintekkers.models.position.FieldMapEntry*S\n\x11PositionViewProto\x12\x19\n\x15UNKNOWN_POSITION_VIEW\x10\x00\x12\x10\n\x0c\x44\x45\x46\x41ULT_VIEW\x10\x01\x12\x11\n\rSTRATEGY_VIEW\x10\x02*L\n\x11PositionTypeProto\x12\x19\n\x15UNKNOWN_POSITION_TYPE\x10\x00\x12\x0f\n\x0bTRANSACTION\x10\x01\x12\x0b\n\x07TAX_LOT\x10\x02\x42\x12\x42\x0ePositionProtosP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n;fintekkers/requests/portfolio/query_portfolio_request.proto\x12\x1d\x66intekkers.requests.portfolio\x1a!fintekkers/models/util/uuid.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a\x30\x66intekkers/models/position/position_filter.proto\"\x82\x02\n\x1aQueryPortfolioRequestProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x30\n\x05uuids\x18\x15 \x03(\x0b\x32!.fintekkers.models.util.UUIDProto\x12O\n\x16search_portfolio_input\x18\x16 \x01(\x0b\x32/.fintekkers.models.position.PositionFilterProto\x12:\n\x05\x61s_of\x18\x17 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProtoB\x1f\x42\x1bQueryPortfolioRequestProtosP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.models.position.position_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.requests.portfolio.query_portfolio_request_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'B\016PositionProtosP\001'
-  _POSITIONVIEWPROTO._serialized_start=689
-  _POSITIONVIEWPROTO._serialized_end=772
-  _POSITIONTYPEPROTO._serialized_start=774
-  _POSITIONTYPEPROTO._serialized_end=850
-  _MEASUREMAPFIELDENTRY._serialized_start=208
-  _MEASUREMAPFIELDENTRY._serialized_end=363
-  _POSITIONPROTO._serialized_start=366
-  _POSITIONPROTO._serialized_end=687
+  DESCRIPTOR._serialized_options = b'B\033QueryPortfolioRequestProtosP\001'
+  _QUERYPORTFOLIOREQUESTPROTO._serialized_start=226
+  _QUERYPORTFOLIOREQUESTPROTO._serialized_end=484
 # @@protoc_insertion_point(module_scope)
```

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from fintekkers.models.util import decimal_value_pb2 as _decimal_value_pb2
-from fintekkers.models.position import measure_pb2 as _measure_pb2
 from fintekkers.models.position import position_util_pb2 as _position_util_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
@@ -11,36 +9,28 @@
 DESCRIPTOR: _descriptor.FileDescriptor
 STRATEGY_VIEW: PositionViewProto
 TAX_LOT: PositionTypeProto
 TRANSACTION: PositionTypeProto
 UNKNOWN_POSITION_TYPE: PositionTypeProto
 UNKNOWN_POSITION_VIEW: PositionViewProto
 
-class MeasureMapFieldEntry(_message.Message):
-    __slots__ = ["measure", "measure_decimal_value"]
-    MEASURE_DECIMAL_VALUE_FIELD_NUMBER: _ClassVar[int]
-    MEASURE_FIELD_NUMBER: _ClassVar[int]
-    measure: _measure_pb2.MeasureProto
-    measure_decimal_value: _decimal_value_pb2.DecimalValueProto
-    def __init__(self, measure: _Optional[_Union[_measure_pb2.MeasureProto, str]] = ..., measure_decimal_value: _Optional[_Union[_decimal_value_pb2.DecimalValueProto, _Mapping]] = ...) -> None: ...
-
 class PositionProto(_message.Message):
     __slots__ = ["fields", "measures", "object_class", "position_type", "position_view", "version"]
     FIELDS_FIELD_NUMBER: _ClassVar[int]
     MEASURES_FIELD_NUMBER: _ClassVar[int]
     OBJECT_CLASS_FIELD_NUMBER: _ClassVar[int]
     POSITION_TYPE_FIELD_NUMBER: _ClassVar[int]
     POSITION_VIEW_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     fields: _containers.RepeatedCompositeFieldContainer[_position_util_pb2.FieldMapEntry]
-    measures: _containers.RepeatedCompositeFieldContainer[MeasureMapFieldEntry]
+    measures: _containers.RepeatedCompositeFieldContainer[_position_util_pb2.MeasureMapEntry]
     object_class: str
     position_type: PositionTypeProto
     position_view: PositionViewProto
     version: str
-    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., position_view: _Optional[_Union[PositionViewProto, str]] = ..., position_type: _Optional[_Union[PositionTypeProto, str]] = ..., measures: _Optional[_Iterable[_Union[MeasureMapFieldEntry, _Mapping]]] = ..., fields: _Optional[_Iterable[_Union[_position_util_pb2.FieldMapEntry, _Mapping]]] = ...) -> None: ...
+    def __init__(self, object_class: _Optional[str] = ..., version: _Optional[str] = ..., position_view: _Optional[_Union[PositionViewProto, str]] = ..., position_type: _Optional[_Union[PositionTypeProto, str]] = ..., measures: _Optional[_Iterable[_Union[_position_util_pb2.MeasureMapEntry, _Mapping]]] = ..., fields: _Optional[_Iterable[_Union[_position_util_pb2.FieldMapEntry, _Mapping]]] = ...) -> None: ...
 
 class PositionViewProto(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
 class PositionTypeProto(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
```

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_status_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_status_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_util_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_util_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from fintekkers.models.position import field_pb2 as fintekkers_dot_models_dot_position_dot_field__pb2
 from fintekkers.models.position import measure_pb2 as fintekkers_dot_models_dot_position_dot_measure__pb2
 from fintekkers.models.util import decimal_value_pb2 as fintekkers_dot_models_dot_util_dot_decimal__value__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.fintekkers/models/position/position_util.proto\x12\x1a\x66intekkers.models.position\x1a\x19google/protobuf/any.proto\x1a&fintekkers/models/position/field.proto\x1a(fintekkers/models/position/measure.proto\x1a*fintekkers/models/util/decimal_value.proto\"\x8c\x01\n\x0fMeasureMapEntry\x12\x37\n\x05\x66ield\x18\x01 \x01(\x0e\x32(.fintekkers.models.position.MeasureProto\x12@\n\rmeasure_value\x18\x02 \x01(\x0b\x32).fintekkers.models.util.DecimalValueProto\"\xec\x01\n\rFieldMapEntry\x12\x35\n\x05\x66ield\x18\x01 \x01(\x0e\x32&.fintekkers.models.position.FieldProto\x12\x32\n\x12\x66ield_value_packed\x18\x04 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x12\x14\n\nenum_value\x18\x05 \x01(\x05H\x00\x12\x44\n\x08operator\x18\x14 \x01(\x0e\x32\x32.fintekkers.models.position.PositionFilterOperatorB\x14\n\x12\x46ieldMapValueOneOf*\x9a\x01\n\x16PositionFilterOperator\x12\x14\n\x10UNKNOWN_OPERATOR\x10\x00\x12\n\n\x06\x45QUALS\x10\x01\x12\x0e\n\nNOT_EQUALS\x10\x02\x12\r\n\tLESS_THAN\x10\x03\x12\x17\n\x13LESS_THAN_OR_EQUALS\x10\x04\x12\r\n\tMORE_THAN\x10\x05\x12\x17\n\x13MORE_THAN_OR_EQUALS\x10\x06\x42\x16\x42\x12PositionUtilProtosP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.fintekkers/models/position/position_util.proto\x12\x1a\x66intekkers.models.position\x1a\x19google/protobuf/any.proto\x1a&fintekkers/models/position/field.proto\x1a(fintekkers/models/position/measure.proto\x1a*fintekkers/models/util/decimal_value.proto\"\x96\x01\n\x0fMeasureMapEntry\x12\x39\n\x07measure\x18\x01 \x01(\x0e\x32(.fintekkers.models.position.MeasureProto\x12H\n\x15measure_decimal_value\x18\x02 \x01(\x0b\x32).fintekkers.models.util.DecimalValueProto\"\xec\x01\n\rFieldMapEntry\x12\x35\n\x05\x66ield\x18\x01 \x01(\x0e\x32&.fintekkers.models.position.FieldProto\x12\x32\n\x12\x66ield_value_packed\x18\x04 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x12\x14\n\nenum_value\x18\x05 \x01(\x05H\x00\x12\x44\n\x08operator\x18\x14 \x01(\x0e\x32\x32.fintekkers.models.position.PositionFilterOperatorB\x14\n\x12\x46ieldMapValueOneOf*\x9a\x01\n\x16PositionFilterOperator\x12\x14\n\x10UNKNOWN_OPERATOR\x10\x00\x12\n\n\x06\x45QUALS\x10\x01\x12\x0e\n\nNOT_EQUALS\x10\x02\x12\r\n\tLESS_THAN\x10\x03\x12\x17\n\x13LESS_THAN_OR_EQUALS\x10\x04\x12\r\n\tMORE_THAN\x10\x05\x12\x17\n\x13MORE_THAN_OR_EQUALS\x10\x06\x42\x16\x42\x12PositionUtilProtosP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.models.position.position_util_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\022PositionUtilProtosP\001'
-  _POSITIONFILTEROPERATOR._serialized_start=614
-  _POSITIONFILTEROPERATOR._serialized_end=768
+  _POSITIONFILTEROPERATOR._serialized_start=624
+  _POSITIONFILTEROPERATOR._serialized_end=778
   _MEASUREMAPENTRY._serialized_start=232
-  _MEASUREMAPENTRY._serialized_end=372
-  _FIELDMAPENTRY._serialized_start=375
-  _FIELDMAPENTRY._serialized_end=611
+  _MEASUREMAPENTRY._serialized_end=382
+  _FIELDMAPENTRY._serialized_start=385
+  _FIELDMAPENTRY._serialized_end=621
 # @@protoc_insertion_point(module_scope)
```

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/position/position_util_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/position/position_util_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     enum_value: int
     field: _field_pb2.FieldProto
     field_value_packed: _any_pb2.Any
     operator: PositionFilterOperator
     def __init__(self, field: _Optional[_Union[_field_pb2.FieldProto, str]] = ..., field_value_packed: _Optional[_Union[_any_pb2.Any, _Mapping]] = ..., enum_value: _Optional[int] = ..., operator: _Optional[_Union[PositionFilterOperator, str]] = ...) -> None: ...
 
 class MeasureMapEntry(_message.Message):
-    __slots__ = ["field", "measure_value"]
-    FIELD_FIELD_NUMBER: _ClassVar[int]
-    MEASURE_VALUE_FIELD_NUMBER: _ClassVar[int]
-    field: _measure_pb2.MeasureProto
-    measure_value: _decimal_value_pb2.DecimalValueProto
-    def __init__(self, field: _Optional[_Union[_measure_pb2.MeasureProto, str]] = ..., measure_value: _Optional[_Union[_decimal_value_pb2.DecimalValueProto, _Mapping]] = ...) -> None: ...
+    __slots__ = ["measure", "measure_decimal_value"]
+    MEASURE_DECIMAL_VALUE_FIELD_NUMBER: _ClassVar[int]
+    MEASURE_FIELD_NUMBER: _ClassVar[int]
+    measure: _measure_pb2.MeasureProto
+    measure_decimal_value: _decimal_value_pb2.DecimalValueProto
+    def __init__(self, measure: _Optional[_Union[_measure_pb2.MeasureProto, str]] = ..., measure_decimal_value: _Optional[_Union[_decimal_value_pb2.DecimalValueProto, _Mapping]] = ...) -> None: ...
 
 class PositionFilterOperator(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
```

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/price/price_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/price/price_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/price/price_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/price/price_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/security/coupon_frequency_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/security/coupon_frequency_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/security/coupon_frequency_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/security/coupon_frequency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/security/coupon_type_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/security/coupon_type_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/security/identifier/identifier_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/security/identifier/identifier_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/security/identifier/identifier_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/security/identifier/identifier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/security/identifier/identifier_type_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/security/identifier/identifier_type_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/security/identifier/identifier_type_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/security/identifier/identifier_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/security/security_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/security/security_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/security/security_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/security/security_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/security/security_quantity_type_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/security/security_quantity_type_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/security/security_type_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/security/security_type_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/security/tenor_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/security/tenor_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/security/tenor_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/security/tenor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/security/tenor_type_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/security/tenor_type_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/strategy/strategy_allocation_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/strategy/strategy_allocation_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/strategy/strategy_allocation_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/strategy/strategy_allocation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/strategy/strategy_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/strategy/strategy_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/strategy/strategy_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/strategy/strategy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/transaction/transaction_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/transaction/transaction_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/transaction/transaction_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/transaction/transaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/transaction/transaction_type_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/transaction/transaction_type_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/transaction/transaction_type_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/transaction/transaction_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/util/decimal_value_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/util/decimal_value_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/util/endpoint_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/util/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/util/endpoint_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/util/endpoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/util/local_date_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/util/local_date_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/util/local_date_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/util/local_date_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/util/local_timestamp_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/util/local_timestamp_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/util/local_timestamp_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/util/local_timestamp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/util/lock/node_partition_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/util/lock/node_partition_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/util/lock/node_partition_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/util/lock/node_partition_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/util/lock/node_state_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/util/lock/node_state_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/util/lock/node_state_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/models/util/lock/node_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/models/util/uuid_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/models/util/uuid_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/create_portfolio_request_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/create_portfolio_request_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/create_portfolio_request_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/create_portfolio_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/create_portfolio_response_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/create_portfolio_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/create_portfolio_response_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/create_portfolio_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/query_portfolio_request_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/query_transaction_request_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: fintekkers/requests/portfolio/query_portfolio_request.proto
+# source: fintekkers/requests/transaction/query_transaction_request.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
@@ -12,18 +12,18 @@
 
 
 from fintekkers.models.util import uuid_pb2 as fintekkers_dot_models_dot_util_dot_uuid__pb2
 from fintekkers.models.util import local_timestamp_pb2 as fintekkers_dot_models_dot_util_dot_local__timestamp__pb2
 from fintekkers.models.position import position_filter_pb2 as fintekkers_dot_models_dot_position_dot_position__filter__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n;fintekkers/requests/portfolio/query_portfolio_request.proto\x12\x1d\x66intekkers.requests.portfolio\x1a!fintekkers/models/util/uuid.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a\x30\x66intekkers/models/position/position_filter.proto\"\x82\x02\n\x1aQueryPortfolioRequestProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x30\n\x05uuids\x18\x15 \x03(\x0b\x32!.fintekkers.models.util.UUIDProto\x12O\n\x16search_portfolio_input\x18\x16 \x01(\x0b\x32/.fintekkers.models.position.PositionFilterProto\x12:\n\x05\x61s_of\x18\x17 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProtoB\x1f\x42\x1bQueryPortfolioRequestProtosP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n?fintekkers/requests/transaction/query_transaction_request.proto\x12\x1f\x66intekkers.requests.transaction\x1a!fintekkers/models/util/uuid.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a\x30\x66intekkers/models/position/position_filter.proto\"\x86\x02\n\x1cQueryTransactionRequestProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x30\n\x05uuids\x18\x15 \x03(\x0b\x32!.fintekkers.models.util.UUIDProto\x12Q\n\x18search_transaction_input\x18\x16 \x01(\x0b\x32/.fintekkers.models.position.PositionFilterProto\x12:\n\x05\x61s_of\x18\x17 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProtoB!B\x1dQueryTransactionRequestProtosP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.requests.portfolio.query_portfolio_request_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.requests.transaction.query_transaction_request_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'B\033QueryPortfolioRequestProtosP\001'
-  _QUERYPORTFOLIOREQUESTPROTO._serialized_start=226
-  _QUERYPORTFOLIOREQUESTPROTO._serialized_end=484
+  DESCRIPTOR._serialized_options = b'B\035QueryTransactionRequestProtosP\001'
+  _QUERYTRANSACTIONREQUESTPROTO._serialized_start=232
+  _QUERYTRANSACTIONREQUESTPROTO._serialized_end=494
 # @@protoc_insertion_point(module_scope)
```

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/query_portfolio_request_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/query_portfolio_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/query_portfolio_response_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/query_portfolio_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/portfolio/query_portfolio_response_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/portfolio/query_portfolio_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/position/query_position_request_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/position/query_position_request_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/position/query_position_request_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/position/query_position_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/position/query_position_response_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/position/query_position_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/position/query_position_response_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/position/query_position_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/security/create_security_request_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/security/create_security_request_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/security/create_security_request_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/security/create_security_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/security/create_security_response_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/security/create_security_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/security/create_security_response_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/security/create_security_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/security/query_security_request_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/security/query_security_request_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/security/query_security_request_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/security/query_security_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/security/query_security_response_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/security/query_security_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/security/query_security_response_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/security/query_security_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/create_transaction_request_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/create_transaction_request_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/create_transaction_request_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/create_transaction_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/create_transaction_response_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/create_transaction_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/create_transaction_response_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/create_transaction_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/query_transaction_request_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/valuation/valuation_request_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: fintekkers/requests/transaction/query_transaction_request.proto
+# source: fintekkers/requests/valuation/valuation_request.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from fintekkers.models.util import uuid_pb2 as fintekkers_dot_models_dot_util_dot_uuid__pb2
-from fintekkers.models.util import local_timestamp_pb2 as fintekkers_dot_models_dot_util_dot_local__timestamp__pb2
-from fintekkers.models.position import position_filter_pb2 as fintekkers_dot_models_dot_position_dot_position__filter__pb2
+from fintekkers.models.security import security_pb2 as fintekkers_dot_models_dot_security_dot_security__pb2
+from fintekkers.models.position import position_pb2 as fintekkers_dot_models_dot_position_dot_position__pb2
+from fintekkers.models.price import price_pb2 as fintekkers_dot_models_dot_price_dot_price__pb2
+from fintekkers.requests.util import operation_pb2 as fintekkers_dot_requests_dot_util_dot_operation__pb2
+from fintekkers.models.position import measure_pb2 as fintekkers_dot_models_dot_position_dot_measure__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n?fintekkers/requests/transaction/query_transaction_request.proto\x12\x1f\x66intekkers.requests.transaction\x1a!fintekkers/models/util/uuid.proto\x1a,fintekkers/models/util/local_timestamp.proto\x1a\x30\x66intekkers/models/position/position_filter.proto\"\x86\x02\n\x1cQueryTransactionRequestProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x30\n\x05uuids\x18\x15 \x03(\x0b\x32!.fintekkers.models.util.UUIDProto\x12Q\n\x18search_transaction_input\x18\x16 \x01(\x0b\x32/.fintekkers.models.position.PositionFilterProto\x12:\n\x05\x61s_of\x18\x17 \x01(\x0b\x32+.fintekkers.models.util.LocalTimestampProtoB!B\x1dQueryTransactionRequestProtosP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5fintekkers/requests/valuation/valuation_request.proto\x12\x1d\x66intekkers.requests.valuation\x1a)fintekkers/models/security/security.proto\x1a)fintekkers/models/position/position.proto\x1a#fintekkers/models/price/price.proto\x1a(fintekkers/requests/util/operation.proto\x1a(fintekkers/models/position/measure.proto\"\x87\x03\n\x15ValuationRequestProto\x12\x14\n\x0cobject_class\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12K\n\x0eoperation_type\x18\n \x01(\x0e\x32\x33.fintekkers.requests.util.RequestOperationTypeProto\x12:\n\x08measures\x18\x1e \x03(\x0e\x32(.fintekkers.models.position.MeasureProto\x12\x41\n\x0esecurity_input\x18\x14 \x01(\x0b\x32).fintekkers.models.security.SecurityProto\x12\x41\n\x0eposition_input\x18\x15 \x01(\x0b\x32).fintekkers.models.position.PositionProto\x12\x38\n\x0bprice_input\x18\x16 \x01(\x0b\x32#.fintekkers.models.price.PriceProtoB\x1a\x42\x16ValuationRequestProtosP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.requests.transaction.query_transaction_request_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fintekkers.requests.valuation.valuation_request_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'B\035QueryTransactionRequestProtosP\001'
-  _QUERYTRANSACTIONREQUESTPROTO._serialized_start=232
-  _QUERYTRANSACTIONREQUESTPROTO._serialized_end=494
+  DESCRIPTOR._serialized_options = b'B\026ValuationRequestProtosP\001'
+  _VALUATIONREQUESTPROTO._serialized_start=296
+  _VALUATIONREQUESTPROTO._serialized_end=687
 # @@protoc_insertion_point(module_scope)
```

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/query_transaction_request_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/query_transaction_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/query_transaction_response_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/query_transaction_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/transaction/query_transaction_response_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/transaction/query_transaction_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/error_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/error_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/error_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/message_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/message_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/message_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/summary_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/summary_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/util/errors/summary_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/util/errors/summary_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/util/lock/lock_request_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/util/lock/lock_request_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/util/lock/lock_request_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/util/lock/lock_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/util/lock/lock_response_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/util/lock/lock_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/util/lock/lock_response_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/util/lock/lock_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/util/operation_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/util/operation_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/valuation/valuation_request_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/valuation/valuation_request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/valuation/valuation_response_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/valuation/valuation_response_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/requests/valuation/valuation_response_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/requests/valuation/valuation_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/lock_service/lock_service_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/services/lock_service/lock_service_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/lock_service/lock_service_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/services/lock_service/lock_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/lock_service/lock_service_pb2_grpc.py` & `fintekkers-ledger-models-0.1.47/fintekkers/services/lock_service/lock_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/portfolio_service/portfolio_service_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/services/portfolio_service/portfolio_service_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/portfolio_service/portfolio_service_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/services/portfolio_service/portfolio_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/portfolio_service/portfolio_service_pb2_grpc.py` & `fintekkers-ledger-models-0.1.47/fintekkers/services/portfolio_service/portfolio_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/position_service/position_service_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/services/position_service/position_service_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/position_service/position_service_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/services/position_service/position_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/position_service/position_service_pb2_grpc.py` & `fintekkers-ledger-models-0.1.47/fintekkers/services/position_service/position_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/security_service/security_service_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/services/security_service/security_service_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/security_service/security_service_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/services/security_service/security_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/security_service/security_service_pb2_grpc.py` & `fintekkers-ledger-models-0.1.47/fintekkers/services/security_service/security_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/transaction_service/transaction_service_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/services/transaction_service/transaction_service_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/transaction_service/transaction_service_pb2.pyi` & `fintekkers-ledger-models-0.1.47/fintekkers/services/transaction_service/transaction_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/transaction_service/transaction_service_pb2_grpc.py` & `fintekkers-ledger-models-0.1.47/fintekkers/services/transaction_service/transaction_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/valuation_service/valuation_service_pb2.py` & `fintekkers-ledger-models-0.1.47/fintekkers/services/valuation_service/valuation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/services/valuation_service/valuation_service_pb2_grpc.py` & `fintekkers-ledger-models-0.1.47/fintekkers/services/valuation_service/valuation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/portfolio.py` & `fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/portfolio.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/position.py` & `fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/position.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,18 +64,18 @@
 
         raise ValueError("Could not find measure in position")
 
     def get_field_display(self, field_to_get:FieldProto):
         field_value = self.get_field(field_to_get=field_to_get)
         return field_value.__str__()
 
-    def get_measures(self):
+    def get_measures(self) -> list[MeasureMapEntry]:
         return self.positionProto.measures
 
-    def get_fields(self):
+    def get_fields(self) -> list[FieldMapEntry]:
         return self.positionProto.fields
     
     def __str__(self):
         out:StringIO = StringIO()
         
         for field in self.get_fields():
             out.write(FieldProto.Name(number=field.field))
```

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/security.py` & `fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/security.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/tenor.py` & `fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/tenor.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/transaction.py` & `fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/transaction.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/util/date_utils.py` & `fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/util/date_utils.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/util/environment.py` & `fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/util/environment.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/util/fintekkers_uuid.py` & `fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/util/fintekkers_uuid.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/wrappers/models/util/serialization.py` & `fintekkers-ledger-models-0.1.47/fintekkers/wrappers/models/util/serialization.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/wrappers/requests/security.py` & `fintekkers-ledger-models-0.1.47/fintekkers/wrappers/requests/security.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/wrappers/requests/transaction.py` & `fintekkers-ledger-models-0.1.47/fintekkers/wrappers/requests/transaction.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers/wrappers/services/security.py` & `fintekkers-ledger-models-0.1.47/fintekkers/wrappers/services/security.py`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers_ledger_models.egg-info/PKG-INFO` & `fintekkers-ledger-models-0.1.47/fintekkers_ledger_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fintekkers-ledger-models
-Version: 0.1.46
+Version: 0.1.47
 Summary: Fintekkers Ledger Models python package
 Home-page: https://github.com/fintekkers/ledger-models
 Author: David Doherty
 Author-email: dave@fintekkers.org
 License: MIT
 Keywords: fintekkers ledger models
 Platform: UNKNOWN
```

### Comparing `fintekkers-ledger-models-0.1.46/fintekkers_ledger_models.egg-info/SOURCES.txt` & `fintekkers-ledger-models-0.1.47/fintekkers_ledger_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fintekkers-ledger-models-0.1.46/setup.py` & `fintekkers-ledger-models-0.1.47/setup.py`

 * *Files identical despite different names*

