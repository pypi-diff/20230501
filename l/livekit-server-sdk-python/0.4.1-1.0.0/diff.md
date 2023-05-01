# Comparing `tmp/livekit_server_sdk_python-0.4.1.tar.gz` & `tmp/livekit_server_sdk_python-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_server_sdk_python-0.4.1.tar", last modified: Fri Dec 16 18:49:09 2022, max compression
+gzip compressed data, was "livekit_server_sdk_python-1.0.0.tar", last modified: Mon May  1 19:06:07 2023, max compression
```

## Comparing `livekit_server_sdk_python-0.4.1.tar` & `livekit_server_sdk_python-1.0.0.tar`

### file list

```diff
@@ -1,46 +1,60 @@
-drwxr-xr-x   0 amohr     (1000) amohr     (1000)        0 2022-12-16 18:49:09.149116 livekit_server_sdk_python-0.4.1/
--rw-r--r--   0 amohr     (1000) amohr     (1000)    11358 2022-12-16 17:05:13.000000 livekit_server_sdk_python-0.4.1/LICENCE
--rw-r--r--   0 amohr     (1000) amohr     (1000)     2856 2022-12-16 18:49:09.149116 livekit_server_sdk_python-0.4.1/PKG-INFO
--rw-r--r--   0 amohr     (1000) amohr     (1000)     1947 2022-12-16 17:05:13.000000 livekit_server_sdk_python-0.4.1/README.md
-drwxr-xr-x   0 amohr     (1000) amohr     (1000)        0 2022-12-16 18:49:09.145783 livekit_server_sdk_python-0.4.1/livekit/
--rw-r--r--   0 amohr     (1000) amohr     (1000)     9211 2022-12-16 18:44:41.000000 livekit_server_sdk_python-0.4.1/livekit/__init__.py
-drwxr-xr-x   0 amohr     (1000) amohr     (1000)        0 2022-12-16 18:49:09.145783 livekit_server_sdk_python-0.4.1/livekit/proto/
--rw-r--r--   0 amohr     (1000) amohr     (1000)        0 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/__init__.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)     6375 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_analytics_pb2.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)    10465 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_analytics_pb2.pyi
--rw-r--r--   0 amohr     (1000) amohr     (1000)    14065 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_egress_pb2.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)    22259 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_egress_pb2.pyi
--rw-r--r--   0 amohr     (1000) amohr     (1000)     5981 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_ingress_pb2.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)     9527 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_ingress_pb2.pyi
--rw-r--r--   0 amohr     (1000) amohr     (1000)     6430 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_internal_pb2.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)    12805 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_internal_pb2.pyi
--rw-r--r--   0 amohr     (1000) amohr     (1000)    12133 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_models_pb2.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)    22752 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_models_pb2.pyi
--rw-r--r--   0 amohr     (1000) amohr     (1000)     6346 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_room_pb2.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)     7502 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_room_pb2.pyi
--rw-r--r--   0 amohr     (1000) amohr     (1000)     4186 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_rpc_internal_pb2.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)     6922 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_rpc_internal_pb2.pyi
--rw-r--r--   0 amohr     (1000) amohr     (1000)    12516 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_rtc_pb2.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)    24196 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_rtc_pb2.pyi
--rw-r--r--   0 amohr     (1000) amohr     (1000)     1875 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_webhook_pb2.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)     1910 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/proto/livekit_webhook_pb2.pyi
-drwxr-xr-x   0 amohr     (1000) amohr     (1000)        0 2022-12-16 18:49:09.145783 livekit_server_sdk_python-0.4.1/livekit/twirp/
--rw-r--r--   0 amohr     (1000) amohr     (1000)        0 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/twirp/__init__.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)     2083 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/twirp/livekit_analytics_twirp.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)     6160 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/twirp/livekit_egress_twirp.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)     3334 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/twirp/livekit_ingress_twirp.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)      348 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/twirp/livekit_internal_twirp.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)      346 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/twirp/livekit_models_twirp.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)     8454 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/twirp/livekit_room_twirp.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)      352 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/twirp/livekit_rpc_internal_twirp.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)      343 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/twirp/livekit_rtc_twirp.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)      347 2022-12-16 18:38:25.000000 livekit_server_sdk_python-0.4.1/livekit/twirp/livekit_webhook_twirp.py
--rw-r--r--   0 amohr     (1000) amohr     (1000)      401 2022-12-16 17:05:13.000000 livekit_server_sdk_python-0.4.1/livekit/utils.py
-drwxr-xr-x   0 amohr     (1000) amohr     (1000)        0 2022-12-16 18:49:09.149116 livekit_server_sdk_python-0.4.1/livekit_server_sdk_python.egg-info/
--rw-r--r--   0 amohr     (1000) amohr     (1000)     2856 2022-12-16 18:49:09.000000 livekit_server_sdk_python-0.4.1/livekit_server_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 amohr     (1000) amohr     (1000)     1398 2022-12-16 18:49:09.000000 livekit_server_sdk_python-0.4.1/livekit_server_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 amohr     (1000) amohr     (1000)        1 2022-12-16 18:49:09.000000 livekit_server_sdk_python-0.4.1/livekit_server_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 amohr     (1000) amohr     (1000)      109 2022-12-16 18:49:09.000000 livekit_server_sdk_python-0.4.1/livekit_server_sdk_python.egg-info/requires.txt
--rw-r--r--   0 amohr     (1000) amohr     (1000)        8 2022-12-16 18:49:09.000000 livekit_server_sdk_python-0.4.1/livekit_server_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 amohr     (1000) amohr     (1000)      426 2022-12-16 17:05:13.000000 livekit_server_sdk_python-0.4.1/pyproject.toml
--rw-r--r--   0 amohr     (1000) amohr     (1000)     1132 2022-12-16 18:49:09.149116 livekit_server_sdk_python-0.4.1/setup.cfg
+drwxr-xr-x   0 amohr     (1000) amohr     (1000)        0 2023-05-01 19:06:07.940331 livekit_server_sdk_python-1.0.0/
+-rw-r--r--   0 amohr     (1000) amohr     (1000)    11358 2022-12-16 17:05:13.000000 livekit_server_sdk_python-1.0.0/LICENCE
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     3130 2023-05-01 19:06:07.940331 livekit_server_sdk_python-1.0.0/PKG-INFO
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     2221 2023-05-01 19:02:47.000000 livekit_server_sdk_python-1.0.0/README.md
+drwxr-xr-x   0 amohr     (1000) amohr     (1000)        0 2023-05-01 19:06:07.936998 livekit_server_sdk_python-1.0.0/livekit/
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     8257 2023-05-01 19:04:14.000000 livekit_server_sdk_python-1.0.0/livekit/__init__.py
+drwxr-xr-x   0 amohr     (1000) amohr     (1000)        0 2023-05-01 19:06:07.940331 livekit_server_sdk_python-1.0.0/livekit/_proto/
+-rw-r--r--   0 amohr     (1000) amohr     (1000)        0 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/__init__.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     6928 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_analytics_pb2.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)    11469 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_analytics_pb2.pyi
+-rw-r--r--   0 amohr     (1000) amohr     (1000)    17224 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_egress_pb2.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)    25846 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_egress_pb2.pyi
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     7397 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_ingress_pb2.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)    11285 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_ingress_pb2.pyi
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     7977 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_internal_pb2.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)    17109 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_internal_pb2.pyi
+-rw-r--r--   0 amohr     (1000) amohr     (1000)    13490 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_models_pb2.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)    24354 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_models_pb2.pyi
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     6424 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_room_pb2.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     7602 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_room_pb2.pyi
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     2862 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_rpc_internal_pb2.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     3627 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_rpc_internal_pb2.pyi
+-rw-r--r--   0 amohr     (1000) amohr     (1000)    14157 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_rtc_pb2.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)    27666 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_rtc_pb2.pyi
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     1917 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_webhook_pb2.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     2042 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_webhook_pb2.pyi
+drwxr-xr-x   0 amohr     (1000) amohr     (1000)        0 2023-05-01 19:06:07.940331 livekit_server_sdk_python-1.0.0/livekit/_twirp/
+-rw-r--r--   0 amohr     (1000) amohr     (1000)        0 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_twirp/__init__.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     2083 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_twirp/livekit_analytics_twirp.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     6160 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_twirp/livekit_egress_twirp.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     3334 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_twirp/livekit_ingress_twirp.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)      348 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_twirp/livekit_internal_twirp.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)      346 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_twirp/livekit_models_twirp.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     8454 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_twirp/livekit_room_twirp.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)      352 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_twirp/livekit_rpc_internal_twirp.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)      343 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_twirp/livekit_rtc_twirp.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)      347 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_twirp/livekit_webhook_twirp.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)      401 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/_utils.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)       59 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/analytics.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)       56 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/egress.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)       57 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/ingress.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)       58 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/internal.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)       56 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/models.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)       54 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/room.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)       62 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/rpc_internal.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)       53 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/rtc.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)      408 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/twirp.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)       57 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/livekit/webhook.py
+drwxr-xr-x   0 amohr     (1000) amohr     (1000)        0 2023-05-01 19:06:07.940331 livekit_server_sdk_python-1.0.0/livekit_server_sdk_python.egg-info/
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     3130 2023-05-01 19:06:07.000000 livekit_server_sdk_python-1.0.0/livekit_server_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     1696 2023-05-01 19:06:07.000000 livekit_server_sdk_python-1.0.0/livekit_server_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 amohr     (1000) amohr     (1000)        1 2023-05-01 19:06:07.000000 livekit_server_sdk_python-1.0.0/livekit_server_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 amohr     (1000) amohr     (1000)      109 2023-05-01 19:06:07.000000 livekit_server_sdk_python-1.0.0/livekit_server_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 amohr     (1000) amohr     (1000)        8 2023-05-01 19:06:07.000000 livekit_server_sdk_python-1.0.0/livekit_server_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 amohr     (1000) amohr     (1000)      426 2022-12-16 17:05:13.000000 livekit_server_sdk_python-1.0.0/pyproject.toml
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     1132 2023-05-01 19:06:07.940331 livekit_server_sdk_python-1.0.0/setup.cfg
+drwxr-xr-x   0 amohr     (1000) amohr     (1000)        0 2023-05-01 19:06:07.940331 livekit_server_sdk_python-1.0.0/tests/
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     1558 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/tests/test_access_token.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)     1696 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/tests/test_room_service_client.py
+-rw-r--r--   0 amohr     (1000) amohr     (1000)      298 2023-05-01 18:55:32.000000 livekit_server_sdk_python-1.0.0/tests/test_utils.py
```

### Comparing `livekit_server_sdk_python-0.4.1/LICENCE` & `livekit_server_sdk_python-1.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `livekit_server_sdk_python-0.4.1/PKG-INFO` & `livekit_server_sdk_python-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit_server_sdk_python
-Version: 0.4.1
+Version: 1.0.0
 Summary: Livekit Server SDK for Python
 Home-page: https://github.com/tradablebits/livekit-server-sdk-python
 Author: Tradable Bits
 Author-email: dev@tradablebits.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/tradablebits/livekit-server-sdk-python/issues
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,36 +20,43 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENCE
 
 # LiveKit Server SDK
 
 ![https://pypi.org/project/livekit-server-sdk-python/](https://img.shields.io/pypi/v/livekit-server-sdk-python.svg)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 API Reference: https://docs.livekit.io/guides/server-api
 
 ## Examples
 
 ### Generate Access Token for a Client
 
 ```py
-from livekit import AccessToken, VideoGrant
+import livekit
 
-grant = VideoGrant(room_join=True, room="My Cool Room")
-access_token = AccessToken("<api key>", "<api secret>", grant=grant, identity="bob", name="Bob")
+grant = livekit.VideoGrant(room_join=True, room="My Cool Room")
+access_token = livekit.AccessToken("<api key>", "<api secret>", grant=grant, identity="bob", name="Bob")
 token = access_token.to_jwt()
 ```
 
 ### Using `RoomServiceClient`
 
 ```py
-from livekit import RoomServiceClient
+import livekit
 
-client = RoomServiceClient("<host>", "<api key>", "<api secret>")
-client.mute_published_track(room="<room name>", track="<track sid>")
+client = livekit.RoomServiceClient("<host>", "<api key>", "<api secret>")
+client.mute_published_track(
+    room="<room name>",
+    identity="Bob",
+    track_sid="<track sid>",
+    muted=True,
+)
 ```
 
 ## Local Development
 
 Make sure you clone with submodules:
 ```sh
 $ git clone --recurse-submodules https://github.com/tradablebits/livekit-server-sdk-python.git
```

### Comparing `livekit_server_sdk_python-0.4.1/README.md` & `livekit_server_sdk_python-1.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 # LiveKit Server SDK
 
 ![https://pypi.org/project/livekit-server-sdk-python/](https://img.shields.io/pypi/v/livekit-server-sdk-python.svg)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 API Reference: https://docs.livekit.io/guides/server-api
 
 ## Examples
 
 ### Generate Access Token for a Client
 
 ```py
-from livekit import AccessToken, VideoGrant
+import livekit
 
-grant = VideoGrant(room_join=True, room="My Cool Room")
-access_token = AccessToken("<api key>", "<api secret>", grant=grant, identity="bob", name="Bob")
+grant = livekit.VideoGrant(room_join=True, room="My Cool Room")
+access_token = livekit.AccessToken("<api key>", "<api secret>", grant=grant, identity="bob", name="Bob")
 token = access_token.to_jwt()
 ```
 
 ### Using `RoomServiceClient`
 
 ```py
-from livekit import RoomServiceClient
+import livekit
 
-client = RoomServiceClient("<host>", "<api key>", "<api secret>")
-client.mute_published_track(room="<room name>", track="<track sid>")
+client = livekit.RoomServiceClient("<host>", "<api key>", "<api secret>")
+client.mute_published_track(
+    room="<room name>",
+    identity="Bob",
+    track_sid="<track sid>",
+    muted=True,
+)
 ```
 
 ## Local Development
 
 Make sure you clone with submodules:
 ```sh
 $ git clone --recurse-submodules https://github.com/tradablebits/livekit-server-sdk-python.git
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/__init__.py` & `livekit_server_sdk_python-1.0.0/livekit/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,261 +1,220 @@
 """LiveKit Server SDK
 
-Modeled after the official LiveKit Server SDK:
+Loosely modeled after the official LiveKit Server SDK:
 https://docs.livekit.io/server-sdk-js/
 """
 
-__all__ = [
-    # utils
-    "utils",
-    "AccessToken",
-    "VideoGrant",
-    # analytics
-    "AnalyticsRecorderServiceClient",
-    "AnalyticsRecorderServiceServer",
-    # models
-    "DataPacketKind",
-    "ParticipantInfo",
-    "Room",
-    "TrackInfo",
-    # room
-    "CreateRoomRequest",
-    "RoomEgress",
-    "DeleteRoomRequest",
-    "DeleteRoomResponse",
-    "ListParticipantsRequest",
-    "ListParticipantsResponse",
-    "ListRoomsRequest",
-    "ListRoomsResponse",
-    "MuteRoomTrackRequest",
-    "MuteRoomTrackResponse",
-    "RemoveParticipantResponse",
-    "RoomParticipantIdentity",
-    "SendDataRequest",
-    "SendDataResponse",
-    "UpdateParticipantRequest",
-    "UpdateRoomMetadataRequest",
-    "UpdateSubscriptionsRequest",
-    "UpdateSubscriptionsResponse",
-    # room service
-    "RoomServiceClient",
-    "RoomServiceServer",
-]
-
-__version__ = "0.4.1"
+__version__ = "1.0.0"
 
 import calendar
-from dataclasses import asdict, dataclass, field
-from datetime import datetime, timedelta
-from enum import IntEnum
-from typing import List, Optional
+import dataclasses
+import datetime
+import typing as t
 
 import jwt
-from twirp.context import Context  # noqa
+from twirp.context import Context as _TwirpContext
 
-from livekit import utils
-from livekit.proto.livekit_analytics_pb2 import *
-from livekit.proto.livekit_models_pb2 import *
-from livekit.proto.livekit_room_pb2 import *
-from livekit.twirp.livekit_analytics_twirp import *
-from livekit.twirp.livekit_room_twirp import RoomServiceClient as TwirpRoomServiceClient
-from livekit.twirp.livekit_room_twirp import RoomServiceServer
+from livekit import _utils
+from livekit import models as _models
+from livekit import room as _room
+from livekit import twirp as _twirp
 
-DEFAULT_TOKEN_TTL = timedelta(hours=6)
+DEFAULT_TOKEN_TTL = datetime.timedelta(hours=6)
 
 
-@dataclass
+@dataclasses.dataclass
 class VideoGrant:
-    room_create: Optional[bool] = None
-    room_join: Optional[bool] = None
-    room_list: Optional[bool] = None
-    room_record: Optional[bool] = None
-    room_admin: Optional[bool] = None
-    room: Optional[str] = None
-    can_publish: Optional[bool] = None
-    can_subscribe: Optional[bool] = None
-    can_publish_data: Optional[bool] = None
-    hidden: Optional[bool] = None
+    room_create: t.Optional[bool] = None
+    room_join: t.Optional[bool] = None
+    room_list: t.Optional[bool] = None
+    room_record: t.Optional[bool] = None
+    room_admin: t.Optional[bool] = None
+    room: t.Optional[str] = None
+    can_publish: t.Optional[bool] = None
+    can_subscribe: t.Optional[bool] = None
+    can_publish_data: t.Optional[bool] = None
+    hidden: t.Optional[bool] = None
 
 
-@dataclass
+@dataclasses.dataclass
 class AccessToken:
     api_key: str
     api_secret: str
-    grant: VideoGrant = field(default_factory=VideoGrant)
-    identity: Optional[str] = None
-    name: Optional[str] = None
-    ttl: timedelta = DEFAULT_TOKEN_TTL
-    metadata: Optional[str] = None
+    grant: VideoGrant = dataclasses.field(default_factory=VideoGrant)
+    identity: t.Optional[str] = None
+    name: t.Optional[str] = None
+    ttl: datetime.timedelta = DEFAULT_TOKEN_TTL
+    metadata: t.Optional[str] = None
 
     def __post_init__(self):
         if self.grant.room_join and self.identity is None:
             raise ValueError("identity is required for room_join grant")
         if self.ttl.total_seconds() <= 0:
             raise ValueError("AccessToken must expire in the future.")
 
     def to_jwt(self) -> str:
         payload = {
-            "video": asdict(self.grant, dict_factory=utils.camel_case_dict),
+            "video": dataclasses.asdict(
+                self.grant, dict_factory=_utils.camel_case_dict
+            ),
             "iss": self.api_key,
-            "nbf": calendar.timegm(datetime.utcnow().utctimetuple()),
-            "exp": calendar.timegm((datetime.utcnow() + self.ttl).utctimetuple()),
+            "nbf": calendar.timegm(datetime.datetime.utcnow().utctimetuple()),
+            "exp": calendar.timegm(
+                (datetime.datetime.utcnow() + self.ttl).utctimetuple()
+            ),
         }
         if self.metadata is not None:
             payload["metadata"] = self.metadata
         if self.identity is not None:
             payload["sub"] = self.identity
         if self.name:
             payload["name"] = self.name
         return jwt.encode(payload, self.api_secret)
 
 
-class DataPacketKind(IntEnum):
-    RELIABLE = 0
-    LOSSY = 1
-
-
 class RoomServiceClient:
     """
     Client to access Room APIs
     """
 
     def __init__(self, host: str, api_key: str, api_secret: str):
-        self._client = TwirpRoomServiceClient(host)
+        self._client = _twirp.RoomServiceClient(host)
         self._api_key = api_key
         self._api_secret = api_secret
 
     def _create_context(self, **grant_kwargs):
         grant = VideoGrant(**grant_kwargs)
         access_token = AccessToken(
             self._api_key,
             self._api_secret,
             grant=grant,
-            ttl=timedelta(minutes=10),
+            ttl=datetime.timedelta(minutes=10),
+        )
+        return _TwirpContext(
+            headers={"Authorization": f"Bearer {access_token.to_jwt()}"}
         )
-        return Context(headers={"Authorization": f"Bearer {access_token.to_jwt()}"})
 
     def create_room(
         self,
         name: str,
-        empty_timeout: Optional[int] = None,
-        max_participants: Optional[int] = None,
-    ) -> Room:
+        empty_timeout: t.Optional[int] = None,
+        max_participants: t.Optional[int] = None,
+    ) -> _models.Room:
         """
         Creates a new room. Explicit room creation is not required, since rooms will
         be automatically created when the first participant joins. This method can be
         used to customize room settings.
         """
 
         ctx = self._create_context(room_create=True)
-        request = CreateRoomRequest(
+        request = _room.CreateRoomRequest(
             name=name,
             empty_timeout=empty_timeout,
             max_participants=max_participants,
         )
         return self._client.CreateRoom(ctx=ctx, request=request)
 
-    def list_rooms(self) -> List[Room]:
+    def list_rooms(self) -> t.List[_models.Room]:
         """
         List rooms that are active on the server.
         """
         ctx = self._create_context(room_list=True)
-        request = ListRoomsRequest()
+        request = _room.ListRoomsRequest()
         response = self._client.ListRooms(ctx=ctx, request=request)
         return [r for r in response.rooms]
 
     def delete_room(self, room: str):
         """
         Deletes an existing room by name or id. Will disconnect all participants that
         are currently in the room.
         """
-        # TODO: seems like only `room_create` should be necessary
         ctx = self._create_context(room_create=True, room_admin=True, room=room)
-        request = DeleteRoomRequest(room=room)
+        request = _room.DeleteRoomRequest(room=room)
         self._client.DeleteRoom(ctx=ctx, request=request)
 
-    def list_participants(self, room: str) -> List[ParticipantInfo]:
+    def list_participants(self, room: str) -> t.List[_models.ParticipantInfo]:
         """
         Lists participants in a room
         """
         ctx = self._create_context(room_admin=True, room=room)
-        request = ListParticipantsRequest(room=room)
+        request = _room.ListParticipantsRequest(room=room)
         response = self._client.ListParticipants(ctx=ctx, request=request)
         return [p for p in response.participants]
 
-    def get_participant(self, room: str, identity: str) -> ParticipantInfo:
+    def get_participant(self, room: str, identity: str) -> _models.ParticipantInfo:
         """
         Gets information on a specific participant
         """
         ctx = self._create_context(room_admin=True, room=room)
-        request = RoomParticipantIdentity(room=room, identity=identity)
+        request = _room.RoomParticipantIdentity(room=room, identity=identity)
         return self._client.GetParticipant(ctx=ctx, request=request)
 
     def remove_participant(self, room: str, identity: str):
         """
         Removes a participant from room.
         """
         ctx = self._create_context(room_admin=True, room=room)
-        request = RoomParticipantIdentity(room=room, identity=identity)
+        request = _room.RoomParticipantIdentity(room=room, identity=identity)
         self._client.RemoveParticipant(ctx=ctx, request=request)
 
     def mute_published_track(
         self,
         room: str,
         identity: str,
         track_sid: str,
         muted: bool,
     ):
         """
         Mute/unmute a participant's track.
         """
         ctx = self._create_context(room_admin=True, room=room)
-        request = MuteRoomTrackRequest(
+        request = _room.MuteRoomTrackRequest(
             room=room,
             identity=identity,
             track_sid=track_sid,
             muted=muted,
         )
         self._client.MutePublishedTrack(ctx=ctx, request=request)
 
     def update_participant(
         self,
         room: str,
         identity: str,
         metadata: str = "",
-        permission: Optional[ParticipantPermission] = None,
+        permission: t.Optional[_models.ParticipantPermission] = None,
     ):
         """
         Update participant metadata, will cause updates to be broadcasted to everyone
         in the room.
         """
         ctx = self._create_context(room_admin=True, room=room)
-        request = UpdateParticipantRequest(
+        request = _room.UpdateParticipantRequest(
             room=room,
             identity=identity,
             metadata=metadata,
             permission=permission,
         )
         self._client.UpdateParticipant(ctx=ctx, request=request)
 
     def update_subscriptions(
         self,
         room: str,
         identity: str,
-        track_sids: List[str],
+        track_sids: t.List[str],
         subscribe: bool,
     ):
         """
         Subscribes or unsubscribe a participant from tracks.
 
         As an admin, you can subscribe a participant to a track even if they do not
         have canSubscribe permission.
         """
         ctx = self._create_context(room_admin=True, room=room)
-        request = UpdateSubscriptionsRequest(
+        request = _room.UpdateSubscriptionsRequest(
             room=room,
             identity=identity,
             track_sids=track_sids,
             subscribe=subscribe,
         )
         self._client.UpdateSubscriptions(ctx=ctx, request=request)
 
@@ -263,30 +222,30 @@
         """
         Update room level metadata.
 
         This API allows you to attach user-defined metadata to a room.
         Changes to metadata will be broadcasted to all participants in the room.
         """
         ctx = self._create_context(room_admin=True, room=room)
-        request = UpdateRoomMetadataRequest(room=room, metadata=metadata)
+        request = _room.UpdateRoomMetadataRequest(room=room, metadata=metadata)
         self._client.UpdateRoomMetadata(ctx=ctx, request=request)
 
     def send_data(
         self,
         room: str,
         data: bytes,
-        kind: DataPacketKind,
-        destination_sids: Optional[List[str]] = None,
+        kind: _models.DataPacket.Kind,
+        destination_sids: t.Optional[t.List[str]] = None,
     ):
         """
         Sends data messages to participants, triggering `onDataReceived` event on clients.
         """
         if destination_sids is None:
             destination_sids = []
         ctx = self._create_context(room_admin=True, room=room)
-        request = SendDataRequest(
+        request = _room.SendDataRequest(
             room=room,
             data=data,
-            kind=kind.value,
+            kind=kind,
             destination_sids=destination_sids,
         )
         self._client.SendData(ctx=ctx, request=request)
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_analytics_pb2.py` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_analytics_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,37 +16,36 @@
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 from . import livekit_egress_pb2 as livekit__egress__pb2
 from . import livekit_ingress_pb2 as livekit__ingress__pb2
 from . import livekit_models_pb2 as livekit__models__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x17livekit_analytics.proto\x12\x07livekit\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x14livekit_models.proto\x1a\x14livekit_egress.proto\x1a\x15livekit_ingress.proto"T\n\x13\x41nalyticsVideoLayer\x12\r\n\x05layer\x18\x01 \x01(\x05\x12\x0f\n\x07packets\x18\x02 \x01(\r\x12\r\n\x05\x62ytes\x18\x03 \x01(\x04\x12\x0e\n\x06\x66rames\x18\x04 \x01(\r"\xd7\x02\n\x0f\x41nalyticsStream\x12\x0c\n\x04ssrc\x18\x01 \x01(\r\x12\x17\n\x0fprimary_packets\x18\x02 \x01(\r\x12\x15\n\rprimary_bytes\x18\x03 \x01(\x04\x12\x1a\n\x12retransmit_packets\x18\x04 \x01(\r\x12\x18\n\x10retransmit_bytes\x18\x05 \x01(\x04\x12\x17\n\x0fpadding_packets\x18\x06 \x01(\r\x12\x15\n\rpadding_bytes\x18\x07 \x01(\x04\x12\x14\n\x0cpackets_lost\x18\x08 \x01(\r\x12\x0e\n\x06\x66rames\x18\t \x01(\r\x12\x0b\n\x03rtt\x18\n \x01(\r\x12\x0e\n\x06jitter\x18\x0b \x01(\r\x12\r\n\x05nacks\x18\x0c \x01(\r\x12\x0c\n\x04plis\x18\r \x01(\r\x12\x0c\n\x04\x66irs\x18\x0e \x01(\r\x12\x32\n\x0cvideo_layers\x18\x0f \x03(\x0b\x32\x1c.livekit.AnalyticsVideoLayer"\x9d\x02\n\rAnalyticsStat\x12\x15\n\ranalytics_key\x18\x01 \x01(\t\x12!\n\x04kind\x18\x02 \x01(\x0e\x32\x13.livekit.StreamType\x12.\n\ntime_stamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04node\x18\x04 \x01(\t\x12\x0f\n\x07room_id\x18\x05 \x01(\t\x12\x11\n\troom_name\x18\x06 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x07 \x01(\t\x12\x10\n\x08track_id\x18\x08 \x01(\t\x12\r\n\x05score\x18\t \x01(\x02\x12)\n\x07streams\x18\n \x03(\x0b\x32\x18.livekit.AnalyticsStream\x12\x0c\n\x04mime\x18\x0b \x01(\t"7\n\x0e\x41nalyticsStats\x12%\n\x05stats\x18\x01 \x03(\x0b\x32\x16.livekit.AnalyticsStat"~\n\x13\x41nalyticsClientMeta\x12\x0e\n\x06region\x18\x01 \x01(\t\x12\x0c\n\x04node\x18\x02 \x01(\t\x12\x13\n\x0b\x63lient_addr\x18\x03 \x01(\t\x12\x1b\n\x13\x63lient_connect_time\x18\x04 \x01(\r\x12\x17\n\x0f\x63onnection_type\x18\x05 \x01(\t"\xf3\x04\n\x0e\x41nalyticsEvent\x12)\n\x04type\x18\x01 \x01(\x0e\x32\x1b.livekit.AnalyticsEventType\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07room_id\x18\x03 \x01(\t\x12\x1b\n\x04room\x18\x04 \x01(\x0b\x32\r.livekit.Room\x12\x16\n\x0eparticipant_id\x18\x05 \x01(\t\x12-\n\x0bparticipant\x18\x06 \x01(\x0b\x32\x18.livekit.ParticipantInfo\x12\x10\n\x08track_id\x18\x07 \x01(\t\x12!\n\x05track\x18\x08 \x01(\x0b\x32\x12.livekit.TrackInfo\x12\x15\n\ranalytics_key\x18\n \x01(\t\x12(\n\x0b\x63lient_info\x18\x0b \x01(\x0b\x32\x13.livekit.ClientInfo\x12\x31\n\x0b\x63lient_meta\x18\x0c \x01(\x0b\x32\x1c.livekit.AnalyticsClientMeta\x12\x11\n\tegress_id\x18\r \x01(\t\x12\x12\n\ningress_id\x18\x13 \x01(\t\x12;\n\x1cmax_subscribed_video_quality\x18\x0e \x01(\x0e\x32\x15.livekit.VideoQuality\x12+\n\tpublisher\x18\x0f \x01(\x0b\x32\x18.livekit.ParticipantInfo\x12\x0c\n\x04mime\x18\x10 \x01(\t\x12#\n\x06\x65gress\x18\x11 \x01(\x0b\x32\x13.livekit.EgressInfo\x12%\n\x07ingress\x18\x12 \x01(\x0b\x32\x14.livekit.IngressInfo":\n\x0f\x41nalyticsEvents\x12\'\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x17.livekit.AnalyticsEvent**\n\nStreamType\x12\x0c\n\x08UPSTREAM\x10\x00\x12\x0e\n\nDOWNSTREAM\x10\x01*\xa3\x03\n\x12\x41nalyticsEventType\x12\x10\n\x0cROOM_CREATED\x10\x00\x12\x0e\n\nROOM_ENDED\x10\x01\x12\x16\n\x12PARTICIPANT_JOINED\x10\x02\x12\x14\n\x10PARTICIPANT_LEFT\x10\x03\x12\x13\n\x0fTRACK_PUBLISHED\x10\x04\x12\x15\n\x11TRACK_UNPUBLISHED\x10\x05\x12\x14\n\x10TRACK_SUBSCRIBED\x10\x06\x12\x16\n\x12TRACK_UNSUBSCRIBED\x10\x07\x12\x1a\n\x16TRACK_PUBLISHED_UPDATE\x10\n\x12\x16\n\x12PARTICIPANT_ACTIVE\x10\x0b\x12\x12\n\x0e\x45GRESS_STARTED\x10\x0c\x12\x10\n\x0c\x45GRESS_ENDED\x10\r\x12&\n"TRACK_MAX_SUBSCRIBED_VIDEO_QUALITY\x10\x0e\x12\x0f\n\x0bRECONNECTED\x10\x0f\x12\x13\n\x0fINGRESS_CREATED\x10\x12\x12\x13\n\x0fINGRESS_DELETED\x10\x13\x12\x13\n\x0fINGRESS_STARTED\x10\x10\x12\x11\n\rINGRESS_ENDED\x10\x11\x32\xa4\x01\n\x18\x41nalyticsRecorderService\x12\x42\n\x0bIngestStats\x12\x17.livekit.AnalyticsStats\x1a\x16.google.protobuf.Empty"\x00(\x01\x12\x44\n\x0cIngestEvents\x12\x18.livekit.AnalyticsEvents\x1a\x16.google.protobuf.Empty"\x00(\x01\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
+    b'\n\x17livekit_analytics.proto\x12\x07livekit\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x14livekit_models.proto\x1a\x14livekit_egress.proto\x1a\x15livekit_ingress.proto"T\n\x13\x41nalyticsVideoLayer\x12\r\n\x05layer\x18\x01 \x01(\x05\x12\x0f\n\x07packets\x18\x02 \x01(\r\x12\r\n\x05\x62ytes\x18\x03 \x01(\x04\x12\x0e\n\x06\x66rames\x18\x04 \x01(\r"\xd7\x02\n\x0f\x41nalyticsStream\x12\x0c\n\x04ssrc\x18\x01 \x01(\r\x12\x17\n\x0fprimary_packets\x18\x02 \x01(\r\x12\x15\n\rprimary_bytes\x18\x03 \x01(\x04\x12\x1a\n\x12retransmit_packets\x18\x04 \x01(\r\x12\x18\n\x10retransmit_bytes\x18\x05 \x01(\x04\x12\x17\n\x0fpadding_packets\x18\x06 \x01(\r\x12\x15\n\rpadding_bytes\x18\x07 \x01(\x04\x12\x14\n\x0cpackets_lost\x18\x08 \x01(\r\x12\x0e\n\x06\x66rames\x18\t \x01(\r\x12\x0b\n\x03rtt\x18\n \x01(\r\x12\x0e\n\x06jitter\x18\x0b \x01(\r\x12\r\n\x05nacks\x18\x0c \x01(\r\x12\x0c\n\x04plis\x18\r \x01(\r\x12\x0c\n\x04\x66irs\x18\x0e \x01(\r\x12\x32\n\x0cvideo_layers\x18\x0f \x03(\x0b\x32\x1c.livekit.AnalyticsVideoLayer"\x9d\x02\n\rAnalyticsStat\x12\x15\n\ranalytics_key\x18\x01 \x01(\t\x12!\n\x04kind\x18\x02 \x01(\x0e\x32\x13.livekit.StreamType\x12.\n\ntime_stamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04node\x18\x04 \x01(\t\x12\x0f\n\x07room_id\x18\x05 \x01(\t\x12\x11\n\troom_name\x18\x06 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x07 \x01(\t\x12\x10\n\x08track_id\x18\x08 \x01(\t\x12\r\n\x05score\x18\t \x01(\x02\x12)\n\x07streams\x18\n \x03(\x0b\x32\x18.livekit.AnalyticsStream\x12\x0c\n\x04mime\x18\x0b \x01(\t"7\n\x0e\x41nalyticsStats\x12%\n\x05stats\x18\x01 \x03(\x0b\x32\x16.livekit.AnalyticsStat"\xb2\x01\n\x13\x41nalyticsClientMeta\x12\x0e\n\x06region\x18\x01 \x01(\t\x12\x0c\n\x04node\x18\x02 \x01(\t\x12\x13\n\x0b\x63lient_addr\x18\x03 \x01(\t\x12\x1b\n\x13\x63lient_connect_time\x18\x04 \x01(\r\x12\x17\n\x0f\x63onnection_type\x18\x05 \x01(\t\x12\x32\n\x10reconnect_reason\x18\x06 \x01(\x0e\x32\x18.livekit.ReconnectReason"\xbd\x05\n\x0e\x41nalyticsEvent\x12)\n\x04type\x18\x01 \x01(\x0e\x32\x1b.livekit.AnalyticsEventType\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07room_id\x18\x03 \x01(\t\x12\x1b\n\x04room\x18\x04 \x01(\x0b\x32\r.livekit.Room\x12\x16\n\x0eparticipant_id\x18\x05 \x01(\t\x12-\n\x0bparticipant\x18\x06 \x01(\x0b\x32\x18.livekit.ParticipantInfo\x12\x10\n\x08track_id\x18\x07 \x01(\t\x12!\n\x05track\x18\x08 \x01(\x0b\x32\x12.livekit.TrackInfo\x12\x15\n\ranalytics_key\x18\n \x01(\t\x12(\n\x0b\x63lient_info\x18\x0b \x01(\x0b\x32\x13.livekit.ClientInfo\x12\x31\n\x0b\x63lient_meta\x18\x0c \x01(\x0b\x32\x1c.livekit.AnalyticsClientMeta\x12\x11\n\tegress_id\x18\r \x01(\t\x12\x12\n\ningress_id\x18\x13 \x01(\t\x12;\n\x1cmax_subscribed_video_quality\x18\x0e \x01(\x0e\x32\x15.livekit.VideoQuality\x12+\n\tpublisher\x18\x0f \x01(\x0b\x32\x18.livekit.ParticipantInfo\x12\x0c\n\x04mime\x18\x10 \x01(\t\x12#\n\x06\x65gress\x18\x11 \x01(\x0b\x32\x13.livekit.EgressInfo\x12%\n\x07ingress\x18\x12 \x01(\x0b\x32\x14.livekit.IngressInfo\x12\r\n\x05\x65rror\x18\x14 \x01(\t\x12$\n\trtp_stats\x18\x15 \x01(\x0b\x32\x11.livekit.RTPStats\x12\x13\n\x0bvideo_layer\x18\x16 \x01(\x05":\n\x0f\x41nalyticsEvents\x12\'\n\x06\x65vents\x18\x01 \x03(\x0b\x32\x17.livekit.AnalyticsEvent**\n\nStreamType\x12\x0c\n\x08UPSTREAM\x10\x00\x12\x0e\n\nDOWNSTREAM\x10\x01*\xec\x04\n\x12\x41nalyticsEventType\x12\x10\n\x0cROOM_CREATED\x10\x00\x12\x0e\n\nROOM_ENDED\x10\x01\x12\x16\n\x12PARTICIPANT_JOINED\x10\x02\x12\x14\n\x10PARTICIPANT_LEFT\x10\x03\x12\x13\n\x0fTRACK_PUBLISHED\x10\x04\x12\x1b\n\x17TRACK_PUBLISH_REQUESTED\x10\x14\x12\x15\n\x11TRACK_UNPUBLISHED\x10\x05\x12\x14\n\x10TRACK_SUBSCRIBED\x10\x06\x12\x1d\n\x19TRACK_SUBSCRIBE_REQUESTED\x10\x15\x12\x1a\n\x16TRACK_SUBSCRIBE_FAILED\x10\x19\x12\x16\n\x12TRACK_UNSUBSCRIBED\x10\x07\x12\x1a\n\x16TRACK_PUBLISHED_UPDATE\x10\n\x12\x0f\n\x0bTRACK_MUTED\x10\x17\x12\x11\n\rTRACK_UNMUTED\x10\x18\x12\x17\n\x13TRACK_PUBLISH_STATS\x10\x1a\x12\x19\n\x15TRACK_SUBSCRIBE_STATS\x10\x1b\x12\x16\n\x12PARTICIPANT_ACTIVE\x10\x0b\x12\x17\n\x13PARTICIPANT_RESUMED\x10\x16\x12\x12\n\x0e\x45GRESS_STARTED\x10\x0c\x12\x10\n\x0c\x45GRESS_ENDED\x10\r\x12&\n"TRACK_MAX_SUBSCRIBED_VIDEO_QUALITY\x10\x0e\x12\x0f\n\x0bRECONNECTED\x10\x0f\x12\x13\n\x0fINGRESS_CREATED\x10\x12\x12\x13\n\x0fINGRESS_DELETED\x10\x13\x12\x13\n\x0fINGRESS_STARTED\x10\x10\x12\x11\n\rINGRESS_ENDED\x10\x11\x32\xa4\x01\n\x18\x41nalyticsRecorderService\x12\x42\n\x0bIngestStats\x12\x17.livekit.AnalyticsStats\x1a\x16.google.protobuf.Empty"\x00(\x01\x12\x44\n\x0cIngestEvents\x12\x18.livekit.AnalyticsEvents\x1a\x16.google.protobuf.Empty"\x00(\x01\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "livekit_analytics_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto"
-    _STREAMTYPE._serialized_start = 1760
-    _STREAMTYPE._serialized_end = 1802
-    _ANALYTICSEVENTTYPE._serialized_start = 1805
-    _ANALYTICSEVENTTYPE._serialized_end = 2224
+    _STREAMTYPE._serialized_start = 1887
+    _STREAMTYPE._serialized_end = 1929
+    _ANALYTICSEVENTTYPE._serialized_start = 1932
+    _ANALYTICSEVENTTYPE._serialized_end = 2552
     _ANALYTICSVIDEOLAYER._serialized_start = 165
     _ANALYTICSVIDEOLAYER._serialized_end = 249
     _ANALYTICSSTREAM._serialized_start = 252
     _ANALYTICSSTREAM._serialized_end = 595
     _ANALYTICSSTAT._serialized_start = 598
     _ANALYTICSSTAT._serialized_end = 883
     _ANALYTICSSTATS._serialized_start = 885
     _ANALYTICSSTATS._serialized_end = 940
-    _ANALYTICSCLIENTMETA._serialized_start = 942
-    _ANALYTICSCLIENTMETA._serialized_end = 1068
-    _ANALYTICSEVENT._serialized_start = 1071
-    _ANALYTICSEVENT._serialized_end = 1698
-    _ANALYTICSEVENTS._serialized_start = 1700
-    _ANALYTICSEVENTS._serialized_end = 1758
-    _ANALYTICSRECORDERSERVICE._serialized_start = 2227
-    _ANALYTICSRECORDERSERVICE._serialized_end = 2391
+    _ANALYTICSCLIENTMETA._serialized_start = 943
+    _ANALYTICSCLIENTMETA._serialized_end = 1121
+    _ANALYTICSEVENT._serialized_start = 1124
+    _ANALYTICSEVENT._serialized_end = 1825
+    _ANALYTICSEVENTS._serialized_start = 1827
+    _ANALYTICSEVENTS._serialized_end = 1885
+    _ANALYTICSRECORDERSERVICE._serialized_start = 2555
+    _ANALYTICSRECORDERSERVICE._serialized_end = 2719
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_analytics_pb2.pyi` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_analytics_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -21,109 +21,132 @@
 INGRESS_CREATED: AnalyticsEventType
 INGRESS_DELETED: AnalyticsEventType
 INGRESS_ENDED: AnalyticsEventType
 INGRESS_STARTED: AnalyticsEventType
 PARTICIPANT_ACTIVE: AnalyticsEventType
 PARTICIPANT_JOINED: AnalyticsEventType
 PARTICIPANT_LEFT: AnalyticsEventType
+PARTICIPANT_RESUMED: AnalyticsEventType
 RECONNECTED: AnalyticsEventType
 ROOM_CREATED: AnalyticsEventType
 ROOM_ENDED: AnalyticsEventType
 TRACK_MAX_SUBSCRIBED_VIDEO_QUALITY: AnalyticsEventType
+TRACK_MUTED: AnalyticsEventType
 TRACK_PUBLISHED: AnalyticsEventType
 TRACK_PUBLISHED_UPDATE: AnalyticsEventType
+TRACK_PUBLISH_REQUESTED: AnalyticsEventType
+TRACK_PUBLISH_STATS: AnalyticsEventType
 TRACK_SUBSCRIBED: AnalyticsEventType
+TRACK_SUBSCRIBE_FAILED: AnalyticsEventType
+TRACK_SUBSCRIBE_REQUESTED: AnalyticsEventType
+TRACK_SUBSCRIBE_STATS: AnalyticsEventType
+TRACK_UNMUTED: AnalyticsEventType
 TRACK_UNPUBLISHED: AnalyticsEventType
 TRACK_UNSUBSCRIBED: AnalyticsEventType
 UPSTREAM: StreamType
 
 class AnalyticsClientMeta(_message.Message):
     __slots__ = [
         "client_addr",
         "client_connect_time",
         "connection_type",
         "node",
+        "reconnect_reason",
         "region",
     ]
     CLIENT_ADDR_FIELD_NUMBER: _ClassVar[int]
     CLIENT_CONNECT_TIME_FIELD_NUMBER: _ClassVar[int]
     CONNECTION_TYPE_FIELD_NUMBER: _ClassVar[int]
     NODE_FIELD_NUMBER: _ClassVar[int]
+    RECONNECT_REASON_FIELD_NUMBER: _ClassVar[int]
     REGION_FIELD_NUMBER: _ClassVar[int]
     client_addr: str
     client_connect_time: int
     connection_type: str
     node: str
+    reconnect_reason: _livekit_models_pb2.ReconnectReason
     region: str
     def __init__(
         self,
         region: _Optional[str] = ...,
         node: _Optional[str] = ...,
         client_addr: _Optional[str] = ...,
         client_connect_time: _Optional[int] = ...,
         connection_type: _Optional[str] = ...,
+        reconnect_reason: _Optional[
+            _Union[_livekit_models_pb2.ReconnectReason, str]
+        ] = ...,
     ) -> None: ...
 
 class AnalyticsEvent(_message.Message):
     __slots__ = [
         "analytics_key",
         "client_info",
         "client_meta",
         "egress",
         "egress_id",
+        "error",
         "ingress",
         "ingress_id",
         "max_subscribed_video_quality",
         "mime",
         "participant",
         "participant_id",
         "publisher",
         "room",
         "room_id",
+        "rtp_stats",
         "timestamp",
         "track",
         "track_id",
         "type",
+        "video_layer",
     ]
     ANALYTICS_KEY_FIELD_NUMBER: _ClassVar[int]
     CLIENT_INFO_FIELD_NUMBER: _ClassVar[int]
     CLIENT_META_FIELD_NUMBER: _ClassVar[int]
     EGRESS_FIELD_NUMBER: _ClassVar[int]
     EGRESS_ID_FIELD_NUMBER: _ClassVar[int]
+    ERROR_FIELD_NUMBER: _ClassVar[int]
     INGRESS_FIELD_NUMBER: _ClassVar[int]
     INGRESS_ID_FIELD_NUMBER: _ClassVar[int]
     MAX_SUBSCRIBED_VIDEO_QUALITY_FIELD_NUMBER: _ClassVar[int]
     MIME_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_ID_FIELD_NUMBER: _ClassVar[int]
     PUBLISHER_FIELD_NUMBER: _ClassVar[int]
     ROOM_FIELD_NUMBER: _ClassVar[int]
     ROOM_ID_FIELD_NUMBER: _ClassVar[int]
+    RTP_STATS_FIELD_NUMBER: _ClassVar[int]
     TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
     TRACK_FIELD_NUMBER: _ClassVar[int]
     TRACK_ID_FIELD_NUMBER: _ClassVar[int]
     TYPE_FIELD_NUMBER: _ClassVar[int]
+    VIDEO_LAYER_FIELD_NUMBER: _ClassVar[int]
     analytics_key: str
     client_info: _livekit_models_pb2.ClientInfo
     client_meta: AnalyticsClientMeta
     egress: _livekit_egress_pb2.EgressInfo
     egress_id: str
+    error: str
     ingress: _livekit_ingress_pb2.IngressInfo
     ingress_id: str
     max_subscribed_video_quality: _livekit_models_pb2.VideoQuality
     mime: str
     participant: _livekit_models_pb2.ParticipantInfo
     participant_id: str
     publisher: _livekit_models_pb2.ParticipantInfo
     room: _livekit_models_pb2.Room
     room_id: str
+    rtp_stats: _livekit_models_pb2.RTPStats
     timestamp: _timestamp_pb2.Timestamp
     track: _livekit_models_pb2.TrackInfo
     track_id: str
     type: AnalyticsEventType
+    video_layer: int
     def __init__(
         self,
         type: _Optional[_Union[AnalyticsEventType, str]] = ...,
         timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
         room_id: _Optional[str] = ...,
         room: _Optional[_Union[_livekit_models_pb2.Room, _Mapping]] = ...,
         participant_id: _Optional[str] = ...,
@@ -142,14 +165,17 @@
         ] = ...,
         publisher: _Optional[
             _Union[_livekit_models_pb2.ParticipantInfo, _Mapping]
         ] = ...,
         mime: _Optional[str] = ...,
         egress: _Optional[_Union[_livekit_egress_pb2.EgressInfo, _Mapping]] = ...,
         ingress: _Optional[_Union[_livekit_ingress_pb2.IngressInfo, _Mapping]] = ...,
+        error: _Optional[str] = ...,
+        rtp_stats: _Optional[_Union[_livekit_models_pb2.RTPStats, _Mapping]] = ...,
+        video_layer: _Optional[int] = ...,
     ) -> None: ...
 
 class AnalyticsEvents(_message.Message):
     __slots__ = ["events"]
     EVENTS_FIELD_NUMBER: _ClassVar[int]
     events: _containers.RepeatedCompositeFieldContainer[AnalyticsEvent]
     def __init__(
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_egress_pb2.py` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_rtc_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,95 +1,106 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: livekit_egress.proto
+# source: livekit_rtc.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from . import livekit_models_pb2 as livekit__models__pb2
+
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x14livekit_egress.proto\x12\x07livekit"\xfc\x02\n\x1aRoomCompositeEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x0e\n\x06layout\x18\x02 \x01(\t\x12\x12\n\naudio_only\x18\x03 \x01(\x08\x12\x12\n\nvideo_only\x18\x04 \x01(\x08\x12\x17\n\x0f\x63ustom_base_url\x18\x05 \x01(\t\x12*\n\x04\x66ile\x18\x06 \x01(\x0b\x32\x1a.livekit.EncodedFileOutputH\x00\x12\'\n\x06stream\x18\x07 \x01(\x0b\x32\x15.livekit.StreamOutputH\x00\x12\x30\n\x08segments\x18\n \x01(\x0b\x32\x1c.livekit.SegmentedFileOutputH\x00\x12\x30\n\x06preset\x18\x08 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x01\x12,\n\x08\x61\x64vanced\x18\t \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x01\x42\x08\n\x06outputB\t\n\x07options"\xdc\x02\n\x1bTrackCompositeEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x16\n\x0e\x61udio_track_id\x18\x02 \x01(\t\x12\x16\n\x0evideo_track_id\x18\x03 \x01(\t\x12*\n\x04\x66ile\x18\x04 \x01(\x0b\x32\x1a.livekit.EncodedFileOutputH\x00\x12\'\n\x06stream\x18\x05 \x01(\x0b\x32\x15.livekit.StreamOutputH\x00\x12\x30\n\x08segments\x18\x08 \x01(\x0b\x32\x1c.livekit.SegmentedFileOutputH\x00\x12\x30\n\x06preset\x18\x06 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x01\x12,\n\x08\x61\x64vanced\x18\x07 \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x01\x42\x08\n\x06outputB\t\n\x07options"\x87\x01\n\x12TrackEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x10\n\x08track_id\x18\x02 \x01(\t\x12)\n\x04\x66ile\x18\x03 \x01(\x0b\x32\x19.livekit.DirectFileOutputH\x00\x12\x17\n\rwebsocket_url\x18\x04 \x01(\tH\x00\x42\x08\n\x06output"\xc3\x02\n\x10WebEgressRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\naudio_only\x18\x02 \x01(\x08\x12\x12\n\nvideo_only\x18\x03 \x01(\x08\x12*\n\x04\x66ile\x18\x04 \x01(\x0b\x32\x1a.livekit.EncodedFileOutputH\x00\x12\'\n\x06stream\x18\x05 \x01(\x0b\x32\x15.livekit.StreamOutputH\x00\x12\x30\n\x08segments\x18\x06 \x01(\x0b\x32\x1c.livekit.SegmentedFileOutputH\x00\x12\x30\n\x06preset\x18\x07 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x01\x12,\n\x08\x61\x64vanced\x18\x08 \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x01\x42\x08\n\x06outputB\t\n\x07options"\x8e\x02\n\x11\x45ncodedFileOutput\x12+\n\tfile_type\x18\x01 \x01(\x0e\x32\x18.livekit.EncodedFileType\x12\x10\n\x08\x66ilepath\x18\x02 \x01(\t\x12\x18\n\x10\x64isable_manifest\x18\x06 \x01(\x08\x12\x1f\n\x02s3\x18\x03 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x04 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x05 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x12\'\n\x06\x61liOSS\x18\x07 \x01(\x0b\x32\x15.livekit.AliOSSUploadH\x00\x42\x08\n\x06output"\xcd\x02\n\x13SegmentedFileOutput\x12\x30\n\x08protocol\x18\x01 \x01(\x0e\x32\x1e.livekit.SegmentedFileProtocol\x12\x17\n\x0f\x66ilename_prefix\x18\x02 \x01(\t\x12\x15\n\rplaylist_name\x18\x03 \x01(\t\x12\x18\n\x10segment_duration\x18\x04 \x01(\r\x12\x18\n\x10\x64isable_manifest\x18\x08 \x01(\x08\x12\x1f\n\x02s3\x18\x05 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x06 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x07 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x12\'\n\x06\x61liOSS\x18\t \x01(\x0b\x32\x15.livekit.AliOSSUploadH\x00\x42\x08\n\x06output"\xe0\x01\n\x10\x44irectFileOutput\x12\x10\n\x08\x66ilepath\x18\x01 \x01(\t\x12\x18\n\x10\x64isable_manifest\x18\x05 \x01(\x08\x12\x1f\n\x02s3\x18\x02 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x03 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x04 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x12\'\n\x06\x61liOSS\x18\x06 \x01(\x0b\x32\x15.livekit.AliOSSUploadH\x00\x42\x08\n\x06output"\xef\x01\n\x08S3Upload\x12\x12\n\naccess_key\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\x0e\n\x06region\x18\x03 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x04 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x05 \x01(\t\x12\x18\n\x10\x66orce_path_style\x18\x06 \x01(\x08\x12\x31\n\x08metadata\x18\x07 \x03(\x0b\x32\x1f.livekit.S3Upload.MetadataEntry\x12\x0f\n\x07tagging\x18\x08 \x01(\t\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01"0\n\tGCPUpload\x12\x13\n\x0b\x63redentials\x18\x01 \x01(\x0c\x12\x0e\n\x06\x62ucket\x18\x02 \x01(\t"T\n\x0f\x41zureBlobUpload\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63\x63ount_key\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_name\x18\x03 \x01(\t"d\n\x0c\x41liOSSUpload\x12\x12\n\naccess_key\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\x0e\n\x06region\x18\x03 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x04 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x05 \x01(\t"G\n\x0cStreamOutput\x12)\n\x08protocol\x18\x01 \x01(\x0e\x32\x17.livekit.StreamProtocol\x12\x0c\n\x04urls\x18\x02 \x03(\t"\xed\x01\n\x0f\x45ncodingOptions\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\r\n\x05\x64\x65pth\x18\x03 \x01(\x05\x12\x11\n\tframerate\x18\x04 \x01(\x05\x12(\n\x0b\x61udio_codec\x18\x05 \x01(\x0e\x32\x13.livekit.AudioCodec\x12\x15\n\raudio_bitrate\x18\x06 \x01(\x05\x12\x17\n\x0f\x61udio_frequency\x18\x07 \x01(\x05\x12(\n\x0bvideo_codec\x18\x08 \x01(\x0e\x32\x13.livekit.VideoCodec\x12\x15\n\rvideo_bitrate\x18\t \x01(\x05"8\n\x13UpdateLayoutRequest\x12\x11\n\tegress_id\x18\x01 \x01(\t\x12\x0e\n\x06layout\x18\x02 \x01(\t"]\n\x13UpdateStreamRequest\x12\x11\n\tegress_id\x18\x01 \x01(\t\x12\x17\n\x0f\x61\x64\x64_output_urls\x18\x02 \x03(\t\x12\x1a\n\x12remove_output_urls\x18\x03 \x03(\t"&\n\x11ListEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t"8\n\x12ListEgressResponse\x12"\n\x05items\x18\x01 \x03(\x0b\x32\x13.livekit.EgressInfo"&\n\x11StopEgressRequest\x12\x11\n\tegress_id\x18\x01 \x01(\t"\x85\x04\n\nEgressInfo\x12\x11\n\tegress_id\x18\x01 \x01(\t\x12\x0f\n\x07room_id\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\r \x01(\t\x12%\n\x06status\x18\x03 \x01(\x0e\x32\x15.livekit.EgressStatus\x12\x12\n\nstarted_at\x18\n \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x0b \x01(\x03\x12\r\n\x05\x65rror\x18\t \x01(\t\x12=\n\x0eroom_composite\x18\x04 \x01(\x0b\x32#.livekit.RoomCompositeEgressRequestH\x00\x12?\n\x0ftrack_composite\x18\x05 \x01(\x0b\x32$.livekit.TrackCompositeEgressRequestH\x00\x12,\n\x05track\x18\x06 \x01(\x0b\x32\x1b.livekit.TrackEgressRequestH\x00\x12(\n\x03web\x18\x0e \x01(\x0b\x32\x19.livekit.WebEgressRequestH\x00\x12)\n\x06stream\x18\x07 \x01(\x0b\x32\x17.livekit.StreamInfoListH\x01\x12!\n\x04\x66ile\x18\x08 \x01(\x0b\x32\x11.livekit.FileInfoH\x01\x12)\n\x08segments\x18\x0c \x01(\x0b\x32\x15.livekit.SegmentsInfoH\x01\x42\t\n\x07requestB\x08\n\x06result"3\n\x0eStreamInfoList\x12!\n\x04info\x18\x01 \x03(\x0b\x32\x13.livekit.StreamInfo"\xad\x01\n\nStreamInfo\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\nstarted_at\x18\x02 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x03 \x01(\x03\x12\x10\n\x08\x64uration\x18\x04 \x01(\x03\x12*\n\x06status\x18\x05 \x01(\x0e\x32\x1a.livekit.StreamInfo.Status".\n\x06Status\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08\x46INISHED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02"t\n\x08\x46ileInfo\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x12\x12\n\nstarted_at\x18\x02 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x03 \x01(\x03\x12\x10\n\x08\x64uration\x18\x06 \x01(\x03\x12\x0c\n\x04size\x18\x04 \x01(\x03\x12\x10\n\x08location\x18\x05 \x01(\t"\x9d\x01\n\x0cSegmentsInfo\x12\x15\n\rplaylist_name\x18\x01 \x01(\t\x12\x10\n\x08\x64uration\x18\x02 \x01(\x03\x12\x0c\n\x04size\x18\x03 \x01(\x03\x12\x19\n\x11playlist_location\x18\x04 \x01(\t\x12\x15\n\rsegment_count\x18\x05 \x01(\x03\x12\x12\n\nstarted_at\x18\x06 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x07 \x01(\x03"\xb6\x01\n\x0f\x41utoTrackEgress\x12\x10\n\x08\x66ilepath\x18\x01 \x01(\t\x12\x18\n\x10\x64isable_manifest\x18\x05 \x01(\x08\x12\x1f\n\x02s3\x18\x02 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x03 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x04 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x42\x08\n\x06output*9\n\x0f\x45ncodedFileType\x12\x14\n\x10\x44\x45\x46\x41ULT_FILETYPE\x10\x00\x12\x07\n\x03MP4\x10\x01\x12\x07\n\x03OGG\x10\x02*0\n\x0eStreamProtocol\x12\x14\n\x10\x44\x45\x46\x41ULT_PROTOCOL\x10\x00\x12\x08\n\x04RTMP\x10\x01*N\n\x15SegmentedFileProtocol\x12#\n\x1f\x44\x45\x46\x41ULT_SEGMENTED_FILE_PROTOCOL\x10\x00\x12\x10\n\x0cHLS_PROTOCOL\x10\x01*/\n\nAudioCodec\x12\x0e\n\nDEFAULT_AC\x10\x00\x12\x08\n\x04OPUS\x10\x01\x12\x07\n\x03\x41\x41\x43\x10\x02*M\n\nVideoCodec\x12\x0e\n\nDEFAULT_VC\x10\x00\x12\x11\n\rH264_BASELINE\x10\x01\x12\r\n\tH264_MAIN\x10\x02\x12\r\n\tH264_HIGH\x10\x03*\xcf\x01\n\x15\x45ncodingOptionsPreset\x12\x10\n\x0cH264_720P_30\x10\x00\x12\x10\n\x0cH264_720P_60\x10\x01\x12\x11\n\rH264_1080P_30\x10\x02\x12\x11\n\rH264_1080P_60\x10\x03\x12\x19\n\x15PORTRAIT_H264_720P_30\x10\x04\x12\x19\n\x15PORTRAIT_H264_720P_60\x10\x05\x12\x1a\n\x16PORTRAIT_H264_1080P_30\x10\x06\x12\x1a\n\x16PORTRAIT_H264_1080P_60\x10\x07*\x9f\x01\n\x0c\x45gressStatus\x12\x13\n\x0f\x45GRESS_STARTING\x10\x00\x12\x11\n\rEGRESS_ACTIVE\x10\x01\x12\x11\n\rEGRESS_ENDING\x10\x02\x12\x13\n\x0f\x45GRESS_COMPLETE\x10\x03\x12\x11\n\rEGRESS_FAILED\x10\x04\x12\x12\n\x0e\x45GRESS_ABORTED\x10\x05\x12\x18\n\x14\x45GRESS_LIMIT_REACHED\x10\x06\x32\xca\x04\n\x06\x45gress\x12T\n\x18StartRoomCompositeEgress\x12#.livekit.RoomCompositeEgressRequest\x1a\x13.livekit.EgressInfo\x12V\n\x19StartTrackCompositeEgress\x12$.livekit.TrackCompositeEgressRequest\x1a\x13.livekit.EgressInfo\x12\x44\n\x10StartTrackEgress\x12\x1b.livekit.TrackEgressRequest\x1a\x13.livekit.EgressInfo\x12@\n\x0eStartWebEgress\x12\x19.livekit.WebEgressRequest\x1a\x13.livekit.EgressInfo\x12\x41\n\x0cUpdateLayout\x12\x1c.livekit.UpdateLayoutRequest\x1a\x13.livekit.EgressInfo\x12\x41\n\x0cUpdateStream\x12\x1c.livekit.UpdateStreamRequest\x1a\x13.livekit.EgressInfo\x12\x45\n\nListEgress\x12\x1a.livekit.ListEgressRequest\x1a\x1b.livekit.ListEgressResponse\x12=\n\nStopEgress\x12\x1a.livekit.StopEgressRequest\x1a\x13.livekit.EgressInfoBFZ#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
+    b'\n\x11livekit_rtc.proto\x12\x07livekit\x1a\x14livekit_models.proto"\xd5\x05\n\rSignalRequest\x12,\n\x05offer\x18\x01 \x01(\x0b\x32\x1b.livekit.SessionDescriptionH\x00\x12-\n\x06\x61nswer\x18\x02 \x01(\x0b\x32\x1b.livekit.SessionDescriptionH\x00\x12*\n\x07trickle\x18\x03 \x01(\x0b\x32\x17.livekit.TrickleRequestH\x00\x12-\n\tadd_track\x18\x04 \x01(\x0b\x32\x18.livekit.AddTrackRequestH\x00\x12)\n\x04mute\x18\x05 \x01(\x0b\x32\x19.livekit.MuteTrackRequestH\x00\x12\x33\n\x0csubscription\x18\x06 \x01(\x0b\x32\x1b.livekit.UpdateSubscriptionH\x00\x12\x35\n\rtrack_setting\x18\x07 \x01(\x0b\x32\x1c.livekit.UpdateTrackSettingsH\x00\x12&\n\x05leave\x18\x08 \x01(\x0b\x32\x15.livekit.LeaveRequestH\x00\x12\x33\n\rupdate_layers\x18\n \x01(\x0b\x32\x1a.livekit.UpdateVideoLayersH\x00\x12\x42\n\x17subscription_permission\x18\x0b \x01(\x0b\x32\x1f.livekit.SubscriptionPermissionH\x00\x12(\n\nsync_state\x18\x0c \x01(\x0b\x32\x12.livekit.SyncStateH\x00\x12-\n\x08simulate\x18\r \x01(\x0b\x32\x19.livekit.SimulateScenarioH\x00\x12\x0e\n\x04ping\x18\x0e \x01(\x03H\x00\x12=\n\x0fupdate_metadata\x18\x0f \x01(\x0b\x32".livekit.UpdateParticipantMetadataH\x00\x12!\n\x08ping_req\x18\x10 \x01(\x0b\x32\r.livekit.PingH\x00\x42\t\n\x07message"\xbb\x07\n\x0eSignalResponse\x12%\n\x04join\x18\x01 \x01(\x0b\x32\x15.livekit.JoinResponseH\x00\x12-\n\x06\x61nswer\x18\x02 \x01(\x0b\x32\x1b.livekit.SessionDescriptionH\x00\x12,\n\x05offer\x18\x03 \x01(\x0b\x32\x1b.livekit.SessionDescriptionH\x00\x12*\n\x07trickle\x18\x04 \x01(\x0b\x32\x17.livekit.TrickleRequestH\x00\x12,\n\x06update\x18\x05 \x01(\x0b\x32\x1a.livekit.ParticipantUpdateH\x00\x12:\n\x0ftrack_published\x18\x06 \x01(\x0b\x32\x1f.livekit.TrackPublishedResponseH\x00\x12&\n\x05leave\x18\x08 \x01(\x0b\x32\x15.livekit.LeaveRequestH\x00\x12)\n\x04mute\x18\t \x01(\x0b\x32\x19.livekit.MuteTrackRequestH\x00\x12\x34\n\x10speakers_changed\x18\n \x01(\x0b\x32\x18.livekit.SpeakersChangedH\x00\x12*\n\x0broom_update\x18\x0b \x01(\x0b\x32\x13.livekit.RoomUpdateH\x00\x12>\n\x12\x63onnection_quality\x18\x0c \x01(\x0b\x32 .livekit.ConnectionQualityUpdateH\x00\x12\x39\n\x13stream_state_update\x18\r \x01(\x0b\x32\x1a.livekit.StreamStateUpdateH\x00\x12\x45\n\x19subscribed_quality_update\x18\x0e \x01(\x0b\x32 .livekit.SubscribedQualityUpdateH\x00\x12O\n\x1esubscription_permission_update\x18\x0f \x01(\x0b\x32%.livekit.SubscriptionPermissionUpdateH\x00\x12\x17\n\rrefresh_token\x18\x10 \x01(\tH\x00\x12>\n\x11track_unpublished\x18\x11 \x01(\x0b\x32!.livekit.TrackUnpublishedResponseH\x00\x12\x0e\n\x04pong\x18\x12 \x01(\x03H\x00\x12/\n\treconnect\x18\x13 \x01(\x0b\x32\x1a.livekit.ReconnectResponseH\x00\x12"\n\tpong_resp\x18\x14 \x01(\x0b\x32\r.livekit.PongH\x00\x42\t\n\x07message"M\n\x0eSimulcastCodec\x12\r\n\x05\x63odec\x18\x01 \x01(\t\x12\x0b\n\x03\x63id\x18\x02 \x01(\t\x12\x1f\n\x17\x65nable_simulcast_layers\x18\x03 \x01(\x08"\xef\x02\n\x0f\x41\x64\x64TrackRequest\x12\x0b\n\x03\x63id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12 \n\x04type\x18\x03 \x01(\x0e\x32\x12.livekit.TrackType\x12\r\n\x05width\x18\x04 \x01(\r\x12\x0e\n\x06height\x18\x05 \x01(\r\x12\r\n\x05muted\x18\x06 \x01(\x08\x12\x13\n\x0b\x64isable_dtx\x18\x07 \x01(\x08\x12$\n\x06source\x18\x08 \x01(\x0e\x32\x14.livekit.TrackSource\x12#\n\x06layers\x18\t \x03(\x0b\x32\x13.livekit.VideoLayer\x12\x31\n\x10simulcast_codecs\x18\n \x03(\x0b\x32\x17.livekit.SimulcastCodec\x12\x0b\n\x03sid\x18\x0b \x01(\t\x12\x0e\n\x06stereo\x18\x0c \x01(\x08\x12\x13\n\x0b\x64isable_red\x18\r \x01(\x08\x12,\n\nencryption\x18\x0e \x01(\x0e\x32\x18.livekit.Encryption.Type"N\n\x0eTrickleRequest\x12\x15\n\rcandidateInit\x18\x01 \x01(\t\x12%\n\x06target\x18\x02 \x01(\x0e\x32\x15.livekit.SignalTarget".\n\x10MuteTrackRequest\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\r\n\x05muted\x18\x02 \x01(\x08"\xb0\x03\n\x0cJoinResponse\x12\x1b\n\x04room\x18\x01 \x01(\x0b\x32\r.livekit.Room\x12-\n\x0bparticipant\x18\x02 \x01(\x0b\x32\x18.livekit.ParticipantInfo\x12\x34\n\x12other_participants\x18\x03 \x03(\x0b\x32\x18.livekit.ParticipantInfo\x12\x16\n\x0eserver_version\x18\x04 \x01(\t\x12\'\n\x0bice_servers\x18\x05 \x03(\x0b\x32\x12.livekit.ICEServer\x12\x1a\n\x12subscriber_primary\x18\x06 \x01(\x08\x12\x17\n\x0f\x61lternative_url\x18\x07 \x01(\t\x12:\n\x14\x63lient_configuration\x18\x08 \x01(\x0b\x32\x1c.livekit.ClientConfiguration\x12\x15\n\rserver_region\x18\t \x01(\t\x12\x14\n\x0cping_timeout\x18\n \x01(\x05\x12\x15\n\rping_interval\x18\x0b \x01(\x05\x12(\n\x0bserver_info\x18\x0c \x01(\x0b\x32\x13.livekit.ServerInfo"x\n\x11ReconnectResponse\x12\'\n\x0bice_servers\x18\x01 \x03(\x0b\x32\x12.livekit.ICEServer\x12:\n\x14\x63lient_configuration\x18\x02 \x01(\x0b\x32\x1c.livekit.ClientConfiguration"H\n\x16TrackPublishedResponse\x12\x0b\n\x03\x63id\x18\x01 \x01(\t\x12!\n\x05track\x18\x02 \x01(\x0b\x32\x12.livekit.TrackInfo"-\n\x18TrackUnpublishedResponse\x12\x11\n\ttrack_sid\x18\x01 \x01(\t"/\n\x12SessionDescription\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0b\n\x03sdp\x18\x02 \x01(\t"C\n\x11ParticipantUpdate\x12.\n\x0cparticipants\x18\x01 \x03(\x0b\x32\x18.livekit.ParticipantInfo"s\n\x12UpdateSubscription\x12\x12\n\ntrack_sids\x18\x01 \x03(\t\x12\x11\n\tsubscribe\x18\x02 \x01(\x08\x12\x36\n\x12participant_tracks\x18\x03 \x03(\x0b\x32\x1a.livekit.ParticipantTracks"\xa1\x01\n\x13UpdateTrackSettings\x12\x12\n\ntrack_sids\x18\x01 \x03(\t\x12\x10\n\x08\x64isabled\x18\x03 \x01(\x08\x12&\n\x07quality\x18\x04 \x01(\x0e\x32\x15.livekit.VideoQuality\x12\r\n\x05width\x18\x05 \x01(\r\x12\x0e\n\x06height\x18\x06 \x01(\r\x12\x0b\n\x03\x66ps\x18\x07 \x01(\r\x12\x10\n\x08priority\x18\x08 \x01(\r"P\n\x0cLeaveRequest\x12\x15\n\rcan_reconnect\x18\x01 \x01(\x08\x12)\n\x06reason\x18\x02 \x01(\x0e\x32\x19.livekit.DisconnectReason"K\n\x11UpdateVideoLayers\x12\x11\n\ttrack_sid\x18\x01 \x01(\t\x12#\n\x06layers\x18\x02 \x03(\x0b\x32\x13.livekit.VideoLayer";\n\x19UpdateParticipantMetadata\x12\x10\n\x08metadata\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t"?\n\tICEServer\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x12\n\ncredential\x18\x03 \x01(\t"9\n\x0fSpeakersChanged\x12&\n\x08speakers\x18\x01 \x03(\x0b\x32\x14.livekit.SpeakerInfo")\n\nRoomUpdate\x12\x1b\n\x04room\x18\x01 \x01(\x0b\x32\r.livekit.Room"l\n\x15\x43onnectionQualityInfo\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12+\n\x07quality\x18\x02 \x01(\x0e\x32\x1a.livekit.ConnectionQuality\x12\r\n\x05score\x18\x03 \x01(\x02"J\n\x17\x43onnectionQualityUpdate\x12/\n\x07updates\x18\x01 \x03(\x0b\x32\x1e.livekit.ConnectionQualityInfo"b\n\x0fStreamStateInfo\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12\x11\n\ttrack_sid\x18\x02 \x01(\t\x12#\n\x05state\x18\x03 \x01(\x0e\x32\x14.livekit.StreamState"D\n\x11StreamStateUpdate\x12/\n\rstream_states\x18\x01 \x03(\x0b\x32\x18.livekit.StreamStateInfo"L\n\x11SubscribedQuality\x12&\n\x07quality\x18\x01 \x01(\x0e\x32\x15.livekit.VideoQuality\x12\x0f\n\x07\x65nabled\x18\x02 \x01(\x08"O\n\x0fSubscribedCodec\x12\r\n\x05\x63odec\x18\x01 \x01(\t\x12-\n\tqualities\x18\x02 \x03(\x0b\x32\x1a.livekit.SubscribedQuality"\x9b\x01\n\x17SubscribedQualityUpdate\x12\x11\n\ttrack_sid\x18\x01 \x01(\t\x12\x38\n\x14subscribed_qualities\x18\x02 \x03(\x0b\x32\x1a.livekit.SubscribedQuality\x12\x33\n\x11subscribed_codecs\x18\x03 \x03(\x0b\x32\x18.livekit.SubscribedCodec"p\n\x0fTrackPermission\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12\x12\n\nall_tracks\x18\x02 \x01(\x08\x12\x12\n\ntrack_sids\x18\x03 \x03(\t\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t"g\n\x16SubscriptionPermission\x12\x18\n\x10\x61ll_participants\x18\x01 \x01(\x08\x12\x33\n\x11track_permissions\x18\x02 \x03(\x0b\x32\x18.livekit.TrackPermission"[\n\x1cSubscriptionPermissionUpdate\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12\x11\n\ttrack_sid\x18\x02 \x01(\t\x12\x0f\n\x07\x61llowed\x18\x03 \x01(\x08"\x81\x02\n\tSyncState\x12+\n\x06\x61nswer\x18\x01 \x01(\x0b\x32\x1b.livekit.SessionDescription\x12\x31\n\x0csubscription\x18\x02 \x01(\x0b\x32\x1b.livekit.UpdateSubscription\x12\x37\n\x0epublish_tracks\x18\x03 \x03(\x0b\x32\x1f.livekit.TrackPublishedResponse\x12/\n\rdata_channels\x18\x04 \x03(\x0b\x32\x18.livekit.DataChannelInfo\x12*\n\x05offer\x18\x05 \x01(\x0b\x32\x1b.livekit.SessionDescription"S\n\x0f\x44\x61taChannelInfo\x12\r\n\x05label\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\r\x12%\n\x06target\x18\x03 \x01(\x0e\x32\x15.livekit.SignalTarget"\xde\x01\n\x10SimulateScenario\x12\x18\n\x0espeaker_update\x18\x01 \x01(\x05H\x00\x12\x16\n\x0cnode_failure\x18\x02 \x01(\x08H\x00\x12\x13\n\tmigration\x18\x03 \x01(\x08H\x00\x12\x16\n\x0cserver_leave\x18\x04 \x01(\x08H\x00\x12?\n\x19switch_candidate_protocol\x18\x05 \x01(\x0e\x32\x1a.livekit.CandidateProtocolH\x00\x12\x1e\n\x14subscriber_bandwidth\x18\x06 \x01(\x03H\x00\x42\n\n\x08scenario"&\n\x04Ping\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\x12\x0b\n\x03rtt\x18\x02 \x01(\x03"6\n\x04Pong\x12\x1b\n\x13last_ping_timestamp\x18\x01 \x01(\x03\x12\x11\n\ttimestamp\x18\x02 \x01(\x03"6\n\x0eRegionSettings\x12$\n\x07regions\x18\x01 \x03(\x0b\x32\x13.livekit.RegionInfo";\n\nRegionInfo\x12\x0e\n\x06region\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12\x10\n\x08\x64istance\x18\x03 \x01(\x03*-\n\x0cSignalTarget\x12\r\n\tPUBLISHER\x10\x00\x12\x0e\n\nSUBSCRIBER\x10\x01*%\n\x0bStreamState\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\n\n\x06PAUSED\x10\x01*.\n\x11\x43\x61ndidateProtocol\x12\x07\n\x03UDP\x10\x00\x12\x07\n\x03TCP\x10\x01\x12\x07\n\x03TLS\x10\x02\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "livekit_egress_pb2", globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "livekit_rtc_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto"
-    _S3UPLOAD_METADATAENTRY._options = None
-    _S3UPLOAD_METADATAENTRY._serialized_options = b"8\001"
-    _ENCODEDFILETYPE._serialized_start = 4363
-    _ENCODEDFILETYPE._serialized_end = 4420
-    _STREAMPROTOCOL._serialized_start = 4422
-    _STREAMPROTOCOL._serialized_end = 4470
-    _SEGMENTEDFILEPROTOCOL._serialized_start = 4472
-    _SEGMENTEDFILEPROTOCOL._serialized_end = 4550
-    _AUDIOCODEC._serialized_start = 4552
-    _AUDIOCODEC._serialized_end = 4599
-    _VIDEOCODEC._serialized_start = 4601
-    _VIDEOCODEC._serialized_end = 4678
-    _ENCODINGOPTIONSPRESET._serialized_start = 4681
-    _ENCODINGOPTIONSPRESET._serialized_end = 4888
-    _EGRESSSTATUS._serialized_start = 4891
-    _EGRESSSTATUS._serialized_end = 5050
-    _ROOMCOMPOSITEEGRESSREQUEST._serialized_start = 34
-    _ROOMCOMPOSITEEGRESSREQUEST._serialized_end = 414
-    _TRACKCOMPOSITEEGRESSREQUEST._serialized_start = 417
-    _TRACKCOMPOSITEEGRESSREQUEST._serialized_end = 765
-    _TRACKEGRESSREQUEST._serialized_start = 768
-    _TRACKEGRESSREQUEST._serialized_end = 903
-    _WEBEGRESSREQUEST._serialized_start = 906
-    _WEBEGRESSREQUEST._serialized_end = 1229
-    _ENCODEDFILEOUTPUT._serialized_start = 1232
-    _ENCODEDFILEOUTPUT._serialized_end = 1502
-    _SEGMENTEDFILEOUTPUT._serialized_start = 1505
-    _SEGMENTEDFILEOUTPUT._serialized_end = 1838
-    _DIRECTFILEOUTPUT._serialized_start = 1841
-    _DIRECTFILEOUTPUT._serialized_end = 2065
-    _S3UPLOAD._serialized_start = 2068
-    _S3UPLOAD._serialized_end = 2307
-    _S3UPLOAD_METADATAENTRY._serialized_start = 2260
-    _S3UPLOAD_METADATAENTRY._serialized_end = 2307
-    _GCPUPLOAD._serialized_start = 2309
-    _GCPUPLOAD._serialized_end = 2357
-    _AZUREBLOBUPLOAD._serialized_start = 2359
-    _AZUREBLOBUPLOAD._serialized_end = 2443
-    _ALIOSSUPLOAD._serialized_start = 2445
-    _ALIOSSUPLOAD._serialized_end = 2545
-    _STREAMOUTPUT._serialized_start = 2547
-    _STREAMOUTPUT._serialized_end = 2618
-    _ENCODINGOPTIONS._serialized_start = 2621
-    _ENCODINGOPTIONS._serialized_end = 2858
-    _UPDATELAYOUTREQUEST._serialized_start = 2860
-    _UPDATELAYOUTREQUEST._serialized_end = 2916
-    _UPDATESTREAMREQUEST._serialized_start = 2918
-    _UPDATESTREAMREQUEST._serialized_end = 3011
-    _LISTEGRESSREQUEST._serialized_start = 3013
-    _LISTEGRESSREQUEST._serialized_end = 3051
-    _LISTEGRESSRESPONSE._serialized_start = 3053
-    _LISTEGRESSRESPONSE._serialized_end = 3109
-    _STOPEGRESSREQUEST._serialized_start = 3111
-    _STOPEGRESSREQUEST._serialized_end = 3149
-    _EGRESSINFO._serialized_start = 3152
-    _EGRESSINFO._serialized_end = 3669
-    _STREAMINFOLIST._serialized_start = 3671
-    _STREAMINFOLIST._serialized_end = 3722
-    _STREAMINFO._serialized_start = 3725
-    _STREAMINFO._serialized_end = 3898
-    _STREAMINFO_STATUS._serialized_start = 3852
-    _STREAMINFO_STATUS._serialized_end = 3898
-    _FILEINFO._serialized_start = 3900
-    _FILEINFO._serialized_end = 4016
-    _SEGMENTSINFO._serialized_start = 4019
-    _SEGMENTSINFO._serialized_end = 4176
-    _AUTOTRACKEGRESS._serialized_start = 4179
-    _AUTOTRACKEGRESS._serialized_end = 4361
-    _EGRESS._serialized_start = 5053
-    _EGRESS._serialized_end = 5639
+    _SIGNALTARGET._serialized_start = 5547
+    _SIGNALTARGET._serialized_end = 5592
+    _STREAMSTATE._serialized_start = 5594
+    _STREAMSTATE._serialized_end = 5631
+    _CANDIDATEPROTOCOL._serialized_start = 5633
+    _CANDIDATEPROTOCOL._serialized_end = 5679
+    _SIGNALREQUEST._serialized_start = 53
+    _SIGNALREQUEST._serialized_end = 778
+    _SIGNALRESPONSE._serialized_start = 781
+    _SIGNALRESPONSE._serialized_end = 1736
+    _SIMULCASTCODEC._serialized_start = 1738
+    _SIMULCASTCODEC._serialized_end = 1815
+    _ADDTRACKREQUEST._serialized_start = 1818
+    _ADDTRACKREQUEST._serialized_end = 2185
+    _TRICKLEREQUEST._serialized_start = 2187
+    _TRICKLEREQUEST._serialized_end = 2265
+    _MUTETRACKREQUEST._serialized_start = 2267
+    _MUTETRACKREQUEST._serialized_end = 2313
+    _JOINRESPONSE._serialized_start = 2316
+    _JOINRESPONSE._serialized_end = 2748
+    _RECONNECTRESPONSE._serialized_start = 2750
+    _RECONNECTRESPONSE._serialized_end = 2870
+    _TRACKPUBLISHEDRESPONSE._serialized_start = 2872
+    _TRACKPUBLISHEDRESPONSE._serialized_end = 2944
+    _TRACKUNPUBLISHEDRESPONSE._serialized_start = 2946
+    _TRACKUNPUBLISHEDRESPONSE._serialized_end = 2991
+    _SESSIONDESCRIPTION._serialized_start = 2993
+    _SESSIONDESCRIPTION._serialized_end = 3040
+    _PARTICIPANTUPDATE._serialized_start = 3042
+    _PARTICIPANTUPDATE._serialized_end = 3109
+    _UPDATESUBSCRIPTION._serialized_start = 3111
+    _UPDATESUBSCRIPTION._serialized_end = 3226
+    _UPDATETRACKSETTINGS._serialized_start = 3229
+    _UPDATETRACKSETTINGS._serialized_end = 3390
+    _LEAVEREQUEST._serialized_start = 3392
+    _LEAVEREQUEST._serialized_end = 3472
+    _UPDATEVIDEOLAYERS._serialized_start = 3474
+    _UPDATEVIDEOLAYERS._serialized_end = 3549
+    _UPDATEPARTICIPANTMETADATA._serialized_start = 3551
+    _UPDATEPARTICIPANTMETADATA._serialized_end = 3610
+    _ICESERVER._serialized_start = 3612
+    _ICESERVER._serialized_end = 3675
+    _SPEAKERSCHANGED._serialized_start = 3677
+    _SPEAKERSCHANGED._serialized_end = 3734
+    _ROOMUPDATE._serialized_start = 3736
+    _ROOMUPDATE._serialized_end = 3777
+    _CONNECTIONQUALITYINFO._serialized_start = 3779
+    _CONNECTIONQUALITYINFO._serialized_end = 3887
+    _CONNECTIONQUALITYUPDATE._serialized_start = 3889
+    _CONNECTIONQUALITYUPDATE._serialized_end = 3963
+    _STREAMSTATEINFO._serialized_start = 3965
+    _STREAMSTATEINFO._serialized_end = 4063
+    _STREAMSTATEUPDATE._serialized_start = 4065
+    _STREAMSTATEUPDATE._serialized_end = 4133
+    _SUBSCRIBEDQUALITY._serialized_start = 4135
+    _SUBSCRIBEDQUALITY._serialized_end = 4211
+    _SUBSCRIBEDCODEC._serialized_start = 4213
+    _SUBSCRIBEDCODEC._serialized_end = 4292
+    _SUBSCRIBEDQUALITYUPDATE._serialized_start = 4295
+    _SUBSCRIBEDQUALITYUPDATE._serialized_end = 4450
+    _TRACKPERMISSION._serialized_start = 4452
+    _TRACKPERMISSION._serialized_end = 4564
+    _SUBSCRIPTIONPERMISSION._serialized_start = 4566
+    _SUBSCRIPTIONPERMISSION._serialized_end = 4669
+    _SUBSCRIPTIONPERMISSIONUPDATE._serialized_start = 4671
+    _SUBSCRIPTIONPERMISSIONUPDATE._serialized_end = 4762
+    _SYNCSTATE._serialized_start = 4765
+    _SYNCSTATE._serialized_end = 5022
+    _DATACHANNELINFO._serialized_start = 5024
+    _DATACHANNELINFO._serialized_end = 5107
+    _SIMULATESCENARIO._serialized_start = 5110
+    _SIMULATESCENARIO._serialized_end = 5332
+    _PING._serialized_start = 5334
+    _PING._serialized_end = 5372
+    _PONG._serialized_start = 5374
+    _PONG._serialized_end = 5428
+    _REGIONSETTINGS._serialized_start = 5430
+    _REGIONSETTINGS._serialized_end = 5484
+    _REGIONINFO._serialized_start = 5486
+    _REGIONINFO._serialized_end = 5545
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_egress_pb2.pyi` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_egress_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 from typing import ClassVar as _ClassVar
 from typing import Iterable as _Iterable
 from typing import Mapping as _Mapping
 from typing import Optional as _Optional
 from typing import Union as _Union
 
+import livekit_models_pb2 as _livekit_models_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 
-AAC: AudioCodec
-DEFAULT_AC: AudioCodec
 DEFAULT_FILETYPE: EncodedFileType
 DEFAULT_PROTOCOL: StreamProtocol
 DEFAULT_SEGMENTED_FILE_PROTOCOL: SegmentedFileProtocol
-DEFAULT_VC: VideoCodec
 DESCRIPTOR: _descriptor.FileDescriptor
 EGRESS_ABORTED: EgressStatus
 EGRESS_ACTIVE: EgressStatus
 EGRESS_COMPLETE: EgressStatus
 EGRESS_ENDING: EgressStatus
 EGRESS_FAILED: EgressStatus
 EGRESS_LIMIT_REACHED: EgressStatus
 EGRESS_STARTING: EgressStatus
 H264_1080P_30: EncodingOptionsPreset
 H264_1080P_60: EncodingOptionsPreset
 H264_720P_30: EncodingOptionsPreset
 H264_720P_60: EncodingOptionsPreset
-H264_BASELINE: VideoCodec
-H264_HIGH: VideoCodec
-H264_MAIN: VideoCodec
 HLS_PROTOCOL: SegmentedFileProtocol
+INDEX: SegmentedFileSuffix
 MP4: EncodedFileType
 OGG: EncodedFileType
-OPUS: AudioCodec
 PORTRAIT_H264_1080P_30: EncodingOptionsPreset
 PORTRAIT_H264_1080P_60: EncodingOptionsPreset
 PORTRAIT_H264_720P_30: EncodingOptionsPreset
 PORTRAIT_H264_720P_60: EncodingOptionsPreset
 RTMP: StreamProtocol
+TIMESTAMP: SegmentedFileSuffix
 
 class AliOSSUpload(_message.Message):
     __slots__ = ["access_key", "bucket", "endpoint", "region", "secret"]
     ACCESS_KEY_FIELD_NUMBER: _ClassVar[int]
     BUCKET_FIELD_NUMBER: _ClassVar[int]
     ENDPOINT_FIELD_NUMBER: _ClassVar[int]
     REGION_FIELD_NUMBER: _ClassVar[int]
@@ -123,50 +119,59 @@
 
 class EgressInfo(_message.Message):
     __slots__ = [
         "egress_id",
         "ended_at",
         "error",
         "file",
+        "file_results",
         "room_composite",
         "room_id",
         "room_name",
+        "segment_results",
         "segments",
         "started_at",
         "status",
         "stream",
+        "stream_results",
         "track",
         "track_composite",
         "web",
     ]
     EGRESS_ID_FIELD_NUMBER: _ClassVar[int]
     ENDED_AT_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
     FILE_FIELD_NUMBER: _ClassVar[int]
+    FILE_RESULTS_FIELD_NUMBER: _ClassVar[int]
     ROOM_COMPOSITE_FIELD_NUMBER: _ClassVar[int]
     ROOM_ID_FIELD_NUMBER: _ClassVar[int]
     ROOM_NAME_FIELD_NUMBER: _ClassVar[int]
     SEGMENTS_FIELD_NUMBER: _ClassVar[int]
+    SEGMENT_RESULTS_FIELD_NUMBER: _ClassVar[int]
     STARTED_AT_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     STREAM_FIELD_NUMBER: _ClassVar[int]
+    STREAM_RESULTS_FIELD_NUMBER: _ClassVar[int]
     TRACK_COMPOSITE_FIELD_NUMBER: _ClassVar[int]
     TRACK_FIELD_NUMBER: _ClassVar[int]
     WEB_FIELD_NUMBER: _ClassVar[int]
     egress_id: str
     ended_at: int
     error: str
     file: FileInfo
+    file_results: _containers.RepeatedCompositeFieldContainer[FileInfo]
     room_composite: RoomCompositeEgressRequest
     room_id: str
     room_name: str
+    segment_results: _containers.RepeatedCompositeFieldContainer[SegmentsInfo]
     segments: SegmentsInfo
     started_at: int
     status: EgressStatus
     stream: StreamInfoList
+    stream_results: _containers.RepeatedCompositeFieldContainer[StreamInfo]
     track: TrackEgressRequest
     track_composite: TrackCompositeEgressRequest
     web: WebEgressRequest
     def __init__(
         self,
         egress_id: _Optional[str] = ...,
         room_id: _Optional[str] = ...,
@@ -178,14 +183,17 @@
         room_composite: _Optional[_Union[RoomCompositeEgressRequest, _Mapping]] = ...,
         track_composite: _Optional[_Union[TrackCompositeEgressRequest, _Mapping]] = ...,
         track: _Optional[_Union[TrackEgressRequest, _Mapping]] = ...,
         web: _Optional[_Union[WebEgressRequest, _Mapping]] = ...,
         stream: _Optional[_Union[StreamInfoList, _Mapping]] = ...,
         file: _Optional[_Union[FileInfo, _Mapping]] = ...,
         segments: _Optional[_Union[SegmentsInfo, _Mapping]] = ...,
+        stream_results: _Optional[_Iterable[_Union[StreamInfo, _Mapping]]] = ...,
+        file_results: _Optional[_Iterable[_Union[FileInfo, _Mapping]]] = ...,
+        segment_results: _Optional[_Iterable[_Union[SegmentsInfo, _Mapping]]] = ...,
     ) -> None: ...
 
 class EncodedFileOutput(_message.Message):
     __slots__ = [
         "aliOSS",
         "azure",
         "disable_manifest",
@@ -223,47 +231,51 @@
     __slots__ = [
         "audio_bitrate",
         "audio_codec",
         "audio_frequency",
         "depth",
         "framerate",
         "height",
+        "key_frame_interval",
         "video_bitrate",
         "video_codec",
         "width",
     ]
     AUDIO_BITRATE_FIELD_NUMBER: _ClassVar[int]
     AUDIO_CODEC_FIELD_NUMBER: _ClassVar[int]
     AUDIO_FREQUENCY_FIELD_NUMBER: _ClassVar[int]
     DEPTH_FIELD_NUMBER: _ClassVar[int]
     FRAMERATE_FIELD_NUMBER: _ClassVar[int]
     HEIGHT_FIELD_NUMBER: _ClassVar[int]
+    KEY_FRAME_INTERVAL_FIELD_NUMBER: _ClassVar[int]
     VIDEO_BITRATE_FIELD_NUMBER: _ClassVar[int]
     VIDEO_CODEC_FIELD_NUMBER: _ClassVar[int]
     WIDTH_FIELD_NUMBER: _ClassVar[int]
     audio_bitrate: int
-    audio_codec: AudioCodec
+    audio_codec: _livekit_models_pb2.AudioCodec
     audio_frequency: int
     depth: int
     framerate: int
     height: int
+    key_frame_interval: float
     video_bitrate: int
-    video_codec: VideoCodec
+    video_codec: _livekit_models_pb2.VideoCodec
     width: int
     def __init__(
         self,
         width: _Optional[int] = ...,
         height: _Optional[int] = ...,
         depth: _Optional[int] = ...,
         framerate: _Optional[int] = ...,
-        audio_codec: _Optional[_Union[AudioCodec, str]] = ...,
+        audio_codec: _Optional[_Union[_livekit_models_pb2.AudioCodec, str]] = ...,
         audio_bitrate: _Optional[int] = ...,
         audio_frequency: _Optional[int] = ...,
-        video_codec: _Optional[_Union[VideoCodec, str]] = ...,
+        video_codec: _Optional[_Union[_livekit_models_pb2.VideoCodec, str]] = ...,
         video_bitrate: _Optional[int] = ...,
+        key_frame_interval: _Optional[float] = ...,
     ) -> None: ...
 
 class FileInfo(_message.Message):
     __slots__ = ["duration", "ended_at", "filename", "location", "size", "started_at"]
     DURATION_FIELD_NUMBER: _ClassVar[int]
     ENDED_AT_FIELD_NUMBER: _ClassVar[int]
     FILENAME_FIELD_NUMBER: _ClassVar[int]
@@ -287,24 +299,33 @@
     ) -> None: ...
 
 class GCPUpload(_message.Message):
     __slots__ = ["bucket", "credentials"]
     BUCKET_FIELD_NUMBER: _ClassVar[int]
     CREDENTIALS_FIELD_NUMBER: _ClassVar[int]
     bucket: str
-    credentials: bytes
+    credentials: str
     def __init__(
-        self, credentials: _Optional[bytes] = ..., bucket: _Optional[str] = ...
+        self, credentials: _Optional[str] = ..., bucket: _Optional[str] = ...
     ) -> None: ...
 
 class ListEgressRequest(_message.Message):
-    __slots__ = ["room_name"]
+    __slots__ = ["active", "egress_id", "room_name"]
+    ACTIVE_FIELD_NUMBER: _ClassVar[int]
+    EGRESS_ID_FIELD_NUMBER: _ClassVar[int]
     ROOM_NAME_FIELD_NUMBER: _ClassVar[int]
+    active: bool
+    egress_id: str
     room_name: str
-    def __init__(self, room_name: _Optional[str] = ...) -> None: ...
+    def __init__(
+        self,
+        room_name: _Optional[str] = ...,
+        egress_id: _Optional[str] = ...,
+        active: bool = ...,
+    ) -> None: ...
 
 class ListEgressResponse(_message.Message):
     __slots__ = ["items"]
     ITEMS_FIELD_NUMBER: _ClassVar[int]
     items: _containers.RepeatedCompositeFieldContainer[EgressInfo]
     def __init__(
         self, items: _Optional[_Iterable[_Union[EgressInfo, _Mapping]]] = ...
@@ -312,53 +333,67 @@
 
 class RoomCompositeEgressRequest(_message.Message):
     __slots__ = [
         "advanced",
         "audio_only",
         "custom_base_url",
         "file",
+        "file_outputs",
         "layout",
         "preset",
         "room_name",
+        "segment_outputs",
         "segments",
         "stream",
+        "stream_outputs",
         "video_only",
     ]
     ADVANCED_FIELD_NUMBER: _ClassVar[int]
     AUDIO_ONLY_FIELD_NUMBER: _ClassVar[int]
     CUSTOM_BASE_URL_FIELD_NUMBER: _ClassVar[int]
     FILE_FIELD_NUMBER: _ClassVar[int]
+    FILE_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
     LAYOUT_FIELD_NUMBER: _ClassVar[int]
     PRESET_FIELD_NUMBER: _ClassVar[int]
     ROOM_NAME_FIELD_NUMBER: _ClassVar[int]
     SEGMENTS_FIELD_NUMBER: _ClassVar[int]
+    SEGMENT_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
     STREAM_FIELD_NUMBER: _ClassVar[int]
+    STREAM_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
     VIDEO_ONLY_FIELD_NUMBER: _ClassVar[int]
     advanced: EncodingOptions
     audio_only: bool
     custom_base_url: str
     file: EncodedFileOutput
+    file_outputs: _containers.RepeatedCompositeFieldContainer[EncodedFileOutput]
     layout: str
     preset: EncodingOptionsPreset
     room_name: str
+    segment_outputs: _containers.RepeatedCompositeFieldContainer[SegmentedFileOutput]
     segments: SegmentedFileOutput
     stream: StreamOutput
+    stream_outputs: _containers.RepeatedCompositeFieldContainer[StreamOutput]
     video_only: bool
     def __init__(
         self,
         room_name: _Optional[str] = ...,
         layout: _Optional[str] = ...,
         audio_only: bool = ...,
         video_only: bool = ...,
         custom_base_url: _Optional[str] = ...,
         file: _Optional[_Union[EncodedFileOutput, _Mapping]] = ...,
         stream: _Optional[_Union[StreamOutput, _Mapping]] = ...,
         segments: _Optional[_Union[SegmentedFileOutput, _Mapping]] = ...,
         preset: _Optional[_Union[EncodingOptionsPreset, str]] = ...,
         advanced: _Optional[_Union[EncodingOptions, _Mapping]] = ...,
+        file_outputs: _Optional[_Iterable[_Union[EncodedFileOutput, _Mapping]]] = ...,
+        stream_outputs: _Optional[_Iterable[_Union[StreamOutput, _Mapping]]] = ...,
+        segment_outputs: _Optional[
+            _Iterable[_Union[SegmentedFileOutput, _Mapping]]
+        ] = ...,
     ) -> None: ...
 
 class S3Upload(_message.Message):
     __slots__ = [
         "access_key",
         "bucket",
         "endpoint",
@@ -408,44 +443,48 @@
 
 class SegmentedFileOutput(_message.Message):
     __slots__ = [
         "aliOSS",
         "azure",
         "disable_manifest",
         "filename_prefix",
+        "filename_suffix",
         "gcp",
         "playlist_name",
         "protocol",
         "s3",
         "segment_duration",
     ]
     ALIOSS_FIELD_NUMBER: _ClassVar[int]
     AZURE_FIELD_NUMBER: _ClassVar[int]
     DISABLE_MANIFEST_FIELD_NUMBER: _ClassVar[int]
     FILENAME_PREFIX_FIELD_NUMBER: _ClassVar[int]
+    FILENAME_SUFFIX_FIELD_NUMBER: _ClassVar[int]
     GCP_FIELD_NUMBER: _ClassVar[int]
     PLAYLIST_NAME_FIELD_NUMBER: _ClassVar[int]
     PROTOCOL_FIELD_NUMBER: _ClassVar[int]
     S3_FIELD_NUMBER: _ClassVar[int]
     SEGMENT_DURATION_FIELD_NUMBER: _ClassVar[int]
     aliOSS: AliOSSUpload
     azure: AzureBlobUpload
     disable_manifest: bool
     filename_prefix: str
+    filename_suffix: SegmentedFileSuffix
     gcp: GCPUpload
     playlist_name: str
     protocol: SegmentedFileProtocol
     s3: S3Upload
     segment_duration: int
     def __init__(
         self,
         protocol: _Optional[_Union[SegmentedFileProtocol, str]] = ...,
         filename_prefix: _Optional[str] = ...,
         playlist_name: _Optional[str] = ...,
         segment_duration: _Optional[int] = ...,
+        filename_suffix: _Optional[_Union[SegmentedFileSuffix, str]] = ...,
         disable_manifest: bool = ...,
         s3: _Optional[_Union[S3Upload, _Mapping]] = ...,
         gcp: _Optional[_Union[GCPUpload, _Mapping]] = ...,
         azure: _Optional[_Union[AzureBlobUpload, _Mapping]] = ...,
         aliOSS: _Optional[_Union[AliOSSUpload, _Mapping]] = ...,
     ) -> None: ...
 
@@ -487,38 +526,41 @@
 class StopEgressRequest(_message.Message):
     __slots__ = ["egress_id"]
     EGRESS_ID_FIELD_NUMBER: _ClassVar[int]
     egress_id: str
     def __init__(self, egress_id: _Optional[str] = ...) -> None: ...
 
 class StreamInfo(_message.Message):
-    __slots__ = ["duration", "ended_at", "started_at", "status", "url"]
+    __slots__ = ["duration", "ended_at", "error", "started_at", "status", "url"]
 
     class Status(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
     ACTIVE: StreamInfo.Status
     DURATION_FIELD_NUMBER: _ClassVar[int]
     ENDED_AT_FIELD_NUMBER: _ClassVar[int]
+    ERROR_FIELD_NUMBER: _ClassVar[int]
     FAILED: StreamInfo.Status
     FINISHED: StreamInfo.Status
     STARTED_AT_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     URL_FIELD_NUMBER: _ClassVar[int]
     duration: int
     ended_at: int
+    error: str
     started_at: int
     status: StreamInfo.Status
     url: str
     def __init__(
         self,
         url: _Optional[str] = ...,
         started_at: _Optional[int] = ...,
         ended_at: _Optional[int] = ...,
         duration: _Optional[int] = ...,
         status: _Optional[_Union[StreamInfo.Status, str]] = ...,
+        error: _Optional[str] = ...,
     ) -> None: ...
 
 class StreamInfoList(_message.Message):
     __slots__ = ["info"]
     INFO_FIELD_NUMBER: _ClassVar[int]
     info: _containers.RepeatedCompositeFieldContainer[StreamInfo]
     def __init__(
@@ -538,46 +580,60 @@
     ) -> None: ...
 
 class TrackCompositeEgressRequest(_message.Message):
     __slots__ = [
         "advanced",
         "audio_track_id",
         "file",
+        "file_outputs",
         "preset",
         "room_name",
+        "segment_outputs",
         "segments",
         "stream",
+        "stream_outputs",
         "video_track_id",
     ]
     ADVANCED_FIELD_NUMBER: _ClassVar[int]
     AUDIO_TRACK_ID_FIELD_NUMBER: _ClassVar[int]
     FILE_FIELD_NUMBER: _ClassVar[int]
+    FILE_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
     PRESET_FIELD_NUMBER: _ClassVar[int]
     ROOM_NAME_FIELD_NUMBER: _ClassVar[int]
     SEGMENTS_FIELD_NUMBER: _ClassVar[int]
+    SEGMENT_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
     STREAM_FIELD_NUMBER: _ClassVar[int]
+    STREAM_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
     VIDEO_TRACK_ID_FIELD_NUMBER: _ClassVar[int]
     advanced: EncodingOptions
     audio_track_id: str
     file: EncodedFileOutput
+    file_outputs: _containers.RepeatedCompositeFieldContainer[EncodedFileOutput]
     preset: EncodingOptionsPreset
     room_name: str
+    segment_outputs: _containers.RepeatedCompositeFieldContainer[SegmentedFileOutput]
     segments: SegmentedFileOutput
     stream: StreamOutput
+    stream_outputs: _containers.RepeatedCompositeFieldContainer[StreamOutput]
     video_track_id: str
     def __init__(
         self,
         room_name: _Optional[str] = ...,
         audio_track_id: _Optional[str] = ...,
         video_track_id: _Optional[str] = ...,
         file: _Optional[_Union[EncodedFileOutput, _Mapping]] = ...,
         stream: _Optional[_Union[StreamOutput, _Mapping]] = ...,
         segments: _Optional[_Union[SegmentedFileOutput, _Mapping]] = ...,
         preset: _Optional[_Union[EncodingOptionsPreset, str]] = ...,
         advanced: _Optional[_Union[EncodingOptions, _Mapping]] = ...,
+        file_outputs: _Optional[_Iterable[_Union[EncodedFileOutput, _Mapping]]] = ...,
+        stream_outputs: _Optional[_Iterable[_Union[StreamOutput, _Mapping]]] = ...,
+        segment_outputs: _Optional[
+            _Iterable[_Union[SegmentedFileOutput, _Mapping]]
+        ] = ...,
     ) -> None: ...
 
 class TrackEgressRequest(_message.Message):
     __slots__ = ["file", "room_name", "track_id", "websocket_url"]
     FILE_FIELD_NUMBER: _ClassVar[int]
     ROOM_NAME_FIELD_NUMBER: _ClassVar[int]
     TRACK_ID_FIELD_NUMBER: _ClassVar[int]
@@ -620,61 +676,72 @@
     ) -> None: ...
 
 class WebEgressRequest(_message.Message):
     __slots__ = [
         "advanced",
         "audio_only",
         "file",
+        "file_outputs",
         "preset",
+        "segment_outputs",
         "segments",
         "stream",
+        "stream_outputs",
         "url",
         "video_only",
     ]
     ADVANCED_FIELD_NUMBER: _ClassVar[int]
     AUDIO_ONLY_FIELD_NUMBER: _ClassVar[int]
     FILE_FIELD_NUMBER: _ClassVar[int]
+    FILE_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
     PRESET_FIELD_NUMBER: _ClassVar[int]
     SEGMENTS_FIELD_NUMBER: _ClassVar[int]
+    SEGMENT_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
     STREAM_FIELD_NUMBER: _ClassVar[int]
+    STREAM_OUTPUTS_FIELD_NUMBER: _ClassVar[int]
     URL_FIELD_NUMBER: _ClassVar[int]
     VIDEO_ONLY_FIELD_NUMBER: _ClassVar[int]
     advanced: EncodingOptions
     audio_only: bool
     file: EncodedFileOutput
+    file_outputs: _containers.RepeatedCompositeFieldContainer[EncodedFileOutput]
     preset: EncodingOptionsPreset
+    segment_outputs: _containers.RepeatedCompositeFieldContainer[SegmentedFileOutput]
     segments: SegmentedFileOutput
     stream: StreamOutput
+    stream_outputs: _containers.RepeatedCompositeFieldContainer[StreamOutput]
     url: str
     video_only: bool
     def __init__(
         self,
         url: _Optional[str] = ...,
         audio_only: bool = ...,
         video_only: bool = ...,
         file: _Optional[_Union[EncodedFileOutput, _Mapping]] = ...,
         stream: _Optional[_Union[StreamOutput, _Mapping]] = ...,
         segments: _Optional[_Union[SegmentedFileOutput, _Mapping]] = ...,
         preset: _Optional[_Union[EncodingOptionsPreset, str]] = ...,
         advanced: _Optional[_Union[EncodingOptions, _Mapping]] = ...,
+        file_outputs: _Optional[_Iterable[_Union[EncodedFileOutput, _Mapping]]] = ...,
+        stream_outputs: _Optional[_Iterable[_Union[StreamOutput, _Mapping]]] = ...,
+        segment_outputs: _Optional[
+            _Iterable[_Union[SegmentedFileOutput, _Mapping]]
+        ] = ...,
     ) -> None: ...
 
 class EncodedFileType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
-class StreamProtocol(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
-
 class SegmentedFileProtocol(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
-class AudioCodec(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+class SegmentedFileSuffix(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
-class VideoCodec(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+class StreamProtocol(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
 class EncodingOptionsPreset(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
 class EgressStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_ingress_pb2.py` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_ingress_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,45 +11,52 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from . import livekit_models_pb2 as livekit__models__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x15livekit_ingress.proto\x12\x07livekit\x1a\x14livekit_models.proto"\xf4\x01\n\x14\x43reateIngressRequest\x12)\n\ninput_type\x18\x01 \x01(\x0e\x32\x15.livekit.IngressInput\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\x03 \x01(\t\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t\x12\x18\n\x10participant_name\x18\x05 \x01(\t\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptions"\x94\x01\n\x13IngressAudioOptions\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x06source\x18\x02 \x01(\x0e\x32\x14.livekit.TrackSource\x12\x11\n\tmime_type\x18\x03 \x01(\t\x12\x0f\n\x07\x62itrate\x18\x04 \x01(\r\x12\x13\n\x0b\x64isable_dtx\x18\x05 \x01(\x08\x12\x10\n\x08\x63hannels\x18\x06 \x01(\r"\x81\x01\n\x13IngressVideoOptions\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x06source\x18\x02 \x01(\x0e\x32\x14.livekit.TrackSource\x12\x11\n\tmime_type\x18\x03 \x01(\t\x12#\n\x06layers\x18\x04 \x03(\x0b\x32\x13.livekit.VideoLayer"\xd8\x02\n\x0bIngressInfo\x12\x12\n\ningress_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nstream_key\x18\x03 \x01(\t\x12\x0b\n\x03url\x18\x04 \x01(\t\x12)\n\ninput_type\x18\x05 \x01(\x0e\x32\x15.livekit.IngressInput\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptions\x12\x11\n\troom_name\x18\x08 \x01(\t\x12\x1c\n\x14participant_identity\x18\t \x01(\t\x12\x18\n\x10participant_name\x18\n \x01(\t\x12\x10\n\x08reusable\x18\x0b \x01(\x08\x12$\n\x05state\x18\x0c \x01(\x0b\x32\x15.livekit.IngressState"\xde\x02\n\x0cIngressState\x12,\n\x06status\x18\x01 \x01(\x0e\x32\x1c.livekit.IngressState.Status\x12\r\n\x05\x65rror\x18\x02 \x01(\t\x12\'\n\x05video\x18\x03 \x01(\x0b\x32\x18.livekit.InputVideoState\x12\'\n\x05\x61udio\x18\x04 \x01(\x0b\x32\x18.livekit.InputAudioState\x12\x0f\n\x07room_id\x18\x05 \x01(\t\x12\x12\n\nstarted_at\x18\x07 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x08 \x01(\x03\x12"\n\x06tracks\x18\x06 \x03(\x0b\x32\x12.livekit.TrackInfo"d\n\x06Status\x12\x15\n\x11\x45NDPOINT_INACTIVE\x10\x00\x12\x16\n\x12\x45NDPOINT_BUFFERING\x10\x01\x12\x17\n\x13\x45NDPOINT_PUBLISHING\x10\x02\x12\x12\n\x0e\x45NDPOINT_ERROR\x10\x03"V\n\x0fInputVideoState\x12\x11\n\tmime_type\x18\x01 \x01(\r\x12\r\n\x05width\x18\x03 \x01(\r\x12\x0e\n\x06height\x18\x04 \x01(\r\x12\x11\n\tframerate\x18\x05 \x01(\r"K\n\x0fInputAudioState\x12\x11\n\tmime_type\x18\x01 \x01(\r\x12\x10\n\x08\x63hannels\x18\x03 \x01(\r\x12\x13\n\x0bsample_rate\x18\x04 \x01(\r"\xdd\x01\n\x14UpdateIngressRequest\x12\x12\n\ningress_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\x03 \x01(\t\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t\x12\x18\n\x10participant_name\x18\x05 \x01(\t\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptions"\'\n\x12ListIngressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t":\n\x13ListIngressResponse\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.livekit.IngressInfo"*\n\x14\x44\x65leteIngressRequest\x12\x12\n\ningress_id\x18\x01 \x01(\t*\x1e\n\x0cIngressInput\x12\x0e\n\nRTMP_INPUT\x10\x00\x32\xa5\x02\n\x07Ingress\x12\x44\n\rCreateIngress\x12\x1d.livekit.CreateIngressRequest\x1a\x14.livekit.IngressInfo\x12\x44\n\rUpdateIngress\x12\x1d.livekit.UpdateIngressRequest\x1a\x14.livekit.IngressInfo\x12H\n\x0bListIngress\x12\x1b.livekit.ListIngressRequest\x1a\x1c.livekit.ListIngressResponse\x12\x44\n\rDeleteIngress\x12\x1d.livekit.DeleteIngressRequest\x1a\x14.livekit.IngressInfoBFZ#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
+    b'\n\x15livekit_ingress.proto\x12\x07livekit\x1a\x14livekit_models.proto"\xf4\x01\n\x14\x43reateIngressRequest\x12)\n\ninput_type\x18\x01 \x01(\x0e\x32\x15.livekit.IngressInput\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\x03 \x01(\t\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t\x12\x18\n\x10participant_name\x18\x05 \x01(\t\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptions"\xcd\x01\n\x13IngressAudioOptions\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x06source\x18\x02 \x01(\x0e\x32\x14.livekit.TrackSource\x12\x35\n\x06preset\x18\x03 \x01(\x0e\x32#.livekit.IngressAudioEncodingPresetH\x00\x12\x37\n\x07options\x18\x04 \x01(\x0b\x32$.livekit.IngressAudioEncodingOptionsH\x00\x42\x12\n\x10\x65ncoding_options"\xcd\x01\n\x13IngressVideoOptions\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x06source\x18\x02 \x01(\x0e\x32\x14.livekit.TrackSource\x12\x35\n\x06preset\x18\x03 \x01(\x0e\x32#.livekit.IngressVideoEncodingPresetH\x00\x12\x37\n\x07options\x18\x04 \x01(\x0b\x32$.livekit.IngressVideoEncodingOptionsH\x00\x42\x12\n\x10\x65ncoding_options"\x7f\n\x1bIngressAudioEncodingOptions\x12(\n\x0b\x61udio_codec\x18\x01 \x01(\x0e\x32\x13.livekit.AudioCodec\x12\x0f\n\x07\x62itrate\x18\x02 \x01(\r\x12\x13\n\x0b\x64isable_dtx\x18\x03 \x01(\x08\x12\x10\n\x08\x63hannels\x18\x04 \x01(\r"\x80\x01\n\x1bIngressVideoEncodingOptions\x12(\n\x0bvideo_codec\x18\x01 \x01(\x0e\x32\x13.livekit.VideoCodec\x12\x12\n\nframe_rate\x18\x02 \x01(\x01\x12#\n\x06layers\x18\x03 \x03(\x0b\x32\x13.livekit.VideoLayer"\xd8\x02\n\x0bIngressInfo\x12\x12\n\ningress_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nstream_key\x18\x03 \x01(\t\x12\x0b\n\x03url\x18\x04 \x01(\t\x12)\n\ninput_type\x18\x05 \x01(\x0e\x32\x15.livekit.IngressInput\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptions\x12\x11\n\troom_name\x18\x08 \x01(\t\x12\x1c\n\x14participant_identity\x18\t \x01(\t\x12\x18\n\x10participant_name\x18\n \x01(\t\x12\x10\n\x08reusable\x18\x0b \x01(\x08\x12$\n\x05state\x18\x0c \x01(\x0b\x32\x15.livekit.IngressState"\xde\x02\n\x0cIngressState\x12,\n\x06status\x18\x01 \x01(\x0e\x32\x1c.livekit.IngressState.Status\x12\r\n\x05\x65rror\x18\x02 \x01(\t\x12\'\n\x05video\x18\x03 \x01(\x0b\x32\x18.livekit.InputVideoState\x12\'\n\x05\x61udio\x18\x04 \x01(\x0b\x32\x18.livekit.InputAudioState\x12\x0f\n\x07room_id\x18\x05 \x01(\t\x12\x12\n\nstarted_at\x18\x07 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x08 \x01(\x03\x12"\n\x06tracks\x18\x06 \x03(\x0b\x32\x12.livekit.TrackInfo"d\n\x06Status\x12\x15\n\x11\x45NDPOINT_INACTIVE\x10\x00\x12\x16\n\x12\x45NDPOINT_BUFFERING\x10\x01\x12\x17\n\x13\x45NDPOINT_PUBLISHING\x10\x02\x12\x12\n\x0e\x45NDPOINT_ERROR\x10\x03"V\n\x0fInputVideoState\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\r\n\x05width\x18\x03 \x01(\r\x12\x0e\n\x06height\x18\x04 \x01(\r\x12\x11\n\tframerate\x18\x05 \x01(\r"K\n\x0fInputAudioState\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x10\n\x08\x63hannels\x18\x03 \x01(\r\x12\x13\n\x0bsample_rate\x18\x04 \x01(\r"\xdd\x01\n\x14UpdateIngressRequest\x12\x12\n\ningress_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\x03 \x01(\t\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t\x12\x18\n\x10participant_name\x18\x05 \x01(\t\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptions"\'\n\x12ListIngressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t":\n\x13ListIngressResponse\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.livekit.IngressInfo"*\n\x14\x44\x65leteIngressRequest\x12\x12\n\ningress_id\x18\x01 \x01(\t*\x1e\n\x0cIngressInput\x12\x0e\n\nRTMP_INPUT\x10\x00*I\n\x1aIngressAudioEncodingPreset\x12\x16\n\x12OPUS_STEREO_96KBPS\x10\x00\x12\x13\n\x0fOPUS_MONO_64KBS\x10\x01*\xb2\x01\n\x1aIngressVideoEncodingPreset\x12\x1c\n\x18H264_720P_30FPS_3_LAYERS\x10\x00\x12\x1d\n\x19H264_1080P_30FPS_3_LAYERS\x10\x01\x12\x1c\n\x18H264_540P_25FPS_2_LAYERS\x10\x02\x12\x1b\n\x17H264_720P_30FPS_1_LAYER\x10\x03\x12\x1c\n\x18H264_1080P_30FPS_1_LAYER\x10\x04\x32\xa5\x02\n\x07Ingress\x12\x44\n\rCreateIngress\x12\x1d.livekit.CreateIngressRequest\x1a\x14.livekit.IngressInfo\x12\x44\n\rUpdateIngress\x12\x1d.livekit.UpdateIngressRequest\x1a\x14.livekit.IngressInfo\x12H\n\x0bListIngress\x12\x1b.livekit.ListIngressRequest\x1a\x1c.livekit.ListIngressResponse\x12\x44\n\rDeleteIngress\x12\x1d.livekit.DeleteIngressRequest\x1a\x14.livekit.IngressInfoBFZ#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "livekit_ingress_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto"
-    _INGRESSINPUT._serialized_start = 1820
-    _INGRESSINPUT._serialized_end = 1850
+    _INGRESSINPUT._serialized_start = 2213
+    _INGRESSINPUT._serialized_end = 2243
+    _INGRESSAUDIOENCODINGPRESET._serialized_start = 2245
+    _INGRESSAUDIOENCODINGPRESET._serialized_end = 2318
+    _INGRESSVIDEOENCODINGPRESET._serialized_start = 2321
+    _INGRESSVIDEOENCODINGPRESET._serialized_end = 2499
     _CREATEINGRESSREQUEST._serialized_start = 57
     _CREATEINGRESSREQUEST._serialized_end = 301
     _INGRESSAUDIOOPTIONS._serialized_start = 304
-    _INGRESSAUDIOOPTIONS._serialized_end = 452
-    _INGRESSVIDEOOPTIONS._serialized_start = 455
-    _INGRESSVIDEOOPTIONS._serialized_end = 584
-    _INGRESSINFO._serialized_start = 587
-    _INGRESSINFO._serialized_end = 931
-    _INGRESSSTATE._serialized_start = 934
-    _INGRESSSTATE._serialized_end = 1284
-    _INGRESSSTATE_STATUS._serialized_start = 1184
-    _INGRESSSTATE_STATUS._serialized_end = 1284
-    _INPUTVIDEOSTATE._serialized_start = 1286
-    _INPUTVIDEOSTATE._serialized_end = 1372
-    _INPUTAUDIOSTATE._serialized_start = 1374
-    _INPUTAUDIOSTATE._serialized_end = 1449
-    _UPDATEINGRESSREQUEST._serialized_start = 1452
-    _UPDATEINGRESSREQUEST._serialized_end = 1673
-    _LISTINGRESSREQUEST._serialized_start = 1675
-    _LISTINGRESSREQUEST._serialized_end = 1714
-    _LISTINGRESSRESPONSE._serialized_start = 1716
-    _LISTINGRESSRESPONSE._serialized_end = 1774
-    _DELETEINGRESSREQUEST._serialized_start = 1776
-    _DELETEINGRESSREQUEST._serialized_end = 1818
-    _INGRESS._serialized_start = 1853
-    _INGRESS._serialized_end = 2146
+    _INGRESSAUDIOOPTIONS._serialized_end = 509
+    _INGRESSVIDEOOPTIONS._serialized_start = 512
+    _INGRESSVIDEOOPTIONS._serialized_end = 717
+    _INGRESSAUDIOENCODINGOPTIONS._serialized_start = 719
+    _INGRESSAUDIOENCODINGOPTIONS._serialized_end = 846
+    _INGRESSVIDEOENCODINGOPTIONS._serialized_start = 849
+    _INGRESSVIDEOENCODINGOPTIONS._serialized_end = 977
+    _INGRESSINFO._serialized_start = 980
+    _INGRESSINFO._serialized_end = 1324
+    _INGRESSSTATE._serialized_start = 1327
+    _INGRESSSTATE._serialized_end = 1677
+    _INGRESSSTATE_STATUS._serialized_start = 1577
+    _INGRESSSTATE_STATUS._serialized_end = 1677
+    _INPUTVIDEOSTATE._serialized_start = 1679
+    _INPUTVIDEOSTATE._serialized_end = 1765
+    _INPUTAUDIOSTATE._serialized_start = 1767
+    _INPUTAUDIOSTATE._serialized_end = 1842
+    _UPDATEINGRESSREQUEST._serialized_start = 1845
+    _UPDATEINGRESSREQUEST._serialized_end = 2066
+    _LISTINGRESSREQUEST._serialized_start = 2068
+    _LISTINGRESSREQUEST._serialized_end = 2107
+    _LISTINGRESSRESPONSE._serialized_start = 2109
+    _LISTINGRESSRESPONSE._serialized_end = 2167
+    _DELETEINGRESSREQUEST._serialized_start = 2169
+    _DELETEINGRESSREQUEST._serialized_end = 2211
+    _INGRESS._serialized_start = 2502
+    _INGRESS._serialized_end = 2795
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_ingress_pb2.pyi` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_ingress_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 import livekit_models_pb2 as _livekit_models_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 
 DESCRIPTOR: _descriptor.FileDescriptor
+H264_1080P_30FPS_1_LAYER: IngressVideoEncodingPreset
+H264_1080P_30FPS_3_LAYERS: IngressVideoEncodingPreset
+H264_540P_25FPS_2_LAYERS: IngressVideoEncodingPreset
+H264_720P_30FPS_1_LAYER: IngressVideoEncodingPreset
+H264_720P_30FPS_3_LAYERS: IngressVideoEncodingPreset
+OPUS_MONO_64KBS: IngressAudioEncodingPreset
+OPUS_STEREO_96KBPS: IngressAudioEncodingPreset
 RTMP_INPUT: IngressInput
 
 class CreateIngressRequest(_message.Message):
     __slots__ = [
         "audio",
         "input_type",
         "name",
@@ -50,36 +57,48 @@
 
 class DeleteIngressRequest(_message.Message):
     __slots__ = ["ingress_id"]
     INGRESS_ID_FIELD_NUMBER: _ClassVar[int]
     ingress_id: str
     def __init__(self, ingress_id: _Optional[str] = ...) -> None: ...
 
-class IngressAudioOptions(_message.Message):
-    __slots__ = ["bitrate", "channels", "disable_dtx", "mime_type", "name", "source"]
+class IngressAudioEncodingOptions(_message.Message):
+    __slots__ = ["audio_codec", "bitrate", "channels", "disable_dtx"]
+    AUDIO_CODEC_FIELD_NUMBER: _ClassVar[int]
     BITRATE_FIELD_NUMBER: _ClassVar[int]
     CHANNELS_FIELD_NUMBER: _ClassVar[int]
     DISABLE_DTX_FIELD_NUMBER: _ClassVar[int]
-    MIME_TYPE_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    SOURCE_FIELD_NUMBER: _ClassVar[int]
+    audio_codec: _livekit_models_pb2.AudioCodec
     bitrate: int
     channels: int
     disable_dtx: bool
-    mime_type: str
+    def __init__(
+        self,
+        audio_codec: _Optional[_Union[_livekit_models_pb2.AudioCodec, str]] = ...,
+        bitrate: _Optional[int] = ...,
+        disable_dtx: bool = ...,
+        channels: _Optional[int] = ...,
+    ) -> None: ...
+
+class IngressAudioOptions(_message.Message):
+    __slots__ = ["name", "options", "preset", "source"]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    OPTIONS_FIELD_NUMBER: _ClassVar[int]
+    PRESET_FIELD_NUMBER: _ClassVar[int]
+    SOURCE_FIELD_NUMBER: _ClassVar[int]
     name: str
+    options: IngressAudioEncodingOptions
+    preset: IngressAudioEncodingPreset
     source: _livekit_models_pb2.TrackSource
     def __init__(
         self,
         name: _Optional[str] = ...,
         source: _Optional[_Union[_livekit_models_pb2.TrackSource, str]] = ...,
-        mime_type: _Optional[str] = ...,
-        bitrate: _Optional[int] = ...,
-        disable_dtx: bool = ...,
-        channels: _Optional[int] = ...,
+        preset: _Optional[_Union[IngressAudioEncodingPreset, str]] = ...,
+        options: _Optional[_Union[IngressAudioEncodingOptions, _Mapping]] = ...,
     ) -> None: ...
 
 class IngressInfo(_message.Message):
     __slots__ = [
         "audio",
         "ingress_id",
         "input_type",
@@ -177,62 +196,77 @@
         started_at: _Optional[int] = ...,
         ended_at: _Optional[int] = ...,
         tracks: _Optional[
             _Iterable[_Union[_livekit_models_pb2.TrackInfo, _Mapping]]
         ] = ...,
     ) -> None: ...
 
-class IngressVideoOptions(_message.Message):
-    __slots__ = ["layers", "mime_type", "name", "source"]
+class IngressVideoEncodingOptions(_message.Message):
+    __slots__ = ["frame_rate", "layers", "video_codec"]
+    FRAME_RATE_FIELD_NUMBER: _ClassVar[int]
     LAYERS_FIELD_NUMBER: _ClassVar[int]
-    MIME_TYPE_FIELD_NUMBER: _ClassVar[int]
+    VIDEO_CODEC_FIELD_NUMBER: _ClassVar[int]
+    frame_rate: float
+    layers: _containers.RepeatedCompositeFieldContainer[_livekit_models_pb2.VideoLayer]
+    video_codec: _livekit_models_pb2.VideoCodec
+    def __init__(
+        self,
+        video_codec: _Optional[_Union[_livekit_models_pb2.VideoCodec, str]] = ...,
+        frame_rate: _Optional[float] = ...,
+        layers: _Optional[
+            _Iterable[_Union[_livekit_models_pb2.VideoLayer, _Mapping]]
+        ] = ...,
+    ) -> None: ...
+
+class IngressVideoOptions(_message.Message):
+    __slots__ = ["name", "options", "preset", "source"]
     NAME_FIELD_NUMBER: _ClassVar[int]
+    OPTIONS_FIELD_NUMBER: _ClassVar[int]
+    PRESET_FIELD_NUMBER: _ClassVar[int]
     SOURCE_FIELD_NUMBER: _ClassVar[int]
-    layers: _containers.RepeatedCompositeFieldContainer[_livekit_models_pb2.VideoLayer]
-    mime_type: str
     name: str
+    options: IngressVideoEncodingOptions
+    preset: IngressVideoEncodingPreset
     source: _livekit_models_pb2.TrackSource
     def __init__(
         self,
         name: _Optional[str] = ...,
         source: _Optional[_Union[_livekit_models_pb2.TrackSource, str]] = ...,
-        mime_type: _Optional[str] = ...,
-        layers: _Optional[
-            _Iterable[_Union[_livekit_models_pb2.VideoLayer, _Mapping]]
-        ] = ...,
+        preset: _Optional[_Union[IngressVideoEncodingPreset, str]] = ...,
+        options: _Optional[_Union[IngressVideoEncodingOptions, _Mapping]] = ...,
     ) -> None: ...
 
 class InputAudioState(_message.Message):
     __slots__ = ["channels", "mime_type", "sample_rate"]
     CHANNELS_FIELD_NUMBER: _ClassVar[int]
     MIME_TYPE_FIELD_NUMBER: _ClassVar[int]
     SAMPLE_RATE_FIELD_NUMBER: _ClassVar[int]
     channels: int
-    mime_type: int
+    mime_type: str
     sample_rate: int
     def __init__(
         self,
-        mime_type: _Optional[int] = ...,
+        mime_type: _Optional[str] = ...,
         channels: _Optional[int] = ...,
         sample_rate: _Optional[int] = ...,
     ) -> None: ...
 
 class InputVideoState(_message.Message):
     __slots__ = ["framerate", "height", "mime_type", "width"]
     FRAMERATE_FIELD_NUMBER: _ClassVar[int]
     HEIGHT_FIELD_NUMBER: _ClassVar[int]
     MIME_TYPE_FIELD_NUMBER: _ClassVar[int]
     WIDTH_FIELD_NUMBER: _ClassVar[int]
     framerate: int
     height: int
-    mime_type: int
+    mime_type: str
     width: int
     def __init__(
         self,
-        mime_type: _Optional[int] = ...,
+        mime_type: _Optional[str] = ...,
         width: _Optional[int] = ...,
         height: _Optional[int] = ...,
         framerate: _Optional[int] = ...,
     ) -> None: ...
 
 class ListIngressRequest(_message.Message):
     __slots__ = ["room_name"]
@@ -281,7 +315,13 @@
         participant_name: _Optional[str] = ...,
         audio: _Optional[_Union[IngressAudioOptions, _Mapping]] = ...,
         video: _Optional[_Union[IngressVideoOptions, _Mapping]] = ...,
     ) -> None: ...
 
 class IngressInput(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
+
+class IngressAudioEncodingPreset(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+
+class IngressVideoEncodingPreset(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_internal_pb2.py` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_internal_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,39 +14,42 @@
 
 from . import livekit_egress_pb2 as livekit__egress__pb2
 from . import livekit_models_pb2 as livekit__models__pb2
 from . import livekit_room_pb2 as livekit__room__pb2
 from . import livekit_rtc_pb2 as livekit__rtc__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x16livekit_internal.proto\x12\x07livekit\x1a\x14livekit_models.proto\x1a\x11livekit_rtc.proto\x1a\x12livekit_room.proto\x1a\x14livekit_egress.proto"\xa7\x01\n\x04Node\x12\n\n\x02id\x18\x01 \x01(\t\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x10\n\x08num_cpus\x18\x03 \x01(\r\x12!\n\x05stats\x18\x04 \x01(\x0b\x32\x12.livekit.NodeStats\x12\x1f\n\x04type\x18\x05 \x01(\x0e\x32\x11.livekit.NodeType\x12!\n\x05state\x18\x06 \x01(\x0e\x32\x12.livekit.NodeState\x12\x0e\n\x06region\x18\x07 \x01(\t"\xe8\x06\n\tNodeStats\x12\x12\n\nstarted_at\x18\x01 \x01(\x03\x12\x12\n\nupdated_at\x18\x02 \x01(\x03\x12\x11\n\tnum_rooms\x18\x03 \x01(\x05\x12\x13\n\x0bnum_clients\x18\x04 \x01(\x05\x12\x15\n\rnum_tracks_in\x18\x05 \x01(\x05\x12\x16\n\x0enum_tracks_out\x18\x06 \x01(\x05\x12\x10\n\x08\x62ytes_in\x18\x07 \x01(\x04\x12\x11\n\tbytes_out\x18\x08 \x01(\x04\x12\x12\n\npackets_in\x18\t \x01(\x04\x12\x13\n\x0bpackets_out\x18\n \x01(\x04\x12\x12\n\nnack_total\x18\x0b \x01(\x04\x12\x18\n\x10\x62ytes_in_per_sec\x18\x0c \x01(\x02\x12\x19\n\x11\x62ytes_out_per_sec\x18\r \x01(\x02\x12\x1a\n\x12packets_in_per_sec\x18\x0e \x01(\x02\x12\x1b\n\x13packets_out_per_sec\x18\x0f \x01(\x02\x12\x14\n\x0cnack_per_sec\x18\x10 \x01(\x02\x12\x10\n\x08num_cpus\x18\x11 \x01(\r\x12\x19\n\x11load_avg_last1min\x18\x12 \x01(\x02\x12\x19\n\x11load_avg_last5min\x18\x13 \x01(\x02\x12\x1a\n\x12load_avg_last15min\x18\x14 \x01(\x02\x12\x10\n\x08\x63pu_load\x18\x15 \x01(\x02\x12\x13\n\x0bmemory_load\x18! \x01(\x02\x12\x17\n\x0fsys_packets_out\x18\x1c \x01(\r\x12\x1b\n\x13sys_packets_dropped\x18\x1d \x01(\r\x12\x1f\n\x17sys_packets_out_per_sec\x18\x1e \x01(\x02\x12#\n\x1bsys_packets_dropped_per_sec\x18\x1f \x01(\x02\x12\'\n\x1fsys_packets_dropped_pct_per_sec\x18  \x01(\x02\x12\x1c\n\x14retransmit_bytes_out\x18\x16 \x01(\x04\x12\x1e\n\x16retransmit_packets_out\x18\x17 \x01(\x04\x12$\n\x1cretransmit_bytes_out_per_sec\x18\x18 \x01(\x02\x12&\n\x1eretransmit_packets_out_per_sec\x18\x19 \x01(\x02\x12\x18\n\x10participant_join\x18\x1a \x01(\x04\x12 \n\x18participant_join_per_sec\x18\x1b \x01(\x02"\x86\x05\n\x0eRTCNodeMessage\x12\x17\n\x0fparticipant_key\x18\x01 \x01(\t\x12\x13\n\x0bsender_time\x18\x0b \x01(\x03\x12\x15\n\rconnection_id\x18\r \x01(\t\x12.\n\rstart_session\x18\x02 \x01(\x0b\x32\x15.livekit.StartSessionH\x00\x12)\n\x07request\x18\x03 \x01(\x0b\x32\x16.livekit.SignalRequestH\x00\x12>\n\x12remove_participant\x18\x04 \x01(\x0b\x32 .livekit.RoomParticipantIdentityH\x00\x12\x33\n\nmute_track\x18\x05 \x01(\x0b\x32\x1d.livekit.MuteRoomTrackRequestH\x00\x12?\n\x12update_participant\x18\x06 \x01(\x0b\x32!.livekit.UpdateParticipantRequestH\x00\x12\x31\n\x0b\x64\x65lete_room\x18\x07 \x01(\x0b\x32\x1a.livekit.DeleteRoomRequestH\x00\x12\x43\n\x14update_subscriptions\x18\x08 \x01(\x0b\x32#.livekit.UpdateSubscriptionsRequestH\x00\x12-\n\tsend_data\x18\t \x01(\x0b\x32\x18.livekit.SendDataRequestH\x00\x12\x42\n\x14update_room_metadata\x18\n \x01(\x0b\x32".livekit.UpdateRoomMetadataRequestH\x00\x12(\n\nkeep_alive\x18\x0c \x01(\x0b\x32\x12.livekit.KeepAliveH\x00\x42\t\n\x07message"\x8e\x01\n\x11SignalNodeMessage\x12\x15\n\rconnection_id\x18\x01 \x01(\t\x12+\n\x08response\x18\x02 \x01(\x0b\x32\x17.livekit.SignalResponseH\x00\x12*\n\x0b\x65nd_session\x18\x03 \x01(\x0b\x32\x13.livekit.EndSessionH\x00\x42\t\n\x07message"\x90\x02\n\x0cStartSession\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x15\n\rconnection_id\x18\x03 \x01(\t\x12\x11\n\treconnect\x18\x04 \x01(\x08\x12\x16\n\x0e\x61uto_subscribe\x18\t \x01(\x08\x12\x0e\n\x06hidden\x18\n \x01(\x08\x12#\n\x06\x63lient\x18\x0b \x01(\x0b\x32\x13.livekit.ClientInfo\x12\x10\n\x08recorder\x18\x0c \x01(\x08\x12\x0c\n\x04name\x18\r \x01(\t\x12\x13\n\x0bgrants_json\x18\x0e \x01(\t\x12\x17\n\x0f\x61\x64\x61ptive_stream\x18\x0f \x01(\x08\x12\x16\n\x0eparticipant_id\x18\x10 \x01(\t"\x0c\n\nEndSession"+\n\x11RemoveParticipant\x12\x16\n\x0eparticipant_id\x18\x01 \x01(\t"\x0b\n\tKeepAlive">\n\x0cRoomInternal\x12.\n\x0ctrack_egress\x18\x01 \x01(\x0b\x32\x18.livekit.AutoTrackEgress*;\n\x08NodeType\x12\n\n\x06SERVER\x10\x00\x12\x0e\n\nCONTROLLER\x10\x01\x12\t\n\x05MEDIA\x10\x02\x12\x08\n\x04TURN\x10\x04*<\n\tNodeState\x12\x0f\n\x0bSTARTING_UP\x10\x00\x12\x0b\n\x07SERVING\x10\x01\x12\x11\n\rSHUTTING_DOWN\x10\x02\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
+    b'\n\x16livekit_internal.proto\x12\x07livekit\x1a\x14livekit_models.proto\x1a\x11livekit_rtc.proto\x1a\x12livekit_room.proto\x1a\x14livekit_egress.proto"\xa7\x01\n\x04Node\x12\n\n\x02id\x18\x01 \x01(\t\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x10\n\x08num_cpus\x18\x03 \x01(\r\x12!\n\x05stats\x18\x04 \x01(\x0b\x32\x12.livekit.NodeStats\x12\x1f\n\x04type\x18\x05 \x01(\x0e\x32\x11.livekit.NodeType\x12!\n\x05state\x18\x06 \x01(\x0e\x32\x12.livekit.NodeState\x12\x0e\n\x06region\x18\x07 \x01(\t"\xf1\n\n\tNodeStats\x12\x12\n\nstarted_at\x18\x01 \x01(\x03\x12\x12\n\nupdated_at\x18\x02 \x01(\x03\x12\x11\n\tnum_rooms\x18\x03 \x01(\x05\x12\x13\n\x0bnum_clients\x18\x04 \x01(\x05\x12\x15\n\rnum_tracks_in\x18\x05 \x01(\x05\x12\x16\n\x0enum_tracks_out\x18\x06 \x01(\x05\x12"\n\x1anum_track_publish_attempts\x18$ \x01(\x05\x12&\n\x1etrack_publish_attempts_per_sec\x18% \x01(\x02\x12!\n\x19num_track_publish_success\x18& \x01(\x05\x12%\n\x1dtrack_publish_success_per_sec\x18\' \x01(\x02\x12$\n\x1cnum_track_subscribe_attempts\x18( \x01(\x05\x12(\n track_subscribe_attempts_per_sec\x18) \x01(\x02\x12#\n\x1bnum_track_subscribe_success\x18* \x01(\x05\x12\'\n\x1ftrack_subscribe_success_per_sec\x18+ \x01(\x02\x12\x10\n\x08\x62ytes_in\x18\x07 \x01(\x04\x12\x11\n\tbytes_out\x18\x08 \x01(\x04\x12\x12\n\npackets_in\x18\t \x01(\x04\x12\x13\n\x0bpackets_out\x18\n \x01(\x04\x12\x12\n\nnack_total\x18\x0b \x01(\x04\x12\x18\n\x10\x62ytes_in_per_sec\x18\x0c \x01(\x02\x12\x19\n\x11\x62ytes_out_per_sec\x18\r \x01(\x02\x12\x1a\n\x12packets_in_per_sec\x18\x0e \x01(\x02\x12\x1b\n\x13packets_out_per_sec\x18\x0f \x01(\x02\x12\x14\n\x0cnack_per_sec\x18\x10 \x01(\x02\x12\x10\n\x08num_cpus\x18\x11 \x01(\r\x12\x19\n\x11load_avg_last1min\x18\x12 \x01(\x02\x12\x19\n\x11load_avg_last5min\x18\x13 \x01(\x02\x12\x1a\n\x12load_avg_last15min\x18\x14 \x01(\x02\x12\x10\n\x08\x63pu_load\x18\x15 \x01(\x02\x12\x13\n\x0bmemory_load\x18! \x01(\x02\x12\x14\n\x0cmemory_total\x18" \x01(\x04\x12\x13\n\x0bmemory_used\x18# \x01(\x04\x12\x17\n\x0fsys_packets_out\x18\x1c \x01(\r\x12\x1b\n\x13sys_packets_dropped\x18\x1d \x01(\r\x12\x1f\n\x17sys_packets_out_per_sec\x18\x1e \x01(\x02\x12#\n\x1bsys_packets_dropped_per_sec\x18\x1f \x01(\x02\x12\'\n\x1fsys_packets_dropped_pct_per_sec\x18  \x01(\x02\x12\x1c\n\x14retransmit_bytes_out\x18\x16 \x01(\x04\x12\x1e\n\x16retransmit_packets_out\x18\x17 \x01(\x04\x12$\n\x1cretransmit_bytes_out_per_sec\x18\x18 \x01(\x02\x12&\n\x1eretransmit_packets_out_per_sec\x18\x19 \x01(\x02\x12$\n\x1cparticipant_signal_connected\x18\x1a \x01(\x04\x12,\n$participant_signal_connected_per_sec\x18\x1b \x01(\x02\x12!\n\x19participant_rtc_connected\x18, \x01(\x04\x12)\n!participant_rtc_connected_per_sec\x18- \x01(\x02\x12\x1c\n\x14participant_rtc_init\x18. \x01(\x04\x12$\n\x1cparticipant_rtc_init_per_sec\x18/ \x01(\x02"\xc8\x05\n\x0eRTCNodeMessage\x12\x17\n\x0fparticipant_key\x18\x01 \x01(\t\x12\x13\n\x0bsender_time\x18\x0b \x01(\x03\x12\x15\n\rconnection_id\x18\r \x01(\t\x12\x1b\n\x13participant_key_b62\x18\x0e \x01(\t\x12\x11\n\troom_name\x18\x0f \x01(\t\x12\x10\n\x08identity\x18\x10 \x01(\t\x12.\n\rstart_session\x18\x02 \x01(\x0b\x32\x15.livekit.StartSessionH\x00\x12)\n\x07request\x18\x03 \x01(\x0b\x32\x16.livekit.SignalRequestH\x00\x12>\n\x12remove_participant\x18\x04 \x01(\x0b\x32 .livekit.RoomParticipantIdentityH\x00\x12\x33\n\nmute_track\x18\x05 \x01(\x0b\x32\x1d.livekit.MuteRoomTrackRequestH\x00\x12?\n\x12update_participant\x18\x06 \x01(\x0b\x32!.livekit.UpdateParticipantRequestH\x00\x12\x31\n\x0b\x64\x65lete_room\x18\x07 \x01(\x0b\x32\x1a.livekit.DeleteRoomRequestH\x00\x12\x43\n\x14update_subscriptions\x18\x08 \x01(\x0b\x32#.livekit.UpdateSubscriptionsRequestH\x00\x12-\n\tsend_data\x18\t \x01(\x0b\x32\x18.livekit.SendDataRequestH\x00\x12\x42\n\x14update_room_metadata\x18\n \x01(\x0b\x32".livekit.UpdateRoomMetadataRequestH\x00\x12(\n\nkeep_alive\x18\x0c \x01(\x0b\x32\x12.livekit.KeepAliveH\x00\x42\t\n\x07message"\x8e\x01\n\x11SignalNodeMessage\x12\x15\n\rconnection_id\x18\x01 \x01(\t\x12+\n\x08response\x18\x02 \x01(\x0b\x32\x17.livekit.SignalResponseH\x00\x12*\n\x0b\x65nd_session\x18\x03 \x01(\x0b\x32\x13.livekit.EndSessionH\x00\x42\t\n\x07message"\x84\x03\n\x0cStartSession\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x15\n\rconnection_id\x18\x03 \x01(\t\x12\x11\n\treconnect\x18\x04 \x01(\x08\x12\x16\n\x0e\x61uto_subscribe\x18\t \x01(\x08\x12\x0e\n\x06hidden\x18\n \x01(\x08\x12#\n\x06\x63lient\x18\x0b \x01(\x0b\x32\x13.livekit.ClientInfo\x12\x10\n\x08recorder\x18\x0c \x01(\x08\x12\x0c\n\x04name\x18\r \x01(\t\x12\x13\n\x0bgrants_json\x18\x0e \x01(\t\x12\x17\n\x0f\x61\x64\x61ptive_stream\x18\x0f \x01(\x08\x12\x16\n\x0eparticipant_id\x18\x10 \x01(\t\x12\x32\n\x10reconnect_reason\x18\x11 \x01(\x0e\x32\x18.livekit.ReconnectReason\x12#\n\x16subscriber_allow_pause\x18\x12 \x01(\x08H\x00\x88\x01\x01\x42\x19\n\x17_subscriber_allow_pause"\x0c\n\nEndSession"+\n\x11RemoveParticipant\x12\x16\n\x0eparticipant_id\x18\x01 \x01(\t"\x0b\n\tKeepAlive">\n\x0cRoomInternal\x12.\n\x0ctrack_egress\x18\x01 \x01(\x0b\x32\x18.livekit.AutoTrackEgress"~\n\tICEConfig\x12\x38\n\x15preference_subscriber\x18\x01 \x01(\x0e\x32\x19.livekit.ICECandidateType\x12\x37\n\x14preference_publisher\x18\x02 \x01(\x0e\x32\x19.livekit.ICECandidateType*H\n\x08NodeType\x12\n\n\x06SERVER\x10\x00\x12\x0e\n\nCONTROLLER\x10\x01\x12\t\n\x05MEDIA\x10\x02\x12\x08\n\x04TURN\x10\x04\x12\x0b\n\x07SWEEPER\x10\x05*<\n\tNodeState\x12\x0f\n\x0bSTARTING_UP\x10\x00\x12\x0b\n\x07SERVING\x10\x01\x12\x11\n\rSHUTTING_DOWN\x10\x02*:\n\x10ICECandidateType\x12\x0c\n\x08ICT_NONE\x10\x00\x12\x0b\n\x07ICT_TCP\x10\x01\x12\x0b\n\x07ICT_TLS\x10\x02\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "livekit_internal_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto"
-    _NODETYPE._serialized_start = 2368
-    _NODETYPE._serialized_end = 2427
-    _NODESTATE._serialized_start = 2429
-    _NODESTATE._serialized_end = 2489
+    _NODETYPE._serialized_start = 3199
+    _NODETYPE._serialized_end = 3271
+    _NODESTATE._serialized_start = 3273
+    _NODESTATE._serialized_end = 3333
+    _ICECANDIDATETYPE._serialized_start = 3335
+    _ICECANDIDATETYPE._serialized_end = 3393
     _NODE._serialized_start = 119
     _NODE._serialized_end = 286
     _NODESTATS._serialized_start = 289
-    _NODESTATS._serialized_end = 1161
-    _RTCNODEMESSAGE._serialized_start = 1164
-    _RTCNODEMESSAGE._serialized_end = 1810
-    _SIGNALNODEMESSAGE._serialized_start = 1813
-    _SIGNALNODEMESSAGE._serialized_end = 1955
-    _STARTSESSION._serialized_start = 1958
-    _STARTSESSION._serialized_end = 2230
-    _ENDSESSION._serialized_start = 2232
-    _ENDSESSION._serialized_end = 2244
-    _REMOVEPARTICIPANT._serialized_start = 2246
-    _REMOVEPARTICIPANT._serialized_end = 2289
-    _KEEPALIVE._serialized_start = 2291
-    _KEEPALIVE._serialized_end = 2302
-    _ROOMINTERNAL._serialized_start = 2304
-    _ROOMINTERNAL._serialized_end = 2366
+    _NODESTATS._serialized_end = 1682
+    _RTCNODEMESSAGE._serialized_start = 1685
+    _RTCNODEMESSAGE._serialized_end = 2397
+    _SIGNALNODEMESSAGE._serialized_start = 2400
+    _SIGNALNODEMESSAGE._serialized_end = 2542
+    _STARTSESSION._serialized_start = 2545
+    _STARTSESSION._serialized_end = 2933
+    _ENDSESSION._serialized_start = 2935
+    _ENDSESSION._serialized_end = 2947
+    _REMOVEPARTICIPANT._serialized_start = 2949
+    _REMOVEPARTICIPANT._serialized_end = 2992
+    _KEEPALIVE._serialized_start = 2994
+    _KEEPALIVE._serialized_end = 3005
+    _ROOMINTERNAL._serialized_start = 3007
+    _ROOMINTERNAL._serialized_end = 3069
+    _ICECONFIG._serialized_start = 3071
+    _ICECONFIG._serialized_end = 3197
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_internal_pb2.pyi` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_internal_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -9,25 +9,41 @@
 import livekit_rtc_pb2 as _livekit_rtc_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 
 CONTROLLER: NodeType
 DESCRIPTOR: _descriptor.FileDescriptor
+ICT_NONE: ICECandidateType
+ICT_TCP: ICECandidateType
+ICT_TLS: ICECandidateType
 MEDIA: NodeType
 SERVER: NodeType
 SERVING: NodeState
 SHUTTING_DOWN: NodeState
 STARTING_UP: NodeState
+SWEEPER: NodeType
 TURN: NodeType
 
 class EndSession(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
+class ICEConfig(_message.Message):
+    __slots__ = ["preference_publisher", "preference_subscriber"]
+    PREFERENCE_PUBLISHER_FIELD_NUMBER: _ClassVar[int]
+    PREFERENCE_SUBSCRIBER_FIELD_NUMBER: _ClassVar[int]
+    preference_publisher: ICECandidateType
+    preference_subscriber: ICECandidateType
+    def __init__(
+        self,
+        preference_subscriber: _Optional[_Union[ICECandidateType, str]] = ...,
+        preference_publisher: _Optional[_Union[ICECandidateType, str]] = ...,
+    ) -> None: ...
+
 class KeepAlive(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class Node(_message.Message):
     __slots__ = ["id", "ip", "num_cpus", "region", "state", "stats", "type"]
     ID_FIELD_NUMBER: _ClassVar[int]
@@ -62,113 +78,163 @@
         "bytes_out",
         "bytes_out_per_sec",
         "cpu_load",
         "load_avg_last15min",
         "load_avg_last1min",
         "load_avg_last5min",
         "memory_load",
+        "memory_total",
+        "memory_used",
         "nack_per_sec",
         "nack_total",
         "num_clients",
         "num_cpus",
         "num_rooms",
+        "num_track_publish_attempts",
+        "num_track_publish_success",
+        "num_track_subscribe_attempts",
+        "num_track_subscribe_success",
         "num_tracks_in",
         "num_tracks_out",
         "packets_in",
         "packets_in_per_sec",
         "packets_out",
         "packets_out_per_sec",
-        "participant_join",
-        "participant_join_per_sec",
+        "participant_rtc_connected",
+        "participant_rtc_connected_per_sec",
+        "participant_rtc_init",
+        "participant_rtc_init_per_sec",
+        "participant_signal_connected",
+        "participant_signal_connected_per_sec",
         "retransmit_bytes_out",
         "retransmit_bytes_out_per_sec",
         "retransmit_packets_out",
         "retransmit_packets_out_per_sec",
         "started_at",
         "sys_packets_dropped",
         "sys_packets_dropped_pct_per_sec",
         "sys_packets_dropped_per_sec",
         "sys_packets_out",
         "sys_packets_out_per_sec",
+        "track_publish_attempts_per_sec",
+        "track_publish_success_per_sec",
+        "track_subscribe_attempts_per_sec",
+        "track_subscribe_success_per_sec",
         "updated_at",
     ]
     BYTES_IN_FIELD_NUMBER: _ClassVar[int]
     BYTES_IN_PER_SEC_FIELD_NUMBER: _ClassVar[int]
     BYTES_OUT_FIELD_NUMBER: _ClassVar[int]
     BYTES_OUT_PER_SEC_FIELD_NUMBER: _ClassVar[int]
     CPU_LOAD_FIELD_NUMBER: _ClassVar[int]
     LOAD_AVG_LAST15MIN_FIELD_NUMBER: _ClassVar[int]
     LOAD_AVG_LAST1MIN_FIELD_NUMBER: _ClassVar[int]
     LOAD_AVG_LAST5MIN_FIELD_NUMBER: _ClassVar[int]
     MEMORY_LOAD_FIELD_NUMBER: _ClassVar[int]
+    MEMORY_TOTAL_FIELD_NUMBER: _ClassVar[int]
+    MEMORY_USED_FIELD_NUMBER: _ClassVar[int]
     NACK_PER_SEC_FIELD_NUMBER: _ClassVar[int]
     NACK_TOTAL_FIELD_NUMBER: _ClassVar[int]
     NUM_CLIENTS_FIELD_NUMBER: _ClassVar[int]
     NUM_CPUS_FIELD_NUMBER: _ClassVar[int]
     NUM_ROOMS_FIELD_NUMBER: _ClassVar[int]
     NUM_TRACKS_IN_FIELD_NUMBER: _ClassVar[int]
     NUM_TRACKS_OUT_FIELD_NUMBER: _ClassVar[int]
+    NUM_TRACK_PUBLISH_ATTEMPTS_FIELD_NUMBER: _ClassVar[int]
+    NUM_TRACK_PUBLISH_SUCCESS_FIELD_NUMBER: _ClassVar[int]
+    NUM_TRACK_SUBSCRIBE_ATTEMPTS_FIELD_NUMBER: _ClassVar[int]
+    NUM_TRACK_SUBSCRIBE_SUCCESS_FIELD_NUMBER: _ClassVar[int]
     PACKETS_IN_FIELD_NUMBER: _ClassVar[int]
     PACKETS_IN_PER_SEC_FIELD_NUMBER: _ClassVar[int]
     PACKETS_OUT_FIELD_NUMBER: _ClassVar[int]
     PACKETS_OUT_PER_SEC_FIELD_NUMBER: _ClassVar[int]
-    PARTICIPANT_JOIN_FIELD_NUMBER: _ClassVar[int]
-    PARTICIPANT_JOIN_PER_SEC_FIELD_NUMBER: _ClassVar[int]
+    PARTICIPANT_RTC_CONNECTED_FIELD_NUMBER: _ClassVar[int]
+    PARTICIPANT_RTC_CONNECTED_PER_SEC_FIELD_NUMBER: _ClassVar[int]
+    PARTICIPANT_RTC_INIT_FIELD_NUMBER: _ClassVar[int]
+    PARTICIPANT_RTC_INIT_PER_SEC_FIELD_NUMBER: _ClassVar[int]
+    PARTICIPANT_SIGNAL_CONNECTED_FIELD_NUMBER: _ClassVar[int]
+    PARTICIPANT_SIGNAL_CONNECTED_PER_SEC_FIELD_NUMBER: _ClassVar[int]
     RETRANSMIT_BYTES_OUT_FIELD_NUMBER: _ClassVar[int]
     RETRANSMIT_BYTES_OUT_PER_SEC_FIELD_NUMBER: _ClassVar[int]
     RETRANSMIT_PACKETS_OUT_FIELD_NUMBER: _ClassVar[int]
     RETRANSMIT_PACKETS_OUT_PER_SEC_FIELD_NUMBER: _ClassVar[int]
     STARTED_AT_FIELD_NUMBER: _ClassVar[int]
     SYS_PACKETS_DROPPED_FIELD_NUMBER: _ClassVar[int]
     SYS_PACKETS_DROPPED_PCT_PER_SEC_FIELD_NUMBER: _ClassVar[int]
     SYS_PACKETS_DROPPED_PER_SEC_FIELD_NUMBER: _ClassVar[int]
     SYS_PACKETS_OUT_FIELD_NUMBER: _ClassVar[int]
     SYS_PACKETS_OUT_PER_SEC_FIELD_NUMBER: _ClassVar[int]
+    TRACK_PUBLISH_ATTEMPTS_PER_SEC_FIELD_NUMBER: _ClassVar[int]
+    TRACK_PUBLISH_SUCCESS_PER_SEC_FIELD_NUMBER: _ClassVar[int]
+    TRACK_SUBSCRIBE_ATTEMPTS_PER_SEC_FIELD_NUMBER: _ClassVar[int]
+    TRACK_SUBSCRIBE_SUCCESS_PER_SEC_FIELD_NUMBER: _ClassVar[int]
     UPDATED_AT_FIELD_NUMBER: _ClassVar[int]
     bytes_in: int
     bytes_in_per_sec: float
     bytes_out: int
     bytes_out_per_sec: float
     cpu_load: float
     load_avg_last15min: float
     load_avg_last1min: float
     load_avg_last5min: float
     memory_load: float
+    memory_total: int
+    memory_used: int
     nack_per_sec: float
     nack_total: int
     num_clients: int
     num_cpus: int
     num_rooms: int
+    num_track_publish_attempts: int
+    num_track_publish_success: int
+    num_track_subscribe_attempts: int
+    num_track_subscribe_success: int
     num_tracks_in: int
     num_tracks_out: int
     packets_in: int
     packets_in_per_sec: float
     packets_out: int
     packets_out_per_sec: float
-    participant_join: int
-    participant_join_per_sec: float
+    participant_rtc_connected: int
+    participant_rtc_connected_per_sec: float
+    participant_rtc_init: int
+    participant_rtc_init_per_sec: float
+    participant_signal_connected: int
+    participant_signal_connected_per_sec: float
     retransmit_bytes_out: int
     retransmit_bytes_out_per_sec: float
     retransmit_packets_out: int
     retransmit_packets_out_per_sec: float
     started_at: int
     sys_packets_dropped: int
     sys_packets_dropped_pct_per_sec: float
     sys_packets_dropped_per_sec: float
     sys_packets_out: int
     sys_packets_out_per_sec: float
+    track_publish_attempts_per_sec: float
+    track_publish_success_per_sec: float
+    track_subscribe_attempts_per_sec: float
+    track_subscribe_success_per_sec: float
     updated_at: int
     def __init__(
         self,
         started_at: _Optional[int] = ...,
         updated_at: _Optional[int] = ...,
         num_rooms: _Optional[int] = ...,
         num_clients: _Optional[int] = ...,
         num_tracks_in: _Optional[int] = ...,
         num_tracks_out: _Optional[int] = ...,
+        num_track_publish_attempts: _Optional[int] = ...,
+        track_publish_attempts_per_sec: _Optional[float] = ...,
+        num_track_publish_success: _Optional[int] = ...,
+        track_publish_success_per_sec: _Optional[float] = ...,
+        num_track_subscribe_attempts: _Optional[int] = ...,
+        track_subscribe_attempts_per_sec: _Optional[float] = ...,
+        num_track_subscribe_success: _Optional[int] = ...,
+        track_subscribe_success_per_sec: _Optional[float] = ...,
         bytes_in: _Optional[int] = ...,
         bytes_out: _Optional[int] = ...,
         packets_in: _Optional[int] = ...,
         packets_out: _Optional[int] = ...,
         nack_total: _Optional[int] = ...,
         bytes_in_per_sec: _Optional[float] = ...,
         bytes_out_per_sec: _Optional[float] = ...,
@@ -177,74 +243,92 @@
         nack_per_sec: _Optional[float] = ...,
         num_cpus: _Optional[int] = ...,
         load_avg_last1min: _Optional[float] = ...,
         load_avg_last5min: _Optional[float] = ...,
         load_avg_last15min: _Optional[float] = ...,
         cpu_load: _Optional[float] = ...,
         memory_load: _Optional[float] = ...,
+        memory_total: _Optional[int] = ...,
+        memory_used: _Optional[int] = ...,
         sys_packets_out: _Optional[int] = ...,
         sys_packets_dropped: _Optional[int] = ...,
         sys_packets_out_per_sec: _Optional[float] = ...,
         sys_packets_dropped_per_sec: _Optional[float] = ...,
         sys_packets_dropped_pct_per_sec: _Optional[float] = ...,
         retransmit_bytes_out: _Optional[int] = ...,
         retransmit_packets_out: _Optional[int] = ...,
         retransmit_bytes_out_per_sec: _Optional[float] = ...,
         retransmit_packets_out_per_sec: _Optional[float] = ...,
-        participant_join: _Optional[int] = ...,
-        participant_join_per_sec: _Optional[float] = ...,
+        participant_signal_connected: _Optional[int] = ...,
+        participant_signal_connected_per_sec: _Optional[float] = ...,
+        participant_rtc_connected: _Optional[int] = ...,
+        participant_rtc_connected_per_sec: _Optional[float] = ...,
+        participant_rtc_init: _Optional[int] = ...,
+        participant_rtc_init_per_sec: _Optional[float] = ...,
     ) -> None: ...
 
 class RTCNodeMessage(_message.Message):
     __slots__ = [
         "connection_id",
         "delete_room",
+        "identity",
         "keep_alive",
         "mute_track",
         "participant_key",
+        "participant_key_b62",
         "remove_participant",
         "request",
+        "room_name",
         "send_data",
         "sender_time",
         "start_session",
         "update_participant",
         "update_room_metadata",
         "update_subscriptions",
     ]
     CONNECTION_ID_FIELD_NUMBER: _ClassVar[int]
     DELETE_ROOM_FIELD_NUMBER: _ClassVar[int]
+    IDENTITY_FIELD_NUMBER: _ClassVar[int]
     KEEP_ALIVE_FIELD_NUMBER: _ClassVar[int]
     MUTE_TRACK_FIELD_NUMBER: _ClassVar[int]
+    PARTICIPANT_KEY_B62_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_KEY_FIELD_NUMBER: _ClassVar[int]
     REMOVE_PARTICIPANT_FIELD_NUMBER: _ClassVar[int]
     REQUEST_FIELD_NUMBER: _ClassVar[int]
+    ROOM_NAME_FIELD_NUMBER: _ClassVar[int]
     SENDER_TIME_FIELD_NUMBER: _ClassVar[int]
     SEND_DATA_FIELD_NUMBER: _ClassVar[int]
     START_SESSION_FIELD_NUMBER: _ClassVar[int]
     UPDATE_PARTICIPANT_FIELD_NUMBER: _ClassVar[int]
     UPDATE_ROOM_METADATA_FIELD_NUMBER: _ClassVar[int]
     UPDATE_SUBSCRIPTIONS_FIELD_NUMBER: _ClassVar[int]
     connection_id: str
     delete_room: _livekit_room_pb2.DeleteRoomRequest
+    identity: str
     keep_alive: KeepAlive
     mute_track: _livekit_room_pb2.MuteRoomTrackRequest
     participant_key: str
+    participant_key_b62: str
     remove_participant: _livekit_room_pb2.RoomParticipantIdentity
     request: _livekit_rtc_pb2.SignalRequest
+    room_name: str
     send_data: _livekit_room_pb2.SendDataRequest
     sender_time: int
     start_session: StartSession
     update_participant: _livekit_room_pb2.UpdateParticipantRequest
     update_room_metadata: _livekit_room_pb2.UpdateRoomMetadataRequest
     update_subscriptions: _livekit_room_pb2.UpdateSubscriptionsRequest
     def __init__(
         self,
         participant_key: _Optional[str] = ...,
         sender_time: _Optional[int] = ...,
         connection_id: _Optional[str] = ...,
+        participant_key_b62: _Optional[str] = ...,
+        room_name: _Optional[str] = ...,
+        identity: _Optional[str] = ...,
         start_session: _Optional[_Union[StartSession, _Mapping]] = ...,
         request: _Optional[_Union[_livekit_rtc_pb2.SignalRequest, _Mapping]] = ...,
         remove_participant: _Optional[
             _Union[_livekit_room_pb2.RoomParticipantIdentity, _Mapping]
         ] = ...,
         mute_track: _Optional[
             _Union[_livekit_room_pb2.MuteRoomTrackRequest, _Mapping]
@@ -305,55 +389,68 @@
         "connection_id",
         "grants_json",
         "hidden",
         "identity",
         "name",
         "participant_id",
         "reconnect",
+        "reconnect_reason",
         "recorder",
         "room_name",
+        "subscriber_allow_pause",
     ]
     ADAPTIVE_STREAM_FIELD_NUMBER: _ClassVar[int]
     AUTO_SUBSCRIBE_FIELD_NUMBER: _ClassVar[int]
     CLIENT_FIELD_NUMBER: _ClassVar[int]
     CONNECTION_ID_FIELD_NUMBER: _ClassVar[int]
     GRANTS_JSON_FIELD_NUMBER: _ClassVar[int]
     HIDDEN_FIELD_NUMBER: _ClassVar[int]
     IDENTITY_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_ID_FIELD_NUMBER: _ClassVar[int]
     RECONNECT_FIELD_NUMBER: _ClassVar[int]
+    RECONNECT_REASON_FIELD_NUMBER: _ClassVar[int]
     RECORDER_FIELD_NUMBER: _ClassVar[int]
     ROOM_NAME_FIELD_NUMBER: _ClassVar[int]
+    SUBSCRIBER_ALLOW_PAUSE_FIELD_NUMBER: _ClassVar[int]
     adaptive_stream: bool
     auto_subscribe: bool
     client: _livekit_models_pb2.ClientInfo
     connection_id: str
     grants_json: str
     hidden: bool
     identity: str
     name: str
     participant_id: str
     reconnect: bool
+    reconnect_reason: _livekit_models_pb2.ReconnectReason
     recorder: bool
     room_name: str
+    subscriber_allow_pause: bool
     def __init__(
         self,
         room_name: _Optional[str] = ...,
         identity: _Optional[str] = ...,
         connection_id: _Optional[str] = ...,
         reconnect: bool = ...,
         auto_subscribe: bool = ...,
         hidden: bool = ...,
         client: _Optional[_Union[_livekit_models_pb2.ClientInfo, _Mapping]] = ...,
         recorder: bool = ...,
         name: _Optional[str] = ...,
         grants_json: _Optional[str] = ...,
         adaptive_stream: bool = ...,
         participant_id: _Optional[str] = ...,
+        reconnect_reason: _Optional[
+            _Union[_livekit_models_pb2.ReconnectReason, str]
+        ] = ...,
+        subscriber_allow_pause: bool = ...,
     ) -> None: ...
 
 class NodeType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
 class NodeState(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
+
+class ICECandidateType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_models_pb2.py` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_models_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,79 +11,88 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x14livekit_models.proto\x12\x07livekit\x1a\x1fgoogle/protobuf/timestamp.proto"\xee\x01\n\x04Room\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rempty_timeout\x18\x03 \x01(\r\x12\x18\n\x10max_participants\x18\x04 \x01(\r\x12\x15\n\rcreation_time\x18\x05 \x01(\x03\x12\x15\n\rturn_password\x18\x06 \x01(\t\x12&\n\x0e\x65nabled_codecs\x18\x07 \x03(\x0b\x32\x0e.livekit.Codec\x12\x10\n\x08metadata\x18\x08 \x01(\t\x12\x18\n\x10num_participants\x18\t \x01(\r\x12\x18\n\x10\x61\x63tive_recording\x18\n \x01(\x08"(\n\x05\x43odec\x12\x0c\n\x04mime\x18\x01 \x01(\t\x12\x11\n\tfmtp_line\x18\x02 \x01(\t"\x7f\n\x15ParticipantPermission\x12\x15\n\rcan_subscribe\x18\x01 \x01(\x08\x12\x13\n\x0b\x63\x61n_publish\x18\x02 \x01(\x08\x12\x18\n\x10\x63\x61n_publish_data\x18\x03 \x01(\x08\x12\x0e\n\x06hidden\x18\x07 \x01(\x08\x12\x10\n\x08recorder\x18\x08 \x01(\x08"\xe1\x02\n\x0fParticipantInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12-\n\x05state\x18\x03 \x01(\x0e\x32\x1e.livekit.ParticipantInfo.State\x12"\n\x06tracks\x18\x04 \x03(\x0b\x32\x12.livekit.TrackInfo\x12\x10\n\x08metadata\x18\x05 \x01(\t\x12\x11\n\tjoined_at\x18\x06 \x01(\x03\x12\x0c\n\x04name\x18\t \x01(\t\x12\x0f\n\x07version\x18\n \x01(\r\x12\x32\n\npermission\x18\x0b \x01(\x0b\x32\x1e.livekit.ParticipantPermission\x12\x0e\n\x06region\x18\x0c \x01(\t\x12\x14\n\x0cis_publisher\x18\r \x01(\x08">\n\x05State\x12\x0b\n\x07JOINING\x10\x00\x12\n\n\x06JOINED\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x10\n\x0c\x44ISCONNECTED\x10\x03"f\n\x12SimulcastCodecInfo\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x0b\n\x03mid\x18\x02 \x01(\t\x12\x0b\n\x03\x63id\x18\x03 \x01(\t\x12#\n\x06layers\x18\x04 \x03(\x0b\x32\x13.livekit.VideoLayer"\xdb\x02\n\tTrackInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12 \n\x04type\x18\x02 \x01(\x0e\x32\x12.livekit.TrackType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05muted\x18\x04 \x01(\x08\x12\r\n\x05width\x18\x05 \x01(\r\x12\x0e\n\x06height\x18\x06 \x01(\r\x12\x11\n\tsimulcast\x18\x07 \x01(\x08\x12\x13\n\x0b\x64isable_dtx\x18\x08 \x01(\x08\x12$\n\x06source\x18\t \x01(\x0e\x32\x14.livekit.TrackSource\x12#\n\x06layers\x18\n \x03(\x0b\x32\x13.livekit.VideoLayer\x12\x11\n\tmime_type\x18\x0b \x01(\t\x12\x0b\n\x03mid\x18\x0c \x01(\t\x12+\n\x06\x63odecs\x18\r \x03(\x0b\x32\x1b.livekit.SimulcastCodecInfo\x12\x0e\n\x06stereo\x18\x0e \x01(\x08\x12\x13\n\x0b\x64isable_red\x18\x0f \x01(\x08"r\n\nVideoLayer\x12&\n\x07quality\x18\x01 \x01(\x0e\x32\x15.livekit.VideoQuality\x12\r\n\x05width\x18\x02 \x01(\r\x12\x0e\n\x06height\x18\x03 \x01(\r\x12\x0f\n\x07\x62itrate\x18\x04 \x01(\r\x12\x0c\n\x04ssrc\x18\x05 \x01(\r"\xb4\x01\n\nDataPacket\x12&\n\x04kind\x18\x01 \x01(\x0e\x32\x18.livekit.DataPacket.Kind\x12#\n\x04user\x18\x02 \x01(\x0b\x32\x13.livekit.UserPacketH\x00\x12/\n\x07speaker\x18\x03 \x01(\x0b\x32\x1c.livekit.ActiveSpeakerUpdateH\x00"\x1f\n\x04Kind\x12\x0c\n\x08RELIABLE\x10\x00\x12\t\n\x05LOSSY\x10\x01\x42\x07\n\x05value"=\n\x13\x41\x63tiveSpeakerUpdate\x12&\n\x08speakers\x18\x01 \x03(\x0b\x32\x14.livekit.SpeakerInfo"9\n\x0bSpeakerInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\r\n\x05level\x18\x02 \x01(\x02\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08"P\n\nUserPacket\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x18\n\x10\x64\x65stination_sids\x18\x03 \x03(\t"@\n\x11ParticipantTracks\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12\x12\n\ntrack_sids\x18\x02 \x03(\t"\xb6\x01\n\nServerInfo\x12,\n\x07\x65\x64ition\x18\x01 \x01(\x0e\x32\x1b.livekit.ServerInfo.Edition\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08protocol\x18\x03 \x01(\x05\x12\x0e\n\x06region\x18\x04 \x01(\t\x12\x0f\n\x07node_id\x18\x05 \x01(\t\x12\x12\n\ndebug_info\x18\x06 \x01(\t""\n\x07\x45\x64ition\x12\x0c\n\x08Standard\x10\x00\x12\t\n\x05\x43loud\x10\x01"\xab\x02\n\nClientInfo\x12$\n\x03sdk\x18\x01 \x01(\x0e\x32\x17.livekit.ClientInfo.SDK\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08protocol\x18\x03 \x01(\x05\x12\n\n\x02os\x18\x04 \x01(\t\x12\x12\n\nos_version\x18\x05 \x01(\t\x12\x14\n\x0c\x64\x65vice_model\x18\x06 \x01(\t\x12\x0f\n\x07\x62rowser\x18\x07 \x01(\t\x12\x17\n\x0f\x62rowser_version\x18\x08 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\t \x01(\t\x12\x0f\n\x07network\x18\n \x01(\t"R\n\x03SDK\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x06\n\x02JS\x10\x01\x12\t\n\x05SWIFT\x10\x02\x12\x0b\n\x07\x41NDROID\x10\x03\x12\x0b\n\x07\x46LUTTER\x10\x04\x12\x06\n\x02GO\x10\x05\x12\t\n\x05UNITY\x10\x06"\x8c\x02\n\x13\x43lientConfiguration\x12*\n\x05video\x18\x01 \x01(\x0b\x32\x1b.livekit.VideoConfiguration\x12+\n\x06screen\x18\x02 \x01(\x0b\x32\x1b.livekit.VideoConfiguration\x12\x37\n\x11resume_connection\x18\x03 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting\x12\x30\n\x0f\x64isabled_codecs\x18\x04 \x01(\x0b\x32\x17.livekit.DisabledCodecs\x12\x31\n\x0b\x66orce_relay\x18\x05 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting"L\n\x12VideoConfiguration\x12\x36\n\x10hardware_encoder\x18\x01 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting"0\n\x0e\x44isabledCodecs\x12\x1e\n\x06\x63odecs\x18\x01 \x03(\x0b\x32\x0e.livekit.Codec"\x9d\t\n\x08RTPStats\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12\x0f\n\x07packets\x18\x04 \x01(\r\x12\x13\n\x0bpacket_rate\x18\x05 \x01(\x01\x12\r\n\x05\x62ytes\x18\x06 \x01(\x04\x12\x14\n\x0cheader_bytes\x18\' \x01(\x04\x12\x0f\n\x07\x62itrate\x18\x07 \x01(\x01\x12\x14\n\x0cpackets_lost\x18\x08 \x01(\r\x12\x18\n\x10packet_loss_rate\x18\t \x01(\x01\x12\x1e\n\x16packet_loss_percentage\x18\n \x01(\x02\x12\x19\n\x11packets_duplicate\x18\x0b \x01(\r\x12\x1d\n\x15packet_duplicate_rate\x18\x0c \x01(\x01\x12\x17\n\x0f\x62ytes_duplicate\x18\r \x01(\x04\x12\x1e\n\x16header_bytes_duplicate\x18( \x01(\x04\x12\x19\n\x11\x62itrate_duplicate\x18\x0e \x01(\x01\x12\x17\n\x0fpackets_padding\x18\x0f \x01(\r\x12\x1b\n\x13packet_padding_rate\x18\x10 \x01(\x01\x12\x15\n\rbytes_padding\x18\x11 \x01(\x04\x12\x1c\n\x14header_bytes_padding\x18) \x01(\x04\x12\x17\n\x0f\x62itrate_padding\x18\x12 \x01(\x01\x12\x1c\n\x14packets_out_of_order\x18\x13 \x01(\r\x12\x0e\n\x06\x66rames\x18\x14 \x01(\r\x12\x12\n\nframe_rate\x18\x15 \x01(\x01\x12\x16\n\x0ejitter_current\x18\x16 \x01(\x01\x12\x12\n\njitter_max\x18\x17 \x01(\x01\x12:\n\rgap_histogram\x18\x18 \x03(\x0b\x32#.livekit.RTPStats.GapHistogramEntry\x12\r\n\x05nacks\x18\x19 \x01(\r\x12\x11\n\tnack_acks\x18% \x01(\r\x12\x13\n\x0bnack_misses\x18\x1a \x01(\r\x12\x15\n\rnack_repeated\x18& \x01(\r\x12\x0c\n\x04plis\x18\x1b \x01(\r\x12,\n\x08last_pli\x18\x1c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04\x66irs\x18\x1d \x01(\r\x12,\n\x08last_fir\x18\x1e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0brtt_current\x18\x1f \x01(\r\x12\x0f\n\x07rtt_max\x18  \x01(\r\x12\x12\n\nkey_frames\x18! \x01(\r\x12\x32\n\x0elast_key_frame\x18" \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0flayer_lock_plis\x18# \x01(\r\x12\x37\n\x13last_layer_lock_pli\x18$ \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a\x33\n\x11GapHistogramEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01"1\n\x0cTimedVersion\x12\x12\n\nunix_micro\x18\x01 \x01(\x03\x12\r\n\x05ticks\x18\x02 \x01(\x05*+\n\tTrackType\x12\t\n\x05\x41UDIO\x10\x00\x12\t\n\x05VIDEO\x10\x01\x12\x08\n\x04\x44\x41TA\x10\x02*`\n\x0bTrackSource\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06\x43\x41MERA\x10\x01\x12\x0e\n\nMICROPHONE\x10\x02\x12\x10\n\x0cSCREEN_SHARE\x10\x03\x12\x16\n\x12SCREEN_SHARE_AUDIO\x10\x04*6\n\x0cVideoQuality\x12\x07\n\x03LOW\x10\x00\x12\n\n\x06MEDIUM\x10\x01\x12\x08\n\x04HIGH\x10\x02\x12\x07\n\x03OFF\x10\x03*6\n\x11\x43onnectionQuality\x12\x08\n\x04POOR\x10\x00\x12\x08\n\x04GOOD\x10\x01\x12\r\n\tEXCELLENT\x10\x02*;\n\x13\x43lientConfigSetting\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x44ISABLED\x10\x01\x12\x0b\n\x07\x45NABLED\x10\x02*\xba\x01\n\x10\x44isconnectReason\x12\x12\n\x0eUNKNOWN_REASON\x10\x00\x12\x14\n\x10\x43LIENT_INITIATED\x10\x01\x12\x16\n\x12\x44UPLICATE_IDENTITY\x10\x02\x12\x13\n\x0fSERVER_SHUTDOWN\x10\x03\x12\x17\n\x13PARTICIPANT_REMOVED\x10\x04\x12\x10\n\x0cROOM_DELETED\x10\x05\x12\x12\n\x0eSTATE_MISMATCH\x10\x06\x12\x10\n\x0cJOIN_FAILURE\x10\x07\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
+    b'\n\x14livekit_models.proto\x12\x07livekit\x1a\x1fgoogle/protobuf/timestamp.proto"\xee\x01\n\x04Room\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rempty_timeout\x18\x03 \x01(\r\x12\x18\n\x10max_participants\x18\x04 \x01(\r\x12\x15\n\rcreation_time\x18\x05 \x01(\x03\x12\x15\n\rturn_password\x18\x06 \x01(\t\x12&\n\x0e\x65nabled_codecs\x18\x07 \x03(\x0b\x32\x0e.livekit.Codec\x12\x10\n\x08metadata\x18\x08 \x01(\t\x12\x18\n\x10num_participants\x18\t \x01(\r\x12\x18\n\x10\x61\x63tive_recording\x18\n \x01(\x08"(\n\x05\x43odec\x12\x0c\n\x04mime\x18\x01 \x01(\t\x12\x11\n\tfmtp_line\x18\x02 \x01(\t"\xcf\x01\n\x15ParticipantPermission\x12\x15\n\rcan_subscribe\x18\x01 \x01(\x08\x12\x13\n\x0b\x63\x61n_publish\x18\x02 \x01(\x08\x12\x18\n\x10\x63\x61n_publish_data\x18\x03 \x01(\x08\x12\x31\n\x13\x63\x61n_publish_sources\x18\t \x03(\x0e\x32\x14.livekit.TrackSource\x12\x0e\n\x06hidden\x18\x07 \x01(\x08\x12\x10\n\x08recorder\x18\x08 \x01(\x08\x12\x1b\n\x13\x63\x61n_update_metadata\x18\n \x01(\x08"\xe1\x02\n\x0fParticipantInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12-\n\x05state\x18\x03 \x01(\x0e\x32\x1e.livekit.ParticipantInfo.State\x12"\n\x06tracks\x18\x04 \x03(\x0b\x32\x12.livekit.TrackInfo\x12\x10\n\x08metadata\x18\x05 \x01(\t\x12\x11\n\tjoined_at\x18\x06 \x01(\x03\x12\x0c\n\x04name\x18\t \x01(\t\x12\x0f\n\x07version\x18\n \x01(\r\x12\x32\n\npermission\x18\x0b \x01(\x0b\x32\x1e.livekit.ParticipantPermission\x12\x0e\n\x06region\x18\x0c \x01(\t\x12\x14\n\x0cis_publisher\x18\r \x01(\x08">\n\x05State\x12\x0b\n\x07JOINING\x10\x00\x12\n\n\x06JOINED\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x10\n\x0c\x44ISCONNECTED\x10\x03"3\n\nEncryption"%\n\x04Type\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03GCM\x10\x01\x12\n\n\x06\x43USTOM\x10\x02"f\n\x12SimulcastCodecInfo\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x0b\n\x03mid\x18\x02 \x01(\t\x12\x0b\n\x03\x63id\x18\x03 \x01(\t\x12#\n\x06layers\x18\x04 \x03(\x0b\x32\x13.livekit.VideoLayer"\x89\x03\n\tTrackInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12 \n\x04type\x18\x02 \x01(\x0e\x32\x12.livekit.TrackType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05muted\x18\x04 \x01(\x08\x12\r\n\x05width\x18\x05 \x01(\r\x12\x0e\n\x06height\x18\x06 \x01(\r\x12\x11\n\tsimulcast\x18\x07 \x01(\x08\x12\x13\n\x0b\x64isable_dtx\x18\x08 \x01(\x08\x12$\n\x06source\x18\t \x01(\x0e\x32\x14.livekit.TrackSource\x12#\n\x06layers\x18\n \x03(\x0b\x32\x13.livekit.VideoLayer\x12\x11\n\tmime_type\x18\x0b \x01(\t\x12\x0b\n\x03mid\x18\x0c \x01(\t\x12+\n\x06\x63odecs\x18\r \x03(\x0b\x32\x1b.livekit.SimulcastCodecInfo\x12\x0e\n\x06stereo\x18\x0e \x01(\x08\x12\x13\n\x0b\x64isable_red\x18\x0f \x01(\x08\x12,\n\nencryption\x18\x10 \x01(\x0e\x32\x18.livekit.Encryption.Type"r\n\nVideoLayer\x12&\n\x07quality\x18\x01 \x01(\x0e\x32\x15.livekit.VideoQuality\x12\r\n\x05width\x18\x02 \x01(\r\x12\x0e\n\x06height\x18\x03 \x01(\r\x12\x0f\n\x07\x62itrate\x18\x04 \x01(\r\x12\x0c\n\x04ssrc\x18\x05 \x01(\r"\xb4\x01\n\nDataPacket\x12&\n\x04kind\x18\x01 \x01(\x0e\x32\x18.livekit.DataPacket.Kind\x12#\n\x04user\x18\x02 \x01(\x0b\x32\x13.livekit.UserPacketH\x00\x12/\n\x07speaker\x18\x03 \x01(\x0b\x32\x1c.livekit.ActiveSpeakerUpdateH\x00"\x1f\n\x04Kind\x12\x0c\n\x08RELIABLE\x10\x00\x12\t\n\x05LOSSY\x10\x01\x42\x07\n\x05value"=\n\x13\x41\x63tiveSpeakerUpdate\x12&\n\x08speakers\x18\x01 \x03(\x0b\x32\x14.livekit.SpeakerInfo"9\n\x0bSpeakerInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\r\n\x05level\x18\x02 \x01(\x02\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08"n\n\nUserPacket\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x18\n\x10\x64\x65stination_sids\x18\x03 \x03(\t\x12\x12\n\x05topic\x18\x04 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_topic"@\n\x11ParticipantTracks\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12\x12\n\ntrack_sids\x18\x02 \x03(\t"\xb6\x01\n\nServerInfo\x12,\n\x07\x65\x64ition\x18\x01 \x01(\x0e\x32\x1b.livekit.ServerInfo.Edition\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08protocol\x18\x03 \x01(\x05\x12\x0e\n\x06region\x18\x04 \x01(\t\x12\x0f\n\x07node_id\x18\x05 \x01(\t\x12\x12\n\ndebug_info\x18\x06 \x01(\t""\n\x07\x45\x64ition\x12\x0c\n\x08Standard\x10\x00\x12\t\n\x05\x43loud\x10\x01"\xc7\x02\n\nClientInfo\x12$\n\x03sdk\x18\x01 \x01(\x0e\x32\x17.livekit.ClientInfo.SDK\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08protocol\x18\x03 \x01(\x05\x12\n\n\x02os\x18\x04 \x01(\t\x12\x12\n\nos_version\x18\x05 \x01(\t\x12\x14\n\x0c\x64\x65vice_model\x18\x06 \x01(\t\x12\x0f\n\x07\x62rowser\x18\x07 \x01(\t\x12\x17\n\x0f\x62rowser_version\x18\x08 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\t \x01(\t\x12\x0f\n\x07network\x18\n \x01(\t"n\n\x03SDK\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x06\n\x02JS\x10\x01\x12\t\n\x05SWIFT\x10\x02\x12\x0b\n\x07\x41NDROID\x10\x03\x12\x0b\n\x07\x46LUTTER\x10\x04\x12\x06\n\x02GO\x10\x05\x12\t\n\x05UNITY\x10\x06\x12\x10\n\x0cREACT_NATIVE\x10\x07\x12\x08\n\x04RUST\x10\x08"\x8c\x02\n\x13\x43lientConfiguration\x12*\n\x05video\x18\x01 \x01(\x0b\x32\x1b.livekit.VideoConfiguration\x12+\n\x06screen\x18\x02 \x01(\x0b\x32\x1b.livekit.VideoConfiguration\x12\x37\n\x11resume_connection\x18\x03 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting\x12\x30\n\x0f\x64isabled_codecs\x18\x04 \x01(\x0b\x32\x17.livekit.DisabledCodecs\x12\x31\n\x0b\x66orce_relay\x18\x05 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting"L\n\x12VideoConfiguration\x12\x36\n\x10hardware_encoder\x18\x01 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting"0\n\x0e\x44isabledCodecs\x12\x1e\n\x06\x63odecs\x18\x01 \x03(\x0b\x32\x0e.livekit.Codec"\x9d\t\n\x08RTPStats\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12\x0f\n\x07packets\x18\x04 \x01(\r\x12\x13\n\x0bpacket_rate\x18\x05 \x01(\x01\x12\r\n\x05\x62ytes\x18\x06 \x01(\x04\x12\x14\n\x0cheader_bytes\x18\' \x01(\x04\x12\x0f\n\x07\x62itrate\x18\x07 \x01(\x01\x12\x14\n\x0cpackets_lost\x18\x08 \x01(\r\x12\x18\n\x10packet_loss_rate\x18\t \x01(\x01\x12\x1e\n\x16packet_loss_percentage\x18\n \x01(\x02\x12\x19\n\x11packets_duplicate\x18\x0b \x01(\r\x12\x1d\n\x15packet_duplicate_rate\x18\x0c \x01(\x01\x12\x17\n\x0f\x62ytes_duplicate\x18\r \x01(\x04\x12\x1e\n\x16header_bytes_duplicate\x18( \x01(\x04\x12\x19\n\x11\x62itrate_duplicate\x18\x0e \x01(\x01\x12\x17\n\x0fpackets_padding\x18\x0f \x01(\r\x12\x1b\n\x13packet_padding_rate\x18\x10 \x01(\x01\x12\x15\n\rbytes_padding\x18\x11 \x01(\x04\x12\x1c\n\x14header_bytes_padding\x18) \x01(\x04\x12\x17\n\x0f\x62itrate_padding\x18\x12 \x01(\x01\x12\x1c\n\x14packets_out_of_order\x18\x13 \x01(\r\x12\x0e\n\x06\x66rames\x18\x14 \x01(\r\x12\x12\n\nframe_rate\x18\x15 \x01(\x01\x12\x16\n\x0ejitter_current\x18\x16 \x01(\x01\x12\x12\n\njitter_max\x18\x17 \x01(\x01\x12:\n\rgap_histogram\x18\x18 \x03(\x0b\x32#.livekit.RTPStats.GapHistogramEntry\x12\r\n\x05nacks\x18\x19 \x01(\r\x12\x11\n\tnack_acks\x18% \x01(\r\x12\x13\n\x0bnack_misses\x18\x1a \x01(\r\x12\x15\n\rnack_repeated\x18& \x01(\r\x12\x0c\n\x04plis\x18\x1b \x01(\r\x12,\n\x08last_pli\x18\x1c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04\x66irs\x18\x1d \x01(\r\x12,\n\x08last_fir\x18\x1e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0brtt_current\x18\x1f \x01(\r\x12\x0f\n\x07rtt_max\x18  \x01(\r\x12\x12\n\nkey_frames\x18! \x01(\r\x12\x32\n\x0elast_key_frame\x18" \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0flayer_lock_plis\x18# \x01(\r\x12\x37\n\x13last_layer_lock_pli\x18$ \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a\x33\n\x11GapHistogramEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01"1\n\x0cTimedVersion\x12\x12\n\nunix_micro\x18\x01 \x01(\x03\x12\r\n\x05ticks\x18\x02 \x01(\x05*/\n\nAudioCodec\x12\x0e\n\nDEFAULT_AC\x10\x00\x12\x08\n\x04OPUS\x10\x01\x12\x07\n\x03\x41\x41\x43\x10\x02*V\n\nVideoCodec\x12\x0e\n\nDEFAULT_VC\x10\x00\x12\x11\n\rH264_BASELINE\x10\x01\x12\r\n\tH264_MAIN\x10\x02\x12\r\n\tH264_HIGH\x10\x03\x12\x07\n\x03VP8\x10\x04*+\n\tTrackType\x12\t\n\x05\x41UDIO\x10\x00\x12\t\n\x05VIDEO\x10\x01\x12\x08\n\x04\x44\x41TA\x10\x02*`\n\x0bTrackSource\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06\x43\x41MERA\x10\x01\x12\x0e\n\nMICROPHONE\x10\x02\x12\x10\n\x0cSCREEN_SHARE\x10\x03\x12\x16\n\x12SCREEN_SHARE_AUDIO\x10\x04*6\n\x0cVideoQuality\x12\x07\n\x03LOW\x10\x00\x12\n\n\x06MEDIUM\x10\x01\x12\x08\n\x04HIGH\x10\x02\x12\x07\n\x03OFF\x10\x03*6\n\x11\x43onnectionQuality\x12\x08\n\x04POOR\x10\x00\x12\x08\n\x04GOOD\x10\x01\x12\r\n\tEXCELLENT\x10\x02*;\n\x13\x43lientConfigSetting\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x44ISABLED\x10\x01\x12\x0b\n\x07\x45NABLED\x10\x02*\xba\x01\n\x10\x44isconnectReason\x12\x12\n\x0eUNKNOWN_REASON\x10\x00\x12\x14\n\x10\x43LIENT_INITIATED\x10\x01\x12\x16\n\x12\x44UPLICATE_IDENTITY\x10\x02\x12\x13\n\x0fSERVER_SHUTDOWN\x10\x03\x12\x17\n\x13PARTICIPANT_REMOVED\x10\x04\x12\x10\n\x0cROOM_DELETED\x10\x05\x12\x12\n\x0eSTATE_MISMATCH\x10\x06\x12\x10\n\x0cJOIN_FAILURE\x10\x07*\x88\x01\n\x0fReconnectReason\x12\r\n\tRR_UNKOWN\x10\x00\x12\x1a\n\x16RR_SIGNAL_DISCONNECTED\x10\x01\x12\x17\n\x13RR_PUBLISHER_FAILED\x10\x02\x12\x18\n\x14RR_SUBSCRIBER_FAILED\x10\x03\x12\x17\n\x13RR_SWITCH_CANDIDATE\x10\x04\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "livekit_models_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto"
     _RTPSTATS_GAPHISTOGRAMENTRY._options = None
     _RTPSTATS_GAPHISTOGRAMENTRY._serialized_options = b"8\001"
-    _TRACKTYPE._serialized_start = 3978
-    _TRACKTYPE._serialized_end = 4021
-    _TRACKSOURCE._serialized_start = 4023
-    _TRACKSOURCE._serialized_end = 4119
-    _VIDEOQUALITY._serialized_start = 4121
-    _VIDEOQUALITY._serialized_end = 4175
-    _CONNECTIONQUALITY._serialized_start = 4177
-    _CONNECTIONQUALITY._serialized_end = 4231
-    _CLIENTCONFIGSETTING._serialized_start = 4233
-    _CLIENTCONFIGSETTING._serialized_end = 4292
-    _DISCONNECTREASON._serialized_start = 4295
-    _DISCONNECTREASON._serialized_end = 4481
+    _AUDIOCODEC._serialized_start = 4216
+    _AUDIOCODEC._serialized_end = 4263
+    _VIDEOCODEC._serialized_start = 4265
+    _VIDEOCODEC._serialized_end = 4351
+    _TRACKTYPE._serialized_start = 4353
+    _TRACKTYPE._serialized_end = 4396
+    _TRACKSOURCE._serialized_start = 4398
+    _TRACKSOURCE._serialized_end = 4494
+    _VIDEOQUALITY._serialized_start = 4496
+    _VIDEOQUALITY._serialized_end = 4550
+    _CONNECTIONQUALITY._serialized_start = 4552
+    _CONNECTIONQUALITY._serialized_end = 4606
+    _CLIENTCONFIGSETTING._serialized_start = 4608
+    _CLIENTCONFIGSETTING._serialized_end = 4667
+    _DISCONNECTREASON._serialized_start = 4670
+    _DISCONNECTREASON._serialized_end = 4856
+    _RECONNECTREASON._serialized_start = 4859
+    _RECONNECTREASON._serialized_end = 4995
     _ROOM._serialized_start = 67
     _ROOM._serialized_end = 305
     _CODEC._serialized_start = 307
     _CODEC._serialized_end = 347
-    _PARTICIPANTPERMISSION._serialized_start = 349
-    _PARTICIPANTPERMISSION._serialized_end = 476
-    _PARTICIPANTINFO._serialized_start = 479
-    _PARTICIPANTINFO._serialized_end = 832
-    _PARTICIPANTINFO_STATE._serialized_start = 770
-    _PARTICIPANTINFO_STATE._serialized_end = 832
-    _SIMULCASTCODECINFO._serialized_start = 834
-    _SIMULCASTCODECINFO._serialized_end = 936
-    _TRACKINFO._serialized_start = 939
-    _TRACKINFO._serialized_end = 1286
-    _VIDEOLAYER._serialized_start = 1288
-    _VIDEOLAYER._serialized_end = 1402
-    _DATAPACKET._serialized_start = 1405
-    _DATAPACKET._serialized_end = 1585
-    _DATAPACKET_KIND._serialized_start = 1545
-    _DATAPACKET_KIND._serialized_end = 1576
-    _ACTIVESPEAKERUPDATE._serialized_start = 1587
-    _ACTIVESPEAKERUPDATE._serialized_end = 1648
-    _SPEAKERINFO._serialized_start = 1650
-    _SPEAKERINFO._serialized_end = 1707
-    _USERPACKET._serialized_start = 1709
-    _USERPACKET._serialized_end = 1789
-    _PARTICIPANTTRACKS._serialized_start = 1791
-    _PARTICIPANTTRACKS._serialized_end = 1855
-    _SERVERINFO._serialized_start = 1858
-    _SERVERINFO._serialized_end = 2040
-    _SERVERINFO_EDITION._serialized_start = 2006
-    _SERVERINFO_EDITION._serialized_end = 2040
-    _CLIENTINFO._serialized_start = 2043
-    _CLIENTINFO._serialized_end = 2342
-    _CLIENTINFO_SDK._serialized_start = 2260
-    _CLIENTINFO_SDK._serialized_end = 2342
-    _CLIENTCONFIGURATION._serialized_start = 2345
-    _CLIENTCONFIGURATION._serialized_end = 2613
-    _VIDEOCONFIGURATION._serialized_start = 2615
-    _VIDEOCONFIGURATION._serialized_end = 2691
-    _DISABLEDCODECS._serialized_start = 2693
-    _DISABLEDCODECS._serialized_end = 2741
-    _RTPSTATS._serialized_start = 2744
-    _RTPSTATS._serialized_end = 3925
-    _RTPSTATS_GAPHISTOGRAMENTRY._serialized_start = 3874
-    _RTPSTATS_GAPHISTOGRAMENTRY._serialized_end = 3925
-    _TIMEDVERSION._serialized_start = 3927
-    _TIMEDVERSION._serialized_end = 3976
+    _PARTICIPANTPERMISSION._serialized_start = 350
+    _PARTICIPANTPERMISSION._serialized_end = 557
+    _PARTICIPANTINFO._serialized_start = 560
+    _PARTICIPANTINFO._serialized_end = 913
+    _PARTICIPANTINFO_STATE._serialized_start = 851
+    _PARTICIPANTINFO_STATE._serialized_end = 913
+    _ENCRYPTION._serialized_start = 915
+    _ENCRYPTION._serialized_end = 966
+    _ENCRYPTION_TYPE._serialized_start = 929
+    _ENCRYPTION_TYPE._serialized_end = 966
+    _SIMULCASTCODECINFO._serialized_start = 968
+    _SIMULCASTCODECINFO._serialized_end = 1070
+    _TRACKINFO._serialized_start = 1073
+    _TRACKINFO._serialized_end = 1466
+    _VIDEOLAYER._serialized_start = 1468
+    _VIDEOLAYER._serialized_end = 1582
+    _DATAPACKET._serialized_start = 1585
+    _DATAPACKET._serialized_end = 1765
+    _DATAPACKET_KIND._serialized_start = 1725
+    _DATAPACKET_KIND._serialized_end = 1756
+    _ACTIVESPEAKERUPDATE._serialized_start = 1767
+    _ACTIVESPEAKERUPDATE._serialized_end = 1828
+    _SPEAKERINFO._serialized_start = 1830
+    _SPEAKERINFO._serialized_end = 1887
+    _USERPACKET._serialized_start = 1889
+    _USERPACKET._serialized_end = 1999
+    _PARTICIPANTTRACKS._serialized_start = 2001
+    _PARTICIPANTTRACKS._serialized_end = 2065
+    _SERVERINFO._serialized_start = 2068
+    _SERVERINFO._serialized_end = 2250
+    _SERVERINFO_EDITION._serialized_start = 2216
+    _SERVERINFO_EDITION._serialized_end = 2250
+    _CLIENTINFO._serialized_start = 2253
+    _CLIENTINFO._serialized_end = 2580
+    _CLIENTINFO_SDK._serialized_start = 2470
+    _CLIENTINFO_SDK._serialized_end = 2580
+    _CLIENTCONFIGURATION._serialized_start = 2583
+    _CLIENTCONFIGURATION._serialized_end = 2851
+    _VIDEOCONFIGURATION._serialized_start = 2853
+    _VIDEOCONFIGURATION._serialized_end = 2929
+    _DISABLEDCODECS._serialized_start = 2931
+    _DISABLEDCODECS._serialized_end = 2979
+    _RTPSTATS._serialized_start = 2982
+    _RTPSTATS._serialized_end = 4163
+    _RTPSTATS_GAPHISTOGRAMENTRY._serialized_start = 4112
+    _RTPSTATS_GAPHISTOGRAMENTRY._serialized_end = 4163
+    _TIMEDVERSION._serialized_start = 4165
+    _TIMEDVERSION._serialized_end = 4214
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_models_pb2.pyi` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_models_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -6,41 +6,54 @@
 
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 
+AAC: AudioCodec
 AUDIO: TrackType
 CAMERA: TrackSource
 CLIENT_INITIATED: DisconnectReason
 DATA: TrackType
+DEFAULT_AC: AudioCodec
+DEFAULT_VC: VideoCodec
 DESCRIPTOR: _descriptor.FileDescriptor
 DISABLED: ClientConfigSetting
 DUPLICATE_IDENTITY: DisconnectReason
 ENABLED: ClientConfigSetting
 EXCELLENT: ConnectionQuality
 GOOD: ConnectionQuality
+H264_BASELINE: VideoCodec
+H264_HIGH: VideoCodec
+H264_MAIN: VideoCodec
 HIGH: VideoQuality
 JOIN_FAILURE: DisconnectReason
 LOW: VideoQuality
 MEDIUM: VideoQuality
 MICROPHONE: TrackSource
 OFF: VideoQuality
+OPUS: AudioCodec
 PARTICIPANT_REMOVED: DisconnectReason
 POOR: ConnectionQuality
 ROOM_DELETED: DisconnectReason
+RR_PUBLISHER_FAILED: ReconnectReason
+RR_SIGNAL_DISCONNECTED: ReconnectReason
+RR_SUBSCRIBER_FAILED: ReconnectReason
+RR_SWITCH_CANDIDATE: ReconnectReason
+RR_UNKOWN: ReconnectReason
 SCREEN_SHARE: TrackSource
 SCREEN_SHARE_AUDIO: TrackSource
 SERVER_SHUTDOWN: DisconnectReason
 STATE_MISMATCH: DisconnectReason
 UNKNOWN: TrackSource
 UNKNOWN_REASON: DisconnectReason
 UNSET: ClientConfigSetting
 VIDEO: TrackType
+VP8: VideoCodec
 
 class ActiveSpeakerUpdate(_message.Message):
     __slots__ = ["speakers"]
     SPEAKERS_FIELD_NUMBER: _ClassVar[int]
     speakers: _containers.RepeatedCompositeFieldContainer[SpeakerInfo]
     def __init__(
         self, speakers: _Optional[_Iterable[_Union[SpeakerInfo, _Mapping]]] = ...
@@ -97,14 +110,16 @@
     FLUTTER: ClientInfo.SDK
     GO: ClientInfo.SDK
     JS: ClientInfo.SDK
     NETWORK_FIELD_NUMBER: _ClassVar[int]
     OS_FIELD_NUMBER: _ClassVar[int]
     OS_VERSION_FIELD_NUMBER: _ClassVar[int]
     PROTOCOL_FIELD_NUMBER: _ClassVar[int]
+    REACT_NATIVE: ClientInfo.SDK
+    RUST: ClientInfo.SDK
     SDK_FIELD_NUMBER: _ClassVar[int]
     SWIFT: ClientInfo.SDK
     UNITY: ClientInfo.SDK
     UNKNOWN: ClientInfo.SDK
     VERSION_FIELD_NUMBER: _ClassVar[int]
     address: str
     browser: str
@@ -164,14 +179,24 @@
     __slots__ = ["codecs"]
     CODECS_FIELD_NUMBER: _ClassVar[int]
     codecs: _containers.RepeatedCompositeFieldContainer[Codec]
     def __init__(
         self, codecs: _Optional[_Iterable[_Union[Codec, _Mapping]]] = ...
     ) -> None: ...
 
+class Encryption(_message.Message):
+    __slots__ = []
+
+    class Type(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+    CUSTOM: Encryption.Type
+    GCM: Encryption.Type
+    NONE: Encryption.Type
+    def __init__(self) -> None: ...
+
 class ParticipantInfo(_message.Message):
     __slots__ = [
         "identity",
         "is_publisher",
         "joined_at",
         "metadata",
         "name",
@@ -226,35 +251,43 @@
         is_publisher: bool = ...,
     ) -> None: ...
 
 class ParticipantPermission(_message.Message):
     __slots__ = [
         "can_publish",
         "can_publish_data",
+        "can_publish_sources",
         "can_subscribe",
+        "can_update_metadata",
         "hidden",
         "recorder",
     ]
     CAN_PUBLISH_DATA_FIELD_NUMBER: _ClassVar[int]
     CAN_PUBLISH_FIELD_NUMBER: _ClassVar[int]
+    CAN_PUBLISH_SOURCES_FIELD_NUMBER: _ClassVar[int]
     CAN_SUBSCRIBE_FIELD_NUMBER: _ClassVar[int]
+    CAN_UPDATE_METADATA_FIELD_NUMBER: _ClassVar[int]
     HIDDEN_FIELD_NUMBER: _ClassVar[int]
     RECORDER_FIELD_NUMBER: _ClassVar[int]
     can_publish: bool
     can_publish_data: bool
+    can_publish_sources: _containers.RepeatedScalarFieldContainer[TrackSource]
     can_subscribe: bool
+    can_update_metadata: bool
     hidden: bool
     recorder: bool
     def __init__(
         self,
         can_subscribe: bool = ...,
         can_publish: bool = ...,
         can_publish_data: bool = ...,
+        can_publish_sources: _Optional[_Iterable[_Union[TrackSource, str]]] = ...,
         hidden: bool = ...,
         recorder: bool = ...,
+        can_update_metadata: bool = ...,
     ) -> None: ...
 
 class ParticipantTracks(_message.Message):
     __slots__ = ["participant_sid", "track_sids"]
     PARTICIPANT_SID_FIELD_NUMBER: _ClassVar[int]
     TRACK_SIDS_FIELD_NUMBER: _ClassVar[int]
     participant_sid: str
@@ -568,14 +601,15 @@
     ) -> None: ...
 
 class TrackInfo(_message.Message):
     __slots__ = [
         "codecs",
         "disable_dtx",
         "disable_red",
+        "encryption",
         "height",
         "layers",
         "mid",
         "mime_type",
         "muted",
         "name",
         "sid",
@@ -584,14 +618,15 @@
         "stereo",
         "type",
         "width",
     ]
     CODECS_FIELD_NUMBER: _ClassVar[int]
     DISABLE_DTX_FIELD_NUMBER: _ClassVar[int]
     DISABLE_RED_FIELD_NUMBER: _ClassVar[int]
+    ENCRYPTION_FIELD_NUMBER: _ClassVar[int]
     HEIGHT_FIELD_NUMBER: _ClassVar[int]
     LAYERS_FIELD_NUMBER: _ClassVar[int]
     MID_FIELD_NUMBER: _ClassVar[int]
     MIME_TYPE_FIELD_NUMBER: _ClassVar[int]
     MUTED_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     SID_FIELD_NUMBER: _ClassVar[int]
@@ -599,14 +634,15 @@
     SOURCE_FIELD_NUMBER: _ClassVar[int]
     STEREO_FIELD_NUMBER: _ClassVar[int]
     TYPE_FIELD_NUMBER: _ClassVar[int]
     WIDTH_FIELD_NUMBER: _ClassVar[int]
     codecs: _containers.RepeatedCompositeFieldContainer[SimulcastCodecInfo]
     disable_dtx: bool
     disable_red: bool
+    encryption: Encryption.Type
     height: int
     layers: _containers.RepeatedCompositeFieldContainer[VideoLayer]
     mid: str
     mime_type: str
     muted: bool
     name: str
     sid: str
@@ -628,29 +664,33 @@
         source: _Optional[_Union[TrackSource, str]] = ...,
         layers: _Optional[_Iterable[_Union[VideoLayer, _Mapping]]] = ...,
         mime_type: _Optional[str] = ...,
         mid: _Optional[str] = ...,
         codecs: _Optional[_Iterable[_Union[SimulcastCodecInfo, _Mapping]]] = ...,
         stereo: bool = ...,
         disable_red: bool = ...,
+        encryption: _Optional[_Union[Encryption.Type, str]] = ...,
     ) -> None: ...
 
 class UserPacket(_message.Message):
-    __slots__ = ["destination_sids", "participant_sid", "payload"]
+    __slots__ = ["destination_sids", "participant_sid", "payload", "topic"]
     DESTINATION_SIDS_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_SID_FIELD_NUMBER: _ClassVar[int]
     PAYLOAD_FIELD_NUMBER: _ClassVar[int]
+    TOPIC_FIELD_NUMBER: _ClassVar[int]
     destination_sids: _containers.RepeatedScalarFieldContainer[str]
     participant_sid: str
     payload: bytes
+    topic: str
     def __init__(
         self,
         participant_sid: _Optional[str] = ...,
         payload: _Optional[bytes] = ...,
         destination_sids: _Optional[_Iterable[str]] = ...,
+        topic: _Optional[str] = ...,
     ) -> None: ...
 
 class VideoConfiguration(_message.Message):
     __slots__ = ["hardware_encoder"]
     HARDWARE_ENCODER_FIELD_NUMBER: _ClassVar[int]
     hardware_encoder: ClientConfigSetting
     def __init__(
@@ -674,14 +714,20 @@
         quality: _Optional[_Union[VideoQuality, str]] = ...,
         width: _Optional[int] = ...,
         height: _Optional[int] = ...,
         bitrate: _Optional[int] = ...,
         ssrc: _Optional[int] = ...,
     ) -> None: ...
 
+class AudioCodec(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+
+class VideoCodec(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+
 class TrackType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
 class TrackSource(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
 class VideoQuality(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
@@ -691,7 +737,10 @@
     __slots__ = []
 
 class ClientConfigSetting(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
 class DisconnectReason(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
+
+class ReconnectReason(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_room_pb2.py` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_room_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,20 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import livekit_egress_pb2 as livekit__egress__pb2
 from . import livekit_models_pb2 as livekit__models__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x12livekit_room.proto\x12\x07livekit\x1a\x14livekit_models.proto\x1a\x14livekit_egress.proto"\x9a\x01\n\x11\x43reateRoomRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rempty_timeout\x18\x02 \x01(\r\x12\x18\n\x10max_participants\x18\x03 \x01(\r\x12\x0f\n\x07node_id\x18\x04 \x01(\t\x12\x10\n\x08metadata\x18\x05 \x01(\t\x12#\n\x06\x65gress\x18\x06 \x01(\x0b\x32\x13.livekit.RoomEgress"i\n\nRoomEgress\x12\x31\n\x04room\x18\x01 \x01(\x0b\x32#.livekit.RoomCompositeEgressRequest\x12(\n\x06tracks\x18\x02 \x01(\x0b\x32\x18.livekit.AutoTrackEgress"!\n\x10ListRoomsRequest\x12\r\n\x05names\x18\x01 \x03(\t"1\n\x11ListRoomsResponse\x12\x1c\n\x05rooms\x18\x01 \x03(\x0b\x32\r.livekit.Room"!\n\x11\x44\x65leteRoomRequest\x12\x0c\n\x04room\x18\x01 \x01(\t"\x14\n\x12\x44\x65leteRoomResponse"\'\n\x17ListParticipantsRequest\x12\x0c\n\x04room\x18\x01 \x01(\t"J\n\x18ListParticipantsResponse\x12.\n\x0cparticipants\x18\x01 \x03(\x0b\x32\x18.livekit.ParticipantInfo"9\n\x17RoomParticipantIdentity\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t"\x1b\n\x19RemoveParticipantResponse"X\n\x14MuteRoomTrackRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x11\n\ttrack_sid\x18\x03 \x01(\t\x12\r\n\x05muted\x18\x04 \x01(\x08":\n\x15MuteRoomTrackResponse\x12!\n\x05track\x18\x01 \x01(\x0b\x32\x12.livekit.TrackInfo"\x8e\x01\n\x18UpdateParticipantRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x10\n\x08metadata\x18\x03 \x01(\t\x12\x32\n\npermission\x18\x04 \x01(\x0b\x32\x1e.livekit.ParticipantPermission\x12\x0c\n\x04name\x18\x05 \x01(\t"\x9b\x01\n\x1aUpdateSubscriptionsRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x12\n\ntrack_sids\x18\x03 \x03(\t\x12\x11\n\tsubscribe\x18\x04 \x01(\x08\x12\x36\n\x12participant_tracks\x18\x05 \x03(\x0b\x32\x1a.livekit.ParticipantTracks"\x1d\n\x1bUpdateSubscriptionsResponse"o\n\x0fSendDataRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12&\n\x04kind\x18\x03 \x01(\x0e\x32\x18.livekit.DataPacket.Kind\x12\x18\n\x10\x64\x65stination_sids\x18\x04 \x03(\t"\x12\n\x10SendDataResponse";\n\x19UpdateRoomMetadataRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08metadata\x18\x02 \x01(\t2\xe6\x06\n\x0bRoomService\x12\x37\n\nCreateRoom\x12\x1a.livekit.CreateRoomRequest\x1a\r.livekit.Room\x12\x42\n\tListRooms\x12\x19.livekit.ListRoomsRequest\x1a\x1a.livekit.ListRoomsResponse\x12\x45\n\nDeleteRoom\x12\x1a.livekit.DeleteRoomRequest\x1a\x1b.livekit.DeleteRoomResponse\x12W\n\x10ListParticipants\x12 .livekit.ListParticipantsRequest\x1a!.livekit.ListParticipantsResponse\x12L\n\x0eGetParticipant\x12 .livekit.RoomParticipantIdentity\x1a\x18.livekit.ParticipantInfo\x12Y\n\x11RemoveParticipant\x12 .livekit.RoomParticipantIdentity\x1a".livekit.RemoveParticipantResponse\x12S\n\x12MutePublishedTrack\x12\x1d.livekit.MuteRoomTrackRequest\x1a\x1e.livekit.MuteRoomTrackResponse\x12P\n\x11UpdateParticipant\x12!.livekit.UpdateParticipantRequest\x1a\x18.livekit.ParticipantInfo\x12`\n\x13UpdateSubscriptions\x12#.livekit.UpdateSubscriptionsRequest\x1a$.livekit.UpdateSubscriptionsResponse\x12?\n\x08SendData\x12\x18.livekit.SendDataRequest\x1a\x19.livekit.SendDataResponse\x12G\n\x12UpdateRoomMetadata\x12".livekit.UpdateRoomMetadataRequest\x1a\r.livekit.RoomBFZ#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
+    b'\n\x12livekit_room.proto\x12\x07livekit\x1a\x14livekit_models.proto\x1a\x14livekit_egress.proto"\x9a\x01\n\x11\x43reateRoomRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rempty_timeout\x18\x02 \x01(\r\x12\x18\n\x10max_participants\x18\x03 \x01(\r\x12\x0f\n\x07node_id\x18\x04 \x01(\t\x12\x10\n\x08metadata\x18\x05 \x01(\t\x12#\n\x06\x65gress\x18\x06 \x01(\x0b\x32\x13.livekit.RoomEgress"i\n\nRoomEgress\x12\x31\n\x04room\x18\x01 \x01(\x0b\x32#.livekit.RoomCompositeEgressRequest\x12(\n\x06tracks\x18\x02 \x01(\x0b\x32\x18.livekit.AutoTrackEgress"!\n\x10ListRoomsRequest\x12\r\n\x05names\x18\x01 \x03(\t"1\n\x11ListRoomsResponse\x12\x1c\n\x05rooms\x18\x01 \x03(\x0b\x32\r.livekit.Room"!\n\x11\x44\x65leteRoomRequest\x12\x0c\n\x04room\x18\x01 \x01(\t"\x14\n\x12\x44\x65leteRoomResponse"\'\n\x17ListParticipantsRequest\x12\x0c\n\x04room\x18\x01 \x01(\t"J\n\x18ListParticipantsResponse\x12.\n\x0cparticipants\x18\x01 \x03(\x0b\x32\x18.livekit.ParticipantInfo"9\n\x17RoomParticipantIdentity\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t"\x1b\n\x19RemoveParticipantResponse"X\n\x14MuteRoomTrackRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x11\n\ttrack_sid\x18\x03 \x01(\t\x12\r\n\x05muted\x18\x04 \x01(\x08":\n\x15MuteRoomTrackResponse\x12!\n\x05track\x18\x01 \x01(\x0b\x32\x12.livekit.TrackInfo"\x8e\x01\n\x18UpdateParticipantRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x10\n\x08metadata\x18\x03 \x01(\t\x12\x32\n\npermission\x18\x04 \x01(\x0b\x32\x1e.livekit.ParticipantPermission\x12\x0c\n\x04name\x18\x05 \x01(\t"\x9b\x01\n\x1aUpdateSubscriptionsRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12\x12\n\ntrack_sids\x18\x03 \x03(\t\x12\x11\n\tsubscribe\x18\x04 \x01(\x08\x12\x36\n\x12participant_tracks\x18\x05 \x03(\x0b\x32\x1a.livekit.ParticipantTracks"\x1d\n\x1bUpdateSubscriptionsResponse"\x8d\x01\n\x0fSendDataRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12&\n\x04kind\x18\x03 \x01(\x0e\x32\x18.livekit.DataPacket.Kind\x12\x18\n\x10\x64\x65stination_sids\x18\x04 \x03(\t\x12\x12\n\x05topic\x18\x05 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_topic"\x12\n\x10SendDataResponse";\n\x19UpdateRoomMetadataRequest\x12\x0c\n\x04room\x18\x01 \x01(\t\x12\x10\n\x08metadata\x18\x02 \x01(\t2\xe6\x06\n\x0bRoomService\x12\x37\n\nCreateRoom\x12\x1a.livekit.CreateRoomRequest\x1a\r.livekit.Room\x12\x42\n\tListRooms\x12\x19.livekit.ListRoomsRequest\x1a\x1a.livekit.ListRoomsResponse\x12\x45\n\nDeleteRoom\x12\x1a.livekit.DeleteRoomRequest\x1a\x1b.livekit.DeleteRoomResponse\x12W\n\x10ListParticipants\x12 .livekit.ListParticipantsRequest\x1a!.livekit.ListParticipantsResponse\x12L\n\x0eGetParticipant\x12 .livekit.RoomParticipantIdentity\x1a\x18.livekit.ParticipantInfo\x12Y\n\x11RemoveParticipant\x12 .livekit.RoomParticipantIdentity\x1a".livekit.RemoveParticipantResponse\x12S\n\x12MutePublishedTrack\x12\x1d.livekit.MuteRoomTrackRequest\x1a\x1e.livekit.MuteRoomTrackResponse\x12P\n\x11UpdateParticipant\x12!.livekit.UpdateParticipantRequest\x1a\x18.livekit.ParticipantInfo\x12`\n\x13UpdateSubscriptions\x12#.livekit.UpdateSubscriptionsRequest\x1a$.livekit.UpdateSubscriptionsResponse\x12?\n\x08SendData\x12\x18.livekit.SendDataRequest\x1a\x19.livekit.SendDataResponse\x12G\n\x12UpdateRoomMetadata\x12".livekit.UpdateRoomMetadataRequest\x1a\r.livekit.RoomBFZ#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "livekit_room_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto"
     _CREATEROOMREQUEST._serialized_start = 76
     _CREATEROOMREQUEST._serialized_end = 230
     _ROOMEGRESS._serialized_start = 232
     _ROOMEGRESS._serialized_end = 337
     _LISTROOMSREQUEST._serialized_start = 339
@@ -51,16 +50,16 @@
     _MUTEROOMTRACKRESPONSE._serialized_end = 835
     _UPDATEPARTICIPANTREQUEST._serialized_start = 838
     _UPDATEPARTICIPANTREQUEST._serialized_end = 980
     _UPDATESUBSCRIPTIONSREQUEST._serialized_start = 983
     _UPDATESUBSCRIPTIONSREQUEST._serialized_end = 1138
     _UPDATESUBSCRIPTIONSRESPONSE._serialized_start = 1140
     _UPDATESUBSCRIPTIONSRESPONSE._serialized_end = 1169
-    _SENDDATAREQUEST._serialized_start = 1171
-    _SENDDATAREQUEST._serialized_end = 1282
-    _SENDDATARESPONSE._serialized_start = 1284
-    _SENDDATARESPONSE._serialized_end = 1302
-    _UPDATEROOMMETADATAREQUEST._serialized_start = 1304
-    _UPDATEROOMMETADATAREQUEST._serialized_end = 1363
-    _ROOMSERVICE._serialized_start = 1366
-    _ROOMSERVICE._serialized_end = 2236
+    _SENDDATAREQUEST._serialized_start = 1172
+    _SENDDATAREQUEST._serialized_end = 1313
+    _SENDDATARESPONSE._serialized_start = 1315
+    _SENDDATARESPONSE._serialized_end = 1333
+    _UPDATEROOMMETADATAREQUEST._serialized_start = 1335
+    _UPDATEROOMMETADATAREQUEST._serialized_end = 1394
+    _ROOMSERVICE._serialized_start = 1397
+    _ROOMSERVICE._serialized_end = 2267
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_room_pb2.pyi` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_room_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -138,29 +138,32 @@
     identity: str
     room: str
     def __init__(
         self, room: _Optional[str] = ..., identity: _Optional[str] = ...
     ) -> None: ...
 
 class SendDataRequest(_message.Message):
-    __slots__ = ["data", "destination_sids", "kind", "room"]
+    __slots__ = ["data", "destination_sids", "kind", "room", "topic"]
     DATA_FIELD_NUMBER: _ClassVar[int]
     DESTINATION_SIDS_FIELD_NUMBER: _ClassVar[int]
     KIND_FIELD_NUMBER: _ClassVar[int]
     ROOM_FIELD_NUMBER: _ClassVar[int]
+    TOPIC_FIELD_NUMBER: _ClassVar[int]
     data: bytes
     destination_sids: _containers.RepeatedScalarFieldContainer[str]
     kind: _livekit_models_pb2.DataPacket.Kind
     room: str
+    topic: str
     def __init__(
         self,
         room: _Optional[str] = ...,
         data: _Optional[bytes] = ...,
         kind: _Optional[_Union[_livekit_models_pb2.DataPacket.Kind, str]] = ...,
         destination_sids: _Optional[_Iterable[str]] = ...,
+        topic: _Optional[str] = ...,
     ) -> None: ...
 
 class SendDataResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class UpdateParticipantRequest(_message.Message):
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_rtc_pb2.py` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_egress_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,130 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: livekit_rtc.proto
+# source: livekit_egress.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import livekit_models_pb2 as livekit__models__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x11livekit_rtc.proto\x12\x07livekit\x1a\x14livekit_models.proto"\xf3\x04\n\rSignalRequest\x12,\n\x05offer\x18\x01 \x01(\x0b\x32\x1b.livekit.SessionDescriptionH\x00\x12-\n\x06\x61nswer\x18\x02 \x01(\x0b\x32\x1b.livekit.SessionDescriptionH\x00\x12*\n\x07trickle\x18\x03 \x01(\x0b\x32\x17.livekit.TrickleRequestH\x00\x12-\n\tadd_track\x18\x04 \x01(\x0b\x32\x18.livekit.AddTrackRequestH\x00\x12)\n\x04mute\x18\x05 \x01(\x0b\x32\x19.livekit.MuteTrackRequestH\x00\x12\x33\n\x0csubscription\x18\x06 \x01(\x0b\x32\x1b.livekit.UpdateSubscriptionH\x00\x12\x35\n\rtrack_setting\x18\x07 \x01(\x0b\x32\x1c.livekit.UpdateTrackSettingsH\x00\x12&\n\x05leave\x18\x08 \x01(\x0b\x32\x15.livekit.LeaveRequestH\x00\x12\x33\n\rupdate_layers\x18\n \x01(\x0b\x32\x1a.livekit.UpdateVideoLayersH\x00\x12\x42\n\x17subscription_permission\x18\x0b \x01(\x0b\x32\x1f.livekit.SubscriptionPermissionH\x00\x12(\n\nsync_state\x18\x0c \x01(\x0b\x32\x12.livekit.SyncStateH\x00\x12-\n\x08simulate\x18\r \x01(\x0b\x32\x19.livekit.SimulateScenarioH\x00\x12\x0e\n\x04ping\x18\x0e \x01(\x03H\x00\x42\t\n\x07message"\xe6\x06\n\x0eSignalResponse\x12%\n\x04join\x18\x01 \x01(\x0b\x32\x15.livekit.JoinResponseH\x00\x12-\n\x06\x61nswer\x18\x02 \x01(\x0b\x32\x1b.livekit.SessionDescriptionH\x00\x12,\n\x05offer\x18\x03 \x01(\x0b\x32\x1b.livekit.SessionDescriptionH\x00\x12*\n\x07trickle\x18\x04 \x01(\x0b\x32\x17.livekit.TrickleRequestH\x00\x12,\n\x06update\x18\x05 \x01(\x0b\x32\x1a.livekit.ParticipantUpdateH\x00\x12:\n\x0ftrack_published\x18\x06 \x01(\x0b\x32\x1f.livekit.TrackPublishedResponseH\x00\x12&\n\x05leave\x18\x08 \x01(\x0b\x32\x15.livekit.LeaveRequestH\x00\x12)\n\x04mute\x18\t \x01(\x0b\x32\x19.livekit.MuteTrackRequestH\x00\x12\x34\n\x10speakers_changed\x18\n \x01(\x0b\x32\x18.livekit.SpeakersChangedH\x00\x12*\n\x0broom_update\x18\x0b \x01(\x0b\x32\x13.livekit.RoomUpdateH\x00\x12>\n\x12\x63onnection_quality\x18\x0c \x01(\x0b\x32 .livekit.ConnectionQualityUpdateH\x00\x12\x39\n\x13stream_state_update\x18\r \x01(\x0b\x32\x1a.livekit.StreamStateUpdateH\x00\x12\x45\n\x19subscribed_quality_update\x18\x0e \x01(\x0b\x32 .livekit.SubscribedQualityUpdateH\x00\x12O\n\x1esubscription_permission_update\x18\x0f \x01(\x0b\x32%.livekit.SubscriptionPermissionUpdateH\x00\x12\x17\n\rrefresh_token\x18\x10 \x01(\tH\x00\x12>\n\x11track_unpublished\x18\x11 \x01(\x0b\x32!.livekit.TrackUnpublishedResponseH\x00\x12\x0e\n\x04pong\x18\x12 \x01(\x03H\x00\x42\t\n\x07message"M\n\x0eSimulcastCodec\x12\r\n\x05\x63odec\x18\x01 \x01(\t\x12\x0b\n\x03\x63id\x18\x02 \x01(\t\x12\x1f\n\x17\x65nable_simulcast_layers\x18\x03 \x01(\x08"\xc1\x02\n\x0f\x41\x64\x64TrackRequest\x12\x0b\n\x03\x63id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12 \n\x04type\x18\x03 \x01(\x0e\x32\x12.livekit.TrackType\x12\r\n\x05width\x18\x04 \x01(\r\x12\x0e\n\x06height\x18\x05 \x01(\r\x12\r\n\x05muted\x18\x06 \x01(\x08\x12\x13\n\x0b\x64isable_dtx\x18\x07 \x01(\x08\x12$\n\x06source\x18\x08 \x01(\x0e\x32\x14.livekit.TrackSource\x12#\n\x06layers\x18\t \x03(\x0b\x32\x13.livekit.VideoLayer\x12\x31\n\x10simulcast_codecs\x18\n \x03(\x0b\x32\x17.livekit.SimulcastCodec\x12\x0b\n\x03sid\x18\x0b \x01(\t\x12\x0e\n\x06stereo\x18\x0c \x01(\x08\x12\x13\n\x0b\x64isable_red\x18\r \x01(\x08"N\n\x0eTrickleRequest\x12\x15\n\rcandidateInit\x18\x01 \x01(\t\x12%\n\x06target\x18\x02 \x01(\x0e\x32\x15.livekit.SignalTarget".\n\x10MuteTrackRequest\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\r\n\x05muted\x18\x02 \x01(\x08"\xb0\x03\n\x0cJoinResponse\x12\x1b\n\x04room\x18\x01 \x01(\x0b\x32\r.livekit.Room\x12-\n\x0bparticipant\x18\x02 \x01(\x0b\x32\x18.livekit.ParticipantInfo\x12\x34\n\x12other_participants\x18\x03 \x03(\x0b\x32\x18.livekit.ParticipantInfo\x12\x16\n\x0eserver_version\x18\x04 \x01(\t\x12\'\n\x0bice_servers\x18\x05 \x03(\x0b\x32\x12.livekit.ICEServer\x12\x1a\n\x12subscriber_primary\x18\x06 \x01(\x08\x12\x17\n\x0f\x61lternative_url\x18\x07 \x01(\t\x12:\n\x14\x63lient_configuration\x18\x08 \x01(\x0b\x32\x1c.livekit.ClientConfiguration\x12\x15\n\rserver_region\x18\t \x01(\t\x12\x14\n\x0cping_timeout\x18\n \x01(\x05\x12\x15\n\rping_interval\x18\x0b \x01(\x05\x12(\n\x0bserver_info\x18\x0c \x01(\x0b\x32\x13.livekit.ServerInfo"H\n\x16TrackPublishedResponse\x12\x0b\n\x03\x63id\x18\x01 \x01(\t\x12!\n\x05track\x18\x02 \x01(\x0b\x32\x12.livekit.TrackInfo"-\n\x18TrackUnpublishedResponse\x12\x11\n\ttrack_sid\x18\x01 \x01(\t"/\n\x12SessionDescription\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0b\n\x03sdp\x18\x02 \x01(\t"C\n\x11ParticipantUpdate\x12.\n\x0cparticipants\x18\x01 \x03(\x0b\x32\x18.livekit.ParticipantInfo"s\n\x12UpdateSubscription\x12\x12\n\ntrack_sids\x18\x01 \x03(\t\x12\x11\n\tsubscribe\x18\x02 \x01(\x08\x12\x36\n\x12participant_tracks\x18\x03 \x03(\x0b\x32\x1a.livekit.ParticipantTracks"\x8f\x01\n\x13UpdateTrackSettings\x12\x12\n\ntrack_sids\x18\x01 \x03(\t\x12\x10\n\x08\x64isabled\x18\x03 \x01(\x08\x12&\n\x07quality\x18\x04 \x01(\x0e\x32\x15.livekit.VideoQuality\x12\r\n\x05width\x18\x05 \x01(\r\x12\x0e\n\x06height\x18\x06 \x01(\r\x12\x0b\n\x03\x66ps\x18\x07 \x01(\r"P\n\x0cLeaveRequest\x12\x15\n\rcan_reconnect\x18\x01 \x01(\x08\x12)\n\x06reason\x18\x02 \x01(\x0e\x32\x19.livekit.DisconnectReason"K\n\x11UpdateVideoLayers\x12\x11\n\ttrack_sid\x18\x01 \x01(\t\x12#\n\x06layers\x18\x02 \x03(\x0b\x32\x13.livekit.VideoLayer"?\n\tICEServer\x12\x0c\n\x04urls\x18\x01 \x03(\t\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x12\n\ncredential\x18\x03 \x01(\t"9\n\x0fSpeakersChanged\x12&\n\x08speakers\x18\x01 \x03(\x0b\x32\x14.livekit.SpeakerInfo")\n\nRoomUpdate\x12\x1b\n\x04room\x18\x01 \x01(\x0b\x32\r.livekit.Room"l\n\x15\x43onnectionQualityInfo\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12+\n\x07quality\x18\x02 \x01(\x0e\x32\x1a.livekit.ConnectionQuality\x12\r\n\x05score\x18\x03 \x01(\x02"J\n\x17\x43onnectionQualityUpdate\x12/\n\x07updates\x18\x01 \x03(\x0b\x32\x1e.livekit.ConnectionQualityInfo"b\n\x0fStreamStateInfo\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12\x11\n\ttrack_sid\x18\x02 \x01(\t\x12#\n\x05state\x18\x03 \x01(\x0e\x32\x14.livekit.StreamState"D\n\x11StreamStateUpdate\x12/\n\rstream_states\x18\x01 \x03(\x0b\x32\x18.livekit.StreamStateInfo"L\n\x11SubscribedQuality\x12&\n\x07quality\x18\x01 \x01(\x0e\x32\x15.livekit.VideoQuality\x12\x0f\n\x07\x65nabled\x18\x02 \x01(\x08"O\n\x0fSubscribedCodec\x12\r\n\x05\x63odec\x18\x01 \x01(\t\x12-\n\tqualities\x18\x02 \x03(\x0b\x32\x1a.livekit.SubscribedQuality"\x9b\x01\n\x17SubscribedQualityUpdate\x12\x11\n\ttrack_sid\x18\x01 \x01(\t\x12\x38\n\x14subscribed_qualities\x18\x02 \x03(\x0b\x32\x1a.livekit.SubscribedQuality\x12\x33\n\x11subscribed_codecs\x18\x03 \x03(\x0b\x32\x18.livekit.SubscribedCodec"p\n\x0fTrackPermission\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12\x12\n\nall_tracks\x18\x02 \x01(\x08\x12\x12\n\ntrack_sids\x18\x03 \x03(\t\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t"g\n\x16SubscriptionPermission\x12\x18\n\x10\x61ll_participants\x18\x01 \x01(\x08\x12\x33\n\x11track_permissions\x18\x02 \x03(\x0b\x32\x18.livekit.TrackPermission"[\n\x1cSubscriptionPermissionUpdate\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12\x11\n\ttrack_sid\x18\x02 \x01(\t\x12\x0f\n\x07\x61llowed\x18\x03 \x01(\x08"\x81\x02\n\tSyncState\x12+\n\x06\x61nswer\x18\x01 \x01(\x0b\x32\x1b.livekit.SessionDescription\x12\x31\n\x0csubscription\x18\x02 \x01(\x0b\x32\x1b.livekit.UpdateSubscription\x12\x37\n\x0epublish_tracks\x18\x03 \x03(\x0b\x32\x1f.livekit.TrackPublishedResponse\x12/\n\rdata_channels\x18\x04 \x03(\x0b\x32\x18.livekit.DataChannelInfo\x12*\n\x05offer\x18\x05 \x01(\x0b\x32\x1b.livekit.SessionDescription"S\n\x0f\x44\x61taChannelInfo\x12\r\n\x05label\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\r\x12%\n\x06target\x18\x03 \x01(\x0e\x32\x15.livekit.SignalTarget"\xbe\x01\n\x10SimulateScenario\x12\x18\n\x0espeaker_update\x18\x01 \x01(\x05H\x00\x12\x16\n\x0cnode_failure\x18\x02 \x01(\x08H\x00\x12\x13\n\tmigration\x18\x03 \x01(\x08H\x00\x12\x16\n\x0cserver_leave\x18\x04 \x01(\x08H\x00\x12?\n\x19switch_candidate_protocol\x18\x05 \x01(\x0e\x32\x1a.livekit.CandidateProtocolH\x00\x42\n\n\x08scenario*-\n\x0cSignalTarget\x12\r\n\tPUBLISHER\x10\x00\x12\x0e\n\nSUBSCRIBER\x10\x01*%\n\x0bStreamState\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\n\n\x06PAUSED\x10\x01*.\n\x11\x43\x61ndidateProtocol\x12\x07\n\x03UDP\x10\x00\x12\x07\n\x03TCP\x10\x01\x12\x07\n\x03TLS\x10\x02\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
+    b'\n\x14livekit_egress.proto\x12\x07livekit\x1a\x14livekit_models.proto"\xa0\x04\n\x1aRoomCompositeEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x0e\n\x06layout\x18\x02 \x01(\t\x12\x12\n\naudio_only\x18\x03 \x01(\x08\x12\x12\n\nvideo_only\x18\x04 \x01(\x08\x12\x17\n\x0f\x63ustom_base_url\x18\x05 \x01(\t\x12.\n\x04\x66ile\x18\x06 \x01(\x0b\x32\x1a.livekit.EncodedFileOutputB\x02\x18\x01H\x00\x12+\n\x06stream\x18\x07 \x01(\x0b\x32\x15.livekit.StreamOutputB\x02\x18\x01H\x00\x12\x34\n\x08segments\x18\n \x01(\x0b\x32\x1c.livekit.SegmentedFileOutputB\x02\x18\x01H\x00\x12\x30\n\x06preset\x18\x08 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x01\x12,\n\x08\x61\x64vanced\x18\t \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x01\x12\x30\n\x0c\x66ile_outputs\x18\x0b \x03(\x0b\x32\x1a.livekit.EncodedFileOutput\x12-\n\x0estream_outputs\x18\x0c \x03(\x0b\x32\x15.livekit.StreamOutput\x12\x35\n\x0fsegment_outputs\x18\r \x03(\x0b\x32\x1c.livekit.SegmentedFileOutputB\x08\n\x06outputB\t\n\x07options"\xe7\x03\n\x10WebEgressRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\naudio_only\x18\x02 \x01(\x08\x12\x12\n\nvideo_only\x18\x03 \x01(\x08\x12.\n\x04\x66ile\x18\x04 \x01(\x0b\x32\x1a.livekit.EncodedFileOutputB\x02\x18\x01H\x00\x12+\n\x06stream\x18\x05 \x01(\x0b\x32\x15.livekit.StreamOutputB\x02\x18\x01H\x00\x12\x34\n\x08segments\x18\x06 \x01(\x0b\x32\x1c.livekit.SegmentedFileOutputB\x02\x18\x01H\x00\x12\x30\n\x06preset\x18\x07 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x01\x12,\n\x08\x61\x64vanced\x18\x08 \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x01\x12\x30\n\x0c\x66ile_outputs\x18\t \x03(\x0b\x32\x1a.livekit.EncodedFileOutput\x12-\n\x0estream_outputs\x18\n \x03(\x0b\x32\x15.livekit.StreamOutput\x12\x35\n\x0fsegment_outputs\x18\x0b \x03(\x0b\x32\x1c.livekit.SegmentedFileOutputB\x08\n\x06outputB\t\n\x07options"\x80\x04\n\x1bTrackCompositeEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x16\n\x0e\x61udio_track_id\x18\x02 \x01(\t\x12\x16\n\x0evideo_track_id\x18\x03 \x01(\t\x12.\n\x04\x66ile\x18\x04 \x01(\x0b\x32\x1a.livekit.EncodedFileOutputB\x02\x18\x01H\x00\x12+\n\x06stream\x18\x05 \x01(\x0b\x32\x15.livekit.StreamOutputB\x02\x18\x01H\x00\x12\x34\n\x08segments\x18\x08 \x01(\x0b\x32\x1c.livekit.SegmentedFileOutputB\x02\x18\x01H\x00\x12\x30\n\x06preset\x18\x06 \x01(\x0e\x32\x1e.livekit.EncodingOptionsPresetH\x01\x12,\n\x08\x61\x64vanced\x18\x07 \x01(\x0b\x32\x18.livekit.EncodingOptionsH\x01\x12\x30\n\x0c\x66ile_outputs\x18\x0b \x03(\x0b\x32\x1a.livekit.EncodedFileOutput\x12-\n\x0estream_outputs\x18\x0c \x03(\x0b\x32\x15.livekit.StreamOutput\x12\x35\n\x0fsegment_outputs\x18\r \x03(\x0b\x32\x1c.livekit.SegmentedFileOutputB\x08\n\x06outputB\t\n\x07options"\x87\x01\n\x12TrackEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x10\n\x08track_id\x18\x02 \x01(\t\x12)\n\x04\x66ile\x18\x03 \x01(\x0b\x32\x19.livekit.DirectFileOutputH\x00\x12\x17\n\rwebsocket_url\x18\x04 \x01(\tH\x00\x42\x08\n\x06output"\x8e\x02\n\x11\x45ncodedFileOutput\x12+\n\tfile_type\x18\x01 \x01(\x0e\x32\x18.livekit.EncodedFileType\x12\x10\n\x08\x66ilepath\x18\x02 \x01(\t\x12\x18\n\x10\x64isable_manifest\x18\x06 \x01(\x08\x12\x1f\n\x02s3\x18\x03 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x04 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x05 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x12\'\n\x06\x61liOSS\x18\x07 \x01(\x0b\x32\x15.livekit.AliOSSUploadH\x00\x42\x08\n\x06output"\x84\x03\n\x13SegmentedFileOutput\x12\x30\n\x08protocol\x18\x01 \x01(\x0e\x32\x1e.livekit.SegmentedFileProtocol\x12\x17\n\x0f\x66ilename_prefix\x18\x02 \x01(\t\x12\x15\n\rplaylist_name\x18\x03 \x01(\t\x12\x18\n\x10segment_duration\x18\x04 \x01(\r\x12\x35\n\x0f\x66ilename_suffix\x18\n \x01(\x0e\x32\x1c.livekit.SegmentedFileSuffix\x12\x18\n\x10\x64isable_manifest\x18\x08 \x01(\x08\x12\x1f\n\x02s3\x18\x05 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x06 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x07 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x12\'\n\x06\x61liOSS\x18\t \x01(\x0b\x32\x15.livekit.AliOSSUploadH\x00\x42\x08\n\x06output"\xe0\x01\n\x10\x44irectFileOutput\x12\x10\n\x08\x66ilepath\x18\x01 \x01(\t\x12\x18\n\x10\x64isable_manifest\x18\x05 \x01(\x08\x12\x1f\n\x02s3\x18\x02 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x03 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x04 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x12\'\n\x06\x61liOSS\x18\x06 \x01(\x0b\x32\x15.livekit.AliOSSUploadH\x00\x42\x08\n\x06output"\xef\x01\n\x08S3Upload\x12\x12\n\naccess_key\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\x0e\n\x06region\x18\x03 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x04 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x05 \x01(\t\x12\x18\n\x10\x66orce_path_style\x18\x06 \x01(\x08\x12\x31\n\x08metadata\x18\x07 \x03(\x0b\x32\x1f.livekit.S3Upload.MetadataEntry\x12\x0f\n\x07tagging\x18\x08 \x01(\t\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01"0\n\tGCPUpload\x12\x13\n\x0b\x63redentials\x18\x01 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x02 \x01(\t"T\n\x0f\x41zureBlobUpload\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63\x63ount_key\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_name\x18\x03 \x01(\t"d\n\x0c\x41liOSSUpload\x12\x12\n\naccess_key\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\x0e\n\x06region\x18\x03 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x04 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x05 \x01(\t"G\n\x0cStreamOutput\x12)\n\x08protocol\x18\x01 \x01(\x0e\x32\x17.livekit.StreamProtocol\x12\x0c\n\x04urls\x18\x02 \x03(\t"\x89\x02\n\x0f\x45ncodingOptions\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\r\n\x05\x64\x65pth\x18\x03 \x01(\x05\x12\x11\n\tframerate\x18\x04 \x01(\x05\x12(\n\x0b\x61udio_codec\x18\x05 \x01(\x0e\x32\x13.livekit.AudioCodec\x12\x15\n\raudio_bitrate\x18\x06 \x01(\x05\x12\x17\n\x0f\x61udio_frequency\x18\x07 \x01(\x05\x12(\n\x0bvideo_codec\x18\x08 \x01(\x0e\x32\x13.livekit.VideoCodec\x12\x15\n\rvideo_bitrate\x18\t \x01(\x05\x12\x1a\n\x12key_frame_interval\x18\n \x01(\x01"8\n\x13UpdateLayoutRequest\x12\x11\n\tegress_id\x18\x01 \x01(\t\x12\x0e\n\x06layout\x18\x02 \x01(\t"]\n\x13UpdateStreamRequest\x12\x11\n\tegress_id\x18\x01 \x01(\t\x12\x17\n\x0f\x61\x64\x64_output_urls\x18\x02 \x03(\t\x12\x1a\n\x12remove_output_urls\x18\x03 \x03(\t"I\n\x11ListEgressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x11\n\tegress_id\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08"8\n\x12ListEgressResponse\x12"\n\x05items\x18\x01 \x03(\x0b\x32\x13.livekit.EgressInfo"&\n\x11StopEgressRequest\x12\x11\n\tegress_id\x18\x01 \x01(\t"\x97\x05\n\nEgressInfo\x12\x11\n\tegress_id\x18\x01 \x01(\t\x12\x0f\n\x07room_id\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\r \x01(\t\x12%\n\x06status\x18\x03 \x01(\x0e\x32\x15.livekit.EgressStatus\x12\x12\n\nstarted_at\x18\n \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x0b \x01(\x03\x12\r\n\x05\x65rror\x18\t \x01(\t\x12=\n\x0eroom_composite\x18\x04 \x01(\x0b\x32#.livekit.RoomCompositeEgressRequestH\x00\x12?\n\x0ftrack_composite\x18\x05 \x01(\x0b\x32$.livekit.TrackCompositeEgressRequestH\x00\x12,\n\x05track\x18\x06 \x01(\x0b\x32\x1b.livekit.TrackEgressRequestH\x00\x12(\n\x03web\x18\x0e \x01(\x0b\x32\x19.livekit.WebEgressRequestH\x00\x12-\n\x06stream\x18\x07 \x01(\x0b\x32\x17.livekit.StreamInfoListB\x02\x18\x01H\x01\x12%\n\x04\x66ile\x18\x08 \x01(\x0b\x32\x11.livekit.FileInfoB\x02\x18\x01H\x01\x12-\n\x08segments\x18\x0c \x01(\x0b\x32\x15.livekit.SegmentsInfoB\x02\x18\x01H\x01\x12+\n\x0estream_results\x18\x0f \x03(\x0b\x32\x13.livekit.StreamInfo\x12\'\n\x0c\x66ile_results\x18\x10 \x03(\x0b\x32\x11.livekit.FileInfo\x12.\n\x0fsegment_results\x18\x11 \x03(\x0b\x32\x15.livekit.SegmentsInfoB\t\n\x07requestB\x08\n\x06result"7\n\x0eStreamInfoList\x12!\n\x04info\x18\x01 \x03(\x0b\x32\x13.livekit.StreamInfo:\x02\x18\x01"\xbc\x01\n\nStreamInfo\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x12\n\nstarted_at\x18\x02 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x03 \x01(\x03\x12\x10\n\x08\x64uration\x18\x04 \x01(\x03\x12*\n\x06status\x18\x05 \x01(\x0e\x32\x1a.livekit.StreamInfo.Status\x12\r\n\x05\x65rror\x18\x06 \x01(\t".\n\x06Status\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08\x46INISHED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02"t\n\x08\x46ileInfo\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x12\x12\n\nstarted_at\x18\x02 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x03 \x01(\x03\x12\x10\n\x08\x64uration\x18\x06 \x01(\x03\x12\x0c\n\x04size\x18\x04 \x01(\x03\x12\x10\n\x08location\x18\x05 \x01(\t"\x9d\x01\n\x0cSegmentsInfo\x12\x15\n\rplaylist_name\x18\x01 \x01(\t\x12\x10\n\x08\x64uration\x18\x02 \x01(\x03\x12\x0c\n\x04size\x18\x03 \x01(\x03\x12\x19\n\x11playlist_location\x18\x04 \x01(\t\x12\x15\n\rsegment_count\x18\x05 \x01(\x03\x12\x12\n\nstarted_at\x18\x06 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x07 \x01(\x03"\xb6\x01\n\x0f\x41utoTrackEgress\x12\x10\n\x08\x66ilepath\x18\x01 \x01(\t\x12\x18\n\x10\x64isable_manifest\x18\x05 \x01(\x08\x12\x1f\n\x02s3\x18\x02 \x01(\x0b\x32\x11.livekit.S3UploadH\x00\x12!\n\x03gcp\x18\x03 \x01(\x0b\x32\x12.livekit.GCPUploadH\x00\x12)\n\x05\x61zure\x18\x04 \x01(\x0b\x32\x18.livekit.AzureBlobUploadH\x00\x42\x08\n\x06output*9\n\x0f\x45ncodedFileType\x12\x14\n\x10\x44\x45\x46\x41ULT_FILETYPE\x10\x00\x12\x07\n\x03MP4\x10\x01\x12\x07\n\x03OGG\x10\x02*N\n\x15SegmentedFileProtocol\x12#\n\x1f\x44\x45\x46\x41ULT_SEGMENTED_FILE_PROTOCOL\x10\x00\x12\x10\n\x0cHLS_PROTOCOL\x10\x01*/\n\x13SegmentedFileSuffix\x12\t\n\x05INDEX\x10\x00\x12\r\n\tTIMESTAMP\x10\x01*0\n\x0eStreamProtocol\x12\x14\n\x10\x44\x45\x46\x41ULT_PROTOCOL\x10\x00\x12\x08\n\x04RTMP\x10\x01*\xcf\x01\n\x15\x45ncodingOptionsPreset\x12\x10\n\x0cH264_720P_30\x10\x00\x12\x10\n\x0cH264_720P_60\x10\x01\x12\x11\n\rH264_1080P_30\x10\x02\x12\x11\n\rH264_1080P_60\x10\x03\x12\x19\n\x15PORTRAIT_H264_720P_30\x10\x04\x12\x19\n\x15PORTRAIT_H264_720P_60\x10\x05\x12\x1a\n\x16PORTRAIT_H264_1080P_30\x10\x06\x12\x1a\n\x16PORTRAIT_H264_1080P_60\x10\x07*\x9f\x01\n\x0c\x45gressStatus\x12\x13\n\x0f\x45GRESS_STARTING\x10\x00\x12\x11\n\rEGRESS_ACTIVE\x10\x01\x12\x11\n\rEGRESS_ENDING\x10\x02\x12\x13\n\x0f\x45GRESS_COMPLETE\x10\x03\x12\x11\n\rEGRESS_FAILED\x10\x04\x12\x12\n\x0e\x45GRESS_ABORTED\x10\x05\x12\x18\n\x14\x45GRESS_LIMIT_REACHED\x10\x06\x32\xca\x04\n\x06\x45gress\x12T\n\x18StartRoomCompositeEgress\x12#.livekit.RoomCompositeEgressRequest\x1a\x13.livekit.EgressInfo\x12V\n\x19StartTrackCompositeEgress\x12$.livekit.TrackCompositeEgressRequest\x1a\x13.livekit.EgressInfo\x12\x44\n\x10StartTrackEgress\x12\x1b.livekit.TrackEgressRequest\x1a\x13.livekit.EgressInfo\x12@\n\x0eStartWebEgress\x12\x19.livekit.WebEgressRequest\x1a\x13.livekit.EgressInfo\x12\x41\n\x0cUpdateLayout\x12\x1c.livekit.UpdateLayoutRequest\x1a\x13.livekit.EgressInfo\x12\x41\n\x0cUpdateStream\x12\x1c.livekit.UpdateStreamRequest\x1a\x13.livekit.EgressInfo\x12\x45\n\nListEgress\x12\x1a.livekit.ListEgressRequest\x1a\x1b.livekit.ListEgressResponse\x12=\n\nStopEgress\x12\x1a.livekit.StopEgressRequest\x1a\x13.livekit.EgressInfoBFZ#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "livekit_rtc_pb2", globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "livekit_egress_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto"
-    _SIGNALTARGET._serialized_start = 4872
-    _SIGNALTARGET._serialized_end = 4917
-    _STREAMSTATE._serialized_start = 4919
-    _STREAMSTATE._serialized_end = 4956
-    _CANDIDATEPROTOCOL._serialized_start = 4958
-    _CANDIDATEPROTOCOL._serialized_end = 5004
-    _SIGNALREQUEST._serialized_start = 53
-    _SIGNALREQUEST._serialized_end = 680
-    _SIGNALRESPONSE._serialized_start = 683
-    _SIGNALRESPONSE._serialized_end = 1553
-    _SIMULCASTCODEC._serialized_start = 1555
-    _SIMULCASTCODEC._serialized_end = 1632
-    _ADDTRACKREQUEST._serialized_start = 1635
-    _ADDTRACKREQUEST._serialized_end = 1956
-    _TRICKLEREQUEST._serialized_start = 1958
-    _TRICKLEREQUEST._serialized_end = 2036
-    _MUTETRACKREQUEST._serialized_start = 2038
-    _MUTETRACKREQUEST._serialized_end = 2084
-    _JOINRESPONSE._serialized_start = 2087
-    _JOINRESPONSE._serialized_end = 2519
-    _TRACKPUBLISHEDRESPONSE._serialized_start = 2521
-    _TRACKPUBLISHEDRESPONSE._serialized_end = 2593
-    _TRACKUNPUBLISHEDRESPONSE._serialized_start = 2595
-    _TRACKUNPUBLISHEDRESPONSE._serialized_end = 2640
-    _SESSIONDESCRIPTION._serialized_start = 2642
-    _SESSIONDESCRIPTION._serialized_end = 2689
-    _PARTICIPANTUPDATE._serialized_start = 2691
-    _PARTICIPANTUPDATE._serialized_end = 2758
-    _UPDATESUBSCRIPTION._serialized_start = 2760
-    _UPDATESUBSCRIPTION._serialized_end = 2875
-    _UPDATETRACKSETTINGS._serialized_start = 2878
-    _UPDATETRACKSETTINGS._serialized_end = 3021
-    _LEAVEREQUEST._serialized_start = 3023
-    _LEAVEREQUEST._serialized_end = 3103
-    _UPDATEVIDEOLAYERS._serialized_start = 3105
-    _UPDATEVIDEOLAYERS._serialized_end = 3180
-    _ICESERVER._serialized_start = 3182
-    _ICESERVER._serialized_end = 3245
-    _SPEAKERSCHANGED._serialized_start = 3247
-    _SPEAKERSCHANGED._serialized_end = 3304
-    _ROOMUPDATE._serialized_start = 3306
-    _ROOMUPDATE._serialized_end = 3347
-    _CONNECTIONQUALITYINFO._serialized_start = 3349
-    _CONNECTIONQUALITYINFO._serialized_end = 3457
-    _CONNECTIONQUALITYUPDATE._serialized_start = 3459
-    _CONNECTIONQUALITYUPDATE._serialized_end = 3533
-    _STREAMSTATEINFO._serialized_start = 3535
-    _STREAMSTATEINFO._serialized_end = 3633
-    _STREAMSTATEUPDATE._serialized_start = 3635
-    _STREAMSTATEUPDATE._serialized_end = 3703
-    _SUBSCRIBEDQUALITY._serialized_start = 3705
-    _SUBSCRIBEDQUALITY._serialized_end = 3781
-    _SUBSCRIBEDCODEC._serialized_start = 3783
-    _SUBSCRIBEDCODEC._serialized_end = 3862
-    _SUBSCRIBEDQUALITYUPDATE._serialized_start = 3865
-    _SUBSCRIBEDQUALITYUPDATE._serialized_end = 4020
-    _TRACKPERMISSION._serialized_start = 4022
-    _TRACKPERMISSION._serialized_end = 4134
-    _SUBSCRIPTIONPERMISSION._serialized_start = 4136
-    _SUBSCRIPTIONPERMISSION._serialized_end = 4239
-    _SUBSCRIPTIONPERMISSIONUPDATE._serialized_start = 4241
-    _SUBSCRIPTIONPERMISSIONUPDATE._serialized_end = 4332
-    _SYNCSTATE._serialized_start = 4335
-    _SYNCSTATE._serialized_end = 4592
-    _DATACHANNELINFO._serialized_start = 4594
-    _DATACHANNELINFO._serialized_end = 4677
-    _SIMULATESCENARIO._serialized_start = 4680
-    _SIMULATESCENARIO._serialized_end = 4870
+    _ROOMCOMPOSITEEGRESSREQUEST.fields_by_name["file"]._options = None
+    _ROOMCOMPOSITEEGRESSREQUEST.fields_by_name["file"]._serialized_options = b"\030\001"
+    _ROOMCOMPOSITEEGRESSREQUEST.fields_by_name["stream"]._options = None
+    _ROOMCOMPOSITEEGRESSREQUEST.fields_by_name[
+        "stream"
+    ]._serialized_options = b"\030\001"
+    _ROOMCOMPOSITEEGRESSREQUEST.fields_by_name["segments"]._options = None
+    _ROOMCOMPOSITEEGRESSREQUEST.fields_by_name[
+        "segments"
+    ]._serialized_options = b"\030\001"
+    _WEBEGRESSREQUEST.fields_by_name["file"]._options = None
+    _WEBEGRESSREQUEST.fields_by_name["file"]._serialized_options = b"\030\001"
+    _WEBEGRESSREQUEST.fields_by_name["stream"]._options = None
+    _WEBEGRESSREQUEST.fields_by_name["stream"]._serialized_options = b"\030\001"
+    _WEBEGRESSREQUEST.fields_by_name["segments"]._options = None
+    _WEBEGRESSREQUEST.fields_by_name["segments"]._serialized_options = b"\030\001"
+    _TRACKCOMPOSITEEGRESSREQUEST.fields_by_name["file"]._options = None
+    _TRACKCOMPOSITEEGRESSREQUEST.fields_by_name[
+        "file"
+    ]._serialized_options = b"\030\001"
+    _TRACKCOMPOSITEEGRESSREQUEST.fields_by_name["stream"]._options = None
+    _TRACKCOMPOSITEEGRESSREQUEST.fields_by_name[
+        "stream"
+    ]._serialized_options = b"\030\001"
+    _TRACKCOMPOSITEEGRESSREQUEST.fields_by_name["segments"]._options = None
+    _TRACKCOMPOSITEEGRESSREQUEST.fields_by_name[
+        "segments"
+    ]._serialized_options = b"\030\001"
+    _S3UPLOAD_METADATAENTRY._options = None
+    _S3UPLOAD_METADATAENTRY._serialized_options = b"8\001"
+    _EGRESSINFO.fields_by_name["stream"]._options = None
+    _EGRESSINFO.fields_by_name["stream"]._serialized_options = b"\030\001"
+    _EGRESSINFO.fields_by_name["file"]._options = None
+    _EGRESSINFO.fields_by_name["file"]._serialized_options = b"\030\001"
+    _EGRESSINFO.fields_by_name["segments"]._options = None
+    _EGRESSINFO.fields_by_name["segments"]._serialized_options = b"\030\001"
+    _STREAMINFOLIST._options = None
+    _STREAMINFOLIST._serialized_options = b"\030\001"
+    _ENCODEDFILETYPE._serialized_start = 5160
+    _ENCODEDFILETYPE._serialized_end = 5217
+    _SEGMENTEDFILEPROTOCOL._serialized_start = 5219
+    _SEGMENTEDFILEPROTOCOL._serialized_end = 5297
+    _SEGMENTEDFILESUFFIX._serialized_start = 5299
+    _SEGMENTEDFILESUFFIX._serialized_end = 5346
+    _STREAMPROTOCOL._serialized_start = 5348
+    _STREAMPROTOCOL._serialized_end = 5396
+    _ENCODINGOPTIONSPRESET._serialized_start = 5399
+    _ENCODINGOPTIONSPRESET._serialized_end = 5606
+    _EGRESSSTATUS._serialized_start = 5609
+    _EGRESSSTATUS._serialized_end = 5768
+    _ROOMCOMPOSITEEGRESSREQUEST._serialized_start = 56
+    _ROOMCOMPOSITEEGRESSREQUEST._serialized_end = 600
+    _WEBEGRESSREQUEST._serialized_start = 603
+    _WEBEGRESSREQUEST._serialized_end = 1090
+    _TRACKCOMPOSITEEGRESSREQUEST._serialized_start = 1093
+    _TRACKCOMPOSITEEGRESSREQUEST._serialized_end = 1605
+    _TRACKEGRESSREQUEST._serialized_start = 1608
+    _TRACKEGRESSREQUEST._serialized_end = 1743
+    _ENCODEDFILEOUTPUT._serialized_start = 1746
+    _ENCODEDFILEOUTPUT._serialized_end = 2016
+    _SEGMENTEDFILEOUTPUT._serialized_start = 2019
+    _SEGMENTEDFILEOUTPUT._serialized_end = 2407
+    _DIRECTFILEOUTPUT._serialized_start = 2410
+    _DIRECTFILEOUTPUT._serialized_end = 2634
+    _S3UPLOAD._serialized_start = 2637
+    _S3UPLOAD._serialized_end = 2876
+    _S3UPLOAD_METADATAENTRY._serialized_start = 2829
+    _S3UPLOAD_METADATAENTRY._serialized_end = 2876
+    _GCPUPLOAD._serialized_start = 2878
+    _GCPUPLOAD._serialized_end = 2926
+    _AZUREBLOBUPLOAD._serialized_start = 2928
+    _AZUREBLOBUPLOAD._serialized_end = 3012
+    _ALIOSSUPLOAD._serialized_start = 3014
+    _ALIOSSUPLOAD._serialized_end = 3114
+    _STREAMOUTPUT._serialized_start = 3116
+    _STREAMOUTPUT._serialized_end = 3187
+    _ENCODINGOPTIONS._serialized_start = 3190
+    _ENCODINGOPTIONS._serialized_end = 3455
+    _UPDATELAYOUTREQUEST._serialized_start = 3457
+    _UPDATELAYOUTREQUEST._serialized_end = 3513
+    _UPDATESTREAMREQUEST._serialized_start = 3515
+    _UPDATESTREAMREQUEST._serialized_end = 3608
+    _LISTEGRESSREQUEST._serialized_start = 3610
+    _LISTEGRESSREQUEST._serialized_end = 3683
+    _LISTEGRESSRESPONSE._serialized_start = 3685
+    _LISTEGRESSRESPONSE._serialized_end = 3741
+    _STOPEGRESSREQUEST._serialized_start = 3743
+    _STOPEGRESSREQUEST._serialized_end = 3781
+    _EGRESSINFO._serialized_start = 3784
+    _EGRESSINFO._serialized_end = 4447
+    _STREAMINFOLIST._serialized_start = 4449
+    _STREAMINFOLIST._serialized_end = 4504
+    _STREAMINFO._serialized_start = 4507
+    _STREAMINFO._serialized_end = 4695
+    _STREAMINFO_STATUS._serialized_start = 4649
+    _STREAMINFO_STATUS._serialized_end = 4695
+    _FILEINFO._serialized_start = 4697
+    _FILEINFO._serialized_end = 4813
+    _SEGMENTSINFO._serialized_start = 4816
+    _SEGMENTSINFO._serialized_end = 4973
+    _AUTOTRACKEGRESS._serialized_start = 4976
+    _AUTOTRACKEGRESS._serialized_end = 5158
+    _EGRESS._serialized_start = 5771
+    _EGRESS._serialized_end = 6357
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_rtc_pb2.pyi` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_rtc_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -20,41 +20,44 @@
 UDP: CandidateProtocol
 
 class AddTrackRequest(_message.Message):
     __slots__ = [
         "cid",
         "disable_dtx",
         "disable_red",
+        "encryption",
         "height",
         "layers",
         "muted",
         "name",
         "sid",
         "simulcast_codecs",
         "source",
         "stereo",
         "type",
         "width",
     ]
     CID_FIELD_NUMBER: _ClassVar[int]
     DISABLE_DTX_FIELD_NUMBER: _ClassVar[int]
     DISABLE_RED_FIELD_NUMBER: _ClassVar[int]
+    ENCRYPTION_FIELD_NUMBER: _ClassVar[int]
     HEIGHT_FIELD_NUMBER: _ClassVar[int]
     LAYERS_FIELD_NUMBER: _ClassVar[int]
     MUTED_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     SID_FIELD_NUMBER: _ClassVar[int]
     SIMULCAST_CODECS_FIELD_NUMBER: _ClassVar[int]
     SOURCE_FIELD_NUMBER: _ClassVar[int]
     STEREO_FIELD_NUMBER: _ClassVar[int]
     TYPE_FIELD_NUMBER: _ClassVar[int]
     WIDTH_FIELD_NUMBER: _ClassVar[int]
     cid: str
     disable_dtx: bool
     disable_red: bool
+    encryption: _livekit_models_pb2.Encryption.Type
     height: int
     layers: _containers.RepeatedCompositeFieldContainer[_livekit_models_pb2.VideoLayer]
     muted: bool
     name: str
     sid: str
     simulcast_codecs: _containers.RepeatedCompositeFieldContainer[SimulcastCodec]
     source: _livekit_models_pb2.TrackSource
@@ -74,14 +77,15 @@
         layers: _Optional[
             _Iterable[_Union[_livekit_models_pb2.VideoLayer, _Mapping]]
         ] = ...,
         simulcast_codecs: _Optional[_Iterable[_Union[SimulcastCodec, _Mapping]]] = ...,
         sid: _Optional[str] = ...,
         stereo: bool = ...,
         disable_red: bool = ...,
+        encryption: _Optional[_Union[_livekit_models_pb2.Encryption.Type, str]] = ...,
     ) -> None: ...
 
 class ConnectionQualityInfo(_message.Message):
     __slots__ = ["participant_sid", "quality", "score"]
     PARTICIPANT_SID_FIELD_NUMBER: _ClassVar[int]
     QUALITY_FIELD_NUMBER: _ClassVar[int]
     SCORE_FIELD_NUMBER: _ClassVar[int]
@@ -226,14 +230,71 @@
     def __init__(
         self,
         participants: _Optional[
             _Iterable[_Union[_livekit_models_pb2.ParticipantInfo, _Mapping]]
         ] = ...,
     ) -> None: ...
 
+class Ping(_message.Message):
+    __slots__ = ["rtt", "timestamp"]
+    RTT_FIELD_NUMBER: _ClassVar[int]
+    TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
+    rtt: int
+    timestamp: int
+    def __init__(
+        self, timestamp: _Optional[int] = ..., rtt: _Optional[int] = ...
+    ) -> None: ...
+
+class Pong(_message.Message):
+    __slots__ = ["last_ping_timestamp", "timestamp"]
+    LAST_PING_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
+    TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
+    last_ping_timestamp: int
+    timestamp: int
+    def __init__(
+        self, last_ping_timestamp: _Optional[int] = ..., timestamp: _Optional[int] = ...
+    ) -> None: ...
+
+class ReconnectResponse(_message.Message):
+    __slots__ = ["client_configuration", "ice_servers"]
+    CLIENT_CONFIGURATION_FIELD_NUMBER: _ClassVar[int]
+    ICE_SERVERS_FIELD_NUMBER: _ClassVar[int]
+    client_configuration: _livekit_models_pb2.ClientConfiguration
+    ice_servers: _containers.RepeatedCompositeFieldContainer[ICEServer]
+    def __init__(
+        self,
+        ice_servers: _Optional[_Iterable[_Union[ICEServer, _Mapping]]] = ...,
+        client_configuration: _Optional[
+            _Union[_livekit_models_pb2.ClientConfiguration, _Mapping]
+        ] = ...,
+    ) -> None: ...
+
+class RegionInfo(_message.Message):
+    __slots__ = ["distance", "region", "url"]
+    DISTANCE_FIELD_NUMBER: _ClassVar[int]
+    REGION_FIELD_NUMBER: _ClassVar[int]
+    URL_FIELD_NUMBER: _ClassVar[int]
+    distance: int
+    region: str
+    url: str
+    def __init__(
+        self,
+        region: _Optional[str] = ...,
+        url: _Optional[str] = ...,
+        distance: _Optional[int] = ...,
+    ) -> None: ...
+
+class RegionSettings(_message.Message):
+    __slots__ = ["regions"]
+    REGIONS_FIELD_NUMBER: _ClassVar[int]
+    regions: _containers.RepeatedCompositeFieldContainer[RegionInfo]
+    def __init__(
+        self, regions: _Optional[_Iterable[_Union[RegionInfo, _Mapping]]] = ...
+    ) -> None: ...
+
 class RoomUpdate(_message.Message):
     __slots__ = ["room"]
     ROOM_FIELD_NUMBER: _ClassVar[int]
     room: _livekit_models_pb2.Room
     def __init__(
         self, room: _Optional[_Union[_livekit_models_pb2.Room, _Mapping]] = ...
     ) -> None: ...
@@ -252,48 +313,54 @@
     __slots__ = [
         "add_track",
         "answer",
         "leave",
         "mute",
         "offer",
         "ping",
+        "ping_req",
         "simulate",
         "subscription",
         "subscription_permission",
         "sync_state",
         "track_setting",
         "trickle",
         "update_layers",
+        "update_metadata",
     ]
     ADD_TRACK_FIELD_NUMBER: _ClassVar[int]
     ANSWER_FIELD_NUMBER: _ClassVar[int]
     LEAVE_FIELD_NUMBER: _ClassVar[int]
     MUTE_FIELD_NUMBER: _ClassVar[int]
     OFFER_FIELD_NUMBER: _ClassVar[int]
     PING_FIELD_NUMBER: _ClassVar[int]
+    PING_REQ_FIELD_NUMBER: _ClassVar[int]
     SIMULATE_FIELD_NUMBER: _ClassVar[int]
     SUBSCRIPTION_FIELD_NUMBER: _ClassVar[int]
     SUBSCRIPTION_PERMISSION_FIELD_NUMBER: _ClassVar[int]
     SYNC_STATE_FIELD_NUMBER: _ClassVar[int]
     TRACK_SETTING_FIELD_NUMBER: _ClassVar[int]
     TRICKLE_FIELD_NUMBER: _ClassVar[int]
     UPDATE_LAYERS_FIELD_NUMBER: _ClassVar[int]
+    UPDATE_METADATA_FIELD_NUMBER: _ClassVar[int]
     add_track: AddTrackRequest
     answer: SessionDescription
     leave: LeaveRequest
     mute: MuteTrackRequest
     offer: SessionDescription
     ping: int
+    ping_req: Ping
     simulate: SimulateScenario
     subscription: UpdateSubscription
     subscription_permission: SubscriptionPermission
     sync_state: SyncState
     track_setting: UpdateTrackSettings
     trickle: TrickleRequest
     update_layers: UpdateVideoLayers
+    update_metadata: UpdateParticipantMetadata
     def __init__(
         self,
         offer: _Optional[_Union[SessionDescription, _Mapping]] = ...,
         answer: _Optional[_Union[SessionDescription, _Mapping]] = ...,
         trickle: _Optional[_Union[TrickleRequest, _Mapping]] = ...,
         add_track: _Optional[_Union[AddTrackRequest, _Mapping]] = ...,
         mute: _Optional[_Union[MuteTrackRequest, _Mapping]] = ...,
@@ -303,25 +370,29 @@
         update_layers: _Optional[_Union[UpdateVideoLayers, _Mapping]] = ...,
         subscription_permission: _Optional[
             _Union[SubscriptionPermission, _Mapping]
         ] = ...,
         sync_state: _Optional[_Union[SyncState, _Mapping]] = ...,
         simulate: _Optional[_Union[SimulateScenario, _Mapping]] = ...,
         ping: _Optional[int] = ...,
+        update_metadata: _Optional[_Union[UpdateParticipantMetadata, _Mapping]] = ...,
+        ping_req: _Optional[_Union[Ping, _Mapping]] = ...,
     ) -> None: ...
 
 class SignalResponse(_message.Message):
     __slots__ = [
         "answer",
         "connection_quality",
         "join",
         "leave",
         "mute",
         "offer",
         "pong",
+        "pong_resp",
+        "reconnect",
         "refresh_token",
         "room_update",
         "speakers_changed",
         "stream_state_update",
         "subscribed_quality_update",
         "subscription_permission_update",
         "track_published",
@@ -332,14 +403,16 @@
     ANSWER_FIELD_NUMBER: _ClassVar[int]
     CONNECTION_QUALITY_FIELD_NUMBER: _ClassVar[int]
     JOIN_FIELD_NUMBER: _ClassVar[int]
     LEAVE_FIELD_NUMBER: _ClassVar[int]
     MUTE_FIELD_NUMBER: _ClassVar[int]
     OFFER_FIELD_NUMBER: _ClassVar[int]
     PONG_FIELD_NUMBER: _ClassVar[int]
+    PONG_RESP_FIELD_NUMBER: _ClassVar[int]
+    RECONNECT_FIELD_NUMBER: _ClassVar[int]
     REFRESH_TOKEN_FIELD_NUMBER: _ClassVar[int]
     ROOM_UPDATE_FIELD_NUMBER: _ClassVar[int]
     SPEAKERS_CHANGED_FIELD_NUMBER: _ClassVar[int]
     STREAM_STATE_UPDATE_FIELD_NUMBER: _ClassVar[int]
     SUBSCRIBED_QUALITY_UPDATE_FIELD_NUMBER: _ClassVar[int]
     SUBSCRIPTION_PERMISSION_UPDATE_FIELD_NUMBER: _ClassVar[int]
     TRACK_PUBLISHED_FIELD_NUMBER: _ClassVar[int]
@@ -349,14 +422,16 @@
     answer: SessionDescription
     connection_quality: ConnectionQualityUpdate
     join: JoinResponse
     leave: LeaveRequest
     mute: MuteTrackRequest
     offer: SessionDescription
     pong: int
+    pong_resp: Pong
+    reconnect: ReconnectResponse
     refresh_token: str
     room_update: RoomUpdate
     speakers_changed: SpeakersChanged
     stream_state_update: StreamStateUpdate
     subscribed_quality_update: SubscribedQualityUpdate
     subscription_permission_update: SubscriptionPermissionUpdate
     track_published: TrackPublishedResponse
@@ -382,41 +457,47 @@
         ] = ...,
         subscription_permission_update: _Optional[
             _Union[SubscriptionPermissionUpdate, _Mapping]
         ] = ...,
         refresh_token: _Optional[str] = ...,
         track_unpublished: _Optional[_Union[TrackUnpublishedResponse, _Mapping]] = ...,
         pong: _Optional[int] = ...,
+        reconnect: _Optional[_Union[ReconnectResponse, _Mapping]] = ...,
+        pong_resp: _Optional[_Union[Pong, _Mapping]] = ...,
     ) -> None: ...
 
 class SimulateScenario(_message.Message):
     __slots__ = [
         "migration",
         "node_failure",
         "server_leave",
         "speaker_update",
+        "subscriber_bandwidth",
         "switch_candidate_protocol",
     ]
     MIGRATION_FIELD_NUMBER: _ClassVar[int]
     NODE_FAILURE_FIELD_NUMBER: _ClassVar[int]
     SERVER_LEAVE_FIELD_NUMBER: _ClassVar[int]
     SPEAKER_UPDATE_FIELD_NUMBER: _ClassVar[int]
+    SUBSCRIBER_BANDWIDTH_FIELD_NUMBER: _ClassVar[int]
     SWITCH_CANDIDATE_PROTOCOL_FIELD_NUMBER: _ClassVar[int]
     migration: bool
     node_failure: bool
     server_leave: bool
     speaker_update: int
+    subscriber_bandwidth: int
     switch_candidate_protocol: CandidateProtocol
     def __init__(
         self,
         speaker_update: _Optional[int] = ...,
         node_failure: bool = ...,
         migration: bool = ...,
         server_leave: bool = ...,
         switch_candidate_protocol: _Optional[_Union[CandidateProtocol, str]] = ...,
+        subscriber_bandwidth: _Optional[int] = ...,
     ) -> None: ...
 
 class SimulcastCodec(_message.Message):
     __slots__ = ["cid", "codec", "enable_simulcast_layers"]
     CID_FIELD_NUMBER: _ClassVar[int]
     CODEC_FIELD_NUMBER: _ClassVar[int]
     ENABLE_SIMULCAST_LAYERS_FIELD_NUMBER: _ClassVar[int]
@@ -606,14 +687,24 @@
     target: SignalTarget
     def __init__(
         self,
         candidateInit: _Optional[str] = ...,
         target: _Optional[_Union[SignalTarget, str]] = ...,
     ) -> None: ...
 
+class UpdateParticipantMetadata(_message.Message):
+    __slots__ = ["metadata", "name"]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    metadata: str
+    name: str
+    def __init__(
+        self, metadata: _Optional[str] = ..., name: _Optional[str] = ...
+    ) -> None: ...
+
 class UpdateSubscription(_message.Message):
     __slots__ = ["participant_tracks", "subscribe", "track_sids"]
     PARTICIPANT_TRACKS_FIELD_NUMBER: _ClassVar[int]
     SUBSCRIBE_FIELD_NUMBER: _ClassVar[int]
     TRACK_SIDS_FIELD_NUMBER: _ClassVar[int]
     participant_tracks: _containers.RepeatedCompositeFieldContainer[
         _livekit_models_pb2.ParticipantTracks
@@ -626,35 +717,46 @@
         subscribe: bool = ...,
         participant_tracks: _Optional[
             _Iterable[_Union[_livekit_models_pb2.ParticipantTracks, _Mapping]]
         ] = ...,
     ) -> None: ...
 
 class UpdateTrackSettings(_message.Message):
-    __slots__ = ["disabled", "fps", "height", "quality", "track_sids", "width"]
+    __slots__ = [
+        "disabled",
+        "fps",
+        "height",
+        "priority",
+        "quality",
+        "track_sids",
+        "width",
+    ]
     DISABLED_FIELD_NUMBER: _ClassVar[int]
     FPS_FIELD_NUMBER: _ClassVar[int]
     HEIGHT_FIELD_NUMBER: _ClassVar[int]
+    PRIORITY_FIELD_NUMBER: _ClassVar[int]
     QUALITY_FIELD_NUMBER: _ClassVar[int]
     TRACK_SIDS_FIELD_NUMBER: _ClassVar[int]
     WIDTH_FIELD_NUMBER: _ClassVar[int]
     disabled: bool
     fps: int
     height: int
+    priority: int
     quality: _livekit_models_pb2.VideoQuality
     track_sids: _containers.RepeatedScalarFieldContainer[str]
     width: int
     def __init__(
         self,
         track_sids: _Optional[_Iterable[str]] = ...,
         disabled: bool = ...,
         quality: _Optional[_Union[_livekit_models_pb2.VideoQuality, str]] = ...,
         width: _Optional[int] = ...,
         height: _Optional[int] = ...,
         fps: _Optional[int] = ...,
+        priority: _Optional[int] = ...,
     ) -> None: ...
 
 class UpdateVideoLayers(_message.Message):
     __slots__ = ["layers", "track_sid"]
     LAYERS_FIELD_NUMBER: _ClassVar[int]
     TRACK_SID_FIELD_NUMBER: _ClassVar[int]
     layers: _containers.RepeatedCompositeFieldContainer[_livekit_models_pb2.VideoLayer]
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_webhook_pb2.py` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_webhook_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,18 @@
 
 
 from . import livekit_egress_pb2 as livekit__egress__pb2
 from . import livekit_ingress_pb2 as livekit__ingress__pb2
 from . import livekit_models_pb2 as livekit__models__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x15livekit_webhook.proto\x12\x07livekit\x1a\x14livekit_models.proto\x1a\x14livekit_egress.proto\x1a\x15livekit_ingress.proto"\x82\x02\n\x0cWebhookEvent\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x1b\n\x04room\x18\x02 \x01(\x0b\x32\r.livekit.Room\x12-\n\x0bparticipant\x18\x03 \x01(\x0b\x32\x18.livekit.ParticipantInfo\x12(\n\x0b\x65gress_info\x18\t \x01(\x0b\x32\x13.livekit.EgressInfo\x12*\n\x0cingress_info\x18\n \x01(\x0b\x32\x14.livekit.IngressInfo\x12!\n\x05track\x18\x08 \x01(\x0b\x32\x12.livekit.TrackInfo\x12\n\n\x02id\x18\x06 \x01(\t\x12\x12\n\ncreated_at\x18\x07 \x01(\x03\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
+    b'\n\x15livekit_webhook.proto\x12\x07livekit\x1a\x14livekit_models.proto\x1a\x14livekit_egress.proto\x1a\x15livekit_ingress.proto"\x97\x02\n\x0cWebhookEvent\x12\r\n\x05\x65vent\x18\x01 \x01(\t\x12\x1b\n\x04room\x18\x02 \x01(\x0b\x32\r.livekit.Room\x12-\n\x0bparticipant\x18\x03 \x01(\x0b\x32\x18.livekit.ParticipantInfo\x12(\n\x0b\x65gress_info\x18\t \x01(\x0b\x32\x13.livekit.EgressInfo\x12*\n\x0cingress_info\x18\n \x01(\x0b\x32\x14.livekit.IngressInfo\x12!\n\x05track\x18\x08 \x01(\x0b\x32\x12.livekit.TrackInfo\x12\n\n\x02id\x18\x06 \x01(\t\x12\x12\n\ncreated_at\x18\x07 \x01(\x03\x12\x13\n\x0bnum_dropped\x18\x0b \x01(\x05\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "livekit_webhook_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b"Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto"
     _WEBHOOKEVENT._serialized_start = 102
-    _WEBHOOKEVENT._serialized_end = 360
+    _WEBHOOKEVENT._serialized_end = 381
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/proto/livekit_webhook_pb2.pyi` & `livekit_server_sdk_python-1.0.0/livekit/_proto/livekit_webhook_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -14,31 +14,34 @@
 class WebhookEvent(_message.Message):
     __slots__ = [
         "created_at",
         "egress_info",
         "event",
         "id",
         "ingress_info",
+        "num_dropped",
         "participant",
         "room",
         "track",
     ]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
     EGRESS_INFO_FIELD_NUMBER: _ClassVar[int]
     EVENT_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     INGRESS_INFO_FIELD_NUMBER: _ClassVar[int]
+    NUM_DROPPED_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_FIELD_NUMBER: _ClassVar[int]
     ROOM_FIELD_NUMBER: _ClassVar[int]
     TRACK_FIELD_NUMBER: _ClassVar[int]
     created_at: int
     egress_info: _livekit_egress_pb2.EgressInfo
     event: str
     id: str
     ingress_info: _livekit_ingress_pb2.IngressInfo
+    num_dropped: int
     participant: _livekit_models_pb2.ParticipantInfo
     room: _livekit_models_pb2.Room
     track: _livekit_models_pb2.TrackInfo
     def __init__(
         self,
         event: _Optional[str] = ...,
         room: _Optional[_Union[_livekit_models_pb2.Room, _Mapping]] = ...,
@@ -48,8 +51,9 @@
         egress_info: _Optional[_Union[_livekit_egress_pb2.EgressInfo, _Mapping]] = ...,
         ingress_info: _Optional[
             _Union[_livekit_ingress_pb2.IngressInfo, _Mapping]
         ] = ...,
         track: _Optional[_Union[_livekit_models_pb2.TrackInfo, _Mapping]] = ...,
         id: _Optional[str] = ...,
         created_at: _Optional[int] = ...,
+        num_dropped: _Optional[int] = ...,
     ) -> None: ...
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit/twirp/livekit_analytics_twirp.py` & `livekit_server_sdk_python-1.0.0/livekit/_twirp/livekit_analytics_twirp.py`

 * *Files identical despite different names*

### Comparing `livekit_server_sdk_python-0.4.1/livekit/twirp/livekit_egress_twirp.py` & `livekit_server_sdk_python-1.0.0/livekit/_twirp/livekit_egress_twirp.py`

 * *Files identical despite different names*

### Comparing `livekit_server_sdk_python-0.4.1/livekit/twirp/livekit_ingress_twirp.py` & `livekit_server_sdk_python-1.0.0/livekit/_twirp/livekit_ingress_twirp.py`

 * *Files identical despite different names*

### Comparing `livekit_server_sdk_python-0.4.1/livekit/twirp/livekit_room_twirp.py` & `livekit_server_sdk_python-1.0.0/livekit/_twirp/livekit_room_twirp.py`

 * *Files identical despite different names*

### Comparing `livekit_server_sdk_python-0.4.1/livekit_server_sdk_python.egg-info/PKG-INFO` & `livekit_server_sdk_python-1.0.0/livekit_server_sdk_python.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-server-sdk-python
-Version: 0.4.1
+Version: 1.0.0
 Summary: Livekit Server SDK for Python
 Home-page: https://github.com/tradablebits/livekit-server-sdk-python
 Author: Tradable Bits
 Author-email: dev@tradablebits.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/tradablebits/livekit-server-sdk-python/issues
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,36 +20,43 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENCE
 
 # LiveKit Server SDK
 
 ![https://pypi.org/project/livekit-server-sdk-python/](https://img.shields.io/pypi/v/livekit-server-sdk-python.svg)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 API Reference: https://docs.livekit.io/guides/server-api
 
 ## Examples
 
 ### Generate Access Token for a Client
 
 ```py
-from livekit import AccessToken, VideoGrant
+import livekit
 
-grant = VideoGrant(room_join=True, room="My Cool Room")
-access_token = AccessToken("<api key>", "<api secret>", grant=grant, identity="bob", name="Bob")
+grant = livekit.VideoGrant(room_join=True, room="My Cool Room")
+access_token = livekit.AccessToken("<api key>", "<api secret>", grant=grant, identity="bob", name="Bob")
 token = access_token.to_jwt()
 ```
 
 ### Using `RoomServiceClient`
 
 ```py
-from livekit import RoomServiceClient
+import livekit
 
-client = RoomServiceClient("<host>", "<api key>", "<api secret>")
-client.mute_published_track(room="<room name>", track="<track sid>")
+client = livekit.RoomServiceClient("<host>", "<api key>", "<api secret>")
+client.mute_published_track(
+    room="<room name>",
+    identity="Bob",
+    track_sid="<track sid>",
+    muted=True,
+)
 ```
 
 ## Local Development
 
 Make sure you clone with submodules:
 ```sh
 $ git clone --recurse-submodules https://github.com/tradablebits/livekit-server-sdk-python.git
```

### Comparing `livekit_server_sdk_python-0.4.1/livekit_server_sdk_python.egg-info/SOURCES.txt` & `livekit_server_sdk_python-1.0.0/livekit_server_sdk_python.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,53 @@
 LICENCE
 README.md
 pyproject.toml
 setup.cfg
 livekit/__init__.py
-livekit/utils.py
-livekit/proto/__init__.py
-livekit/proto/livekit_analytics_pb2.py
-livekit/proto/livekit_analytics_pb2.pyi
-livekit/proto/livekit_egress_pb2.py
-livekit/proto/livekit_egress_pb2.pyi
-livekit/proto/livekit_ingress_pb2.py
-livekit/proto/livekit_ingress_pb2.pyi
-livekit/proto/livekit_internal_pb2.py
-livekit/proto/livekit_internal_pb2.pyi
-livekit/proto/livekit_models_pb2.py
-livekit/proto/livekit_models_pb2.pyi
-livekit/proto/livekit_room_pb2.py
-livekit/proto/livekit_room_pb2.pyi
-livekit/proto/livekit_rpc_internal_pb2.py
-livekit/proto/livekit_rpc_internal_pb2.pyi
-livekit/proto/livekit_rtc_pb2.py
-livekit/proto/livekit_rtc_pb2.pyi
-livekit/proto/livekit_webhook_pb2.py
-livekit/proto/livekit_webhook_pb2.pyi
-livekit/twirp/__init__.py
-livekit/twirp/livekit_analytics_twirp.py
-livekit/twirp/livekit_egress_twirp.py
-livekit/twirp/livekit_ingress_twirp.py
-livekit/twirp/livekit_internal_twirp.py
-livekit/twirp/livekit_models_twirp.py
-livekit/twirp/livekit_room_twirp.py
-livekit/twirp/livekit_rpc_internal_twirp.py
-livekit/twirp/livekit_rtc_twirp.py
-livekit/twirp/livekit_webhook_twirp.py
+livekit/_utils.py
+livekit/analytics.py
+livekit/egress.py
+livekit/ingress.py
+livekit/internal.py
+livekit/models.py
+livekit/room.py
+livekit/rpc_internal.py
+livekit/rtc.py
+livekit/twirp.py
+livekit/webhook.py
+livekit/_proto/__init__.py
+livekit/_proto/livekit_analytics_pb2.py
+livekit/_proto/livekit_analytics_pb2.pyi
+livekit/_proto/livekit_egress_pb2.py
+livekit/_proto/livekit_egress_pb2.pyi
+livekit/_proto/livekit_ingress_pb2.py
+livekit/_proto/livekit_ingress_pb2.pyi
+livekit/_proto/livekit_internal_pb2.py
+livekit/_proto/livekit_internal_pb2.pyi
+livekit/_proto/livekit_models_pb2.py
+livekit/_proto/livekit_models_pb2.pyi
+livekit/_proto/livekit_room_pb2.py
+livekit/_proto/livekit_room_pb2.pyi
+livekit/_proto/livekit_rpc_internal_pb2.py
+livekit/_proto/livekit_rpc_internal_pb2.pyi
+livekit/_proto/livekit_rtc_pb2.py
+livekit/_proto/livekit_rtc_pb2.pyi
+livekit/_proto/livekit_webhook_pb2.py
+livekit/_proto/livekit_webhook_pb2.pyi
+livekit/_twirp/__init__.py
+livekit/_twirp/livekit_analytics_twirp.py
+livekit/_twirp/livekit_egress_twirp.py
+livekit/_twirp/livekit_ingress_twirp.py
+livekit/_twirp/livekit_internal_twirp.py
+livekit/_twirp/livekit_models_twirp.py
+livekit/_twirp/livekit_room_twirp.py
+livekit/_twirp/livekit_rpc_internal_twirp.py
+livekit/_twirp/livekit_rtc_twirp.py
+livekit/_twirp/livekit_webhook_twirp.py
 livekit_server_sdk_python.egg-info/PKG-INFO
 livekit_server_sdk_python.egg-info/SOURCES.txt
 livekit_server_sdk_python.egg-info/dependency_links.txt
 livekit_server_sdk_python.egg-info/requires.txt
-livekit_server_sdk_python.egg-info/top_level.txt
+livekit_server_sdk_python.egg-info/top_level.txt
+tests/test_access_token.py
+tests/test_room_service_client.py
+tests/test_utils.py
```

### Comparing `livekit_server_sdk_python-0.4.1/setup.cfg` & `livekit_server_sdk_python-1.0.0/setup.cfg`

 * *Files identical despite different names*

