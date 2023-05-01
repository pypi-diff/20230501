# Comparing `tmp/p2pd-2.3.6.tar.gz` & `tmp/p2pd-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p2pd-2.3.6.tar", last modified: Sat Apr 29 16:38:35 2023, max compression
+gzip compressed data, was "p2pd-2.4.0.tar", last modified: Mon May  1 10:41:31 2023, max compression
```

## Comparing `p2pd-2.3.6.tar` & `p2pd-2.4.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-04-29 16:38:35.299638 p2pd-2.3.6/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1570 2023-04-28 06:42:33.000000 p2pd-2.3.6/CREDITS.md
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1072 2023-04-28 06:42:33.000000 p2pd-2.3.6/LICENSE
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      106 2023-04-29 16:38:16.000000 p2pd-2.3.6/MANIFEST.in
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5084 2023-04-29 16:38:35.299638 p2pd-2.3.6/PKG-INFO
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4543 2023-04-28 06:42:33.000000 p2pd-2.3.6/README.md
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-04-29 16:38:35.295637 p2pd-2.3.6/p2pd/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1196 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/__init__.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7065 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/ack_udp.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6437 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/address.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    30486 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/base_stream.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8028 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/clock_skew.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8004 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/cmd_tools.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7896 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/daemon.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      303 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/echo_server.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      222 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/errors.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2465 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/http_client_lib.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5968 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/http_server_lib.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    19527 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/interface.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    11971 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/ip_range.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    27256 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/nat.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    22921 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/net.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4438 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/netiface_extra.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13973 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/ntp_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6624 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/p2p_addr.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13199 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/p2p_node.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    26320 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/p2p_pipe.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    15517 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/p2p_protocol.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2986 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/p2p_utils.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13146 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/rest_api.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    32854 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/route.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5992 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/route_table.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7094 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/settings.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/signaling.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    42083 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/stun_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    40903 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/tcp_punch.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4366 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/test_init.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16867 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/turn_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13940 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/turn_defs.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    10862 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/turn_process.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13894 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/upnp.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16078 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/utils.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1027 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/var_names.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4220 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/win_net.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16718 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/win_netifaces.py
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-04-29 16:38:35.295637 p2pd-2.3.6/p2pd.egg-info/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5084 2023-04-29 16:38:35.000000 p2pd-2.3.6/p2pd.egg-info/PKG-INFO
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1482 2023-04-29 16:38:35.000000 p2pd-2.3.6/p2pd.egg-info/SOURCES.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        1 2023-04-29 16:38:35.000000 p2pd-2.3.6/p2pd.egg-info/dependency_links.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      103 2023-04-29 16:38:35.000000 p2pd-2.3.6/p2pd.egg-info/requires.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        5 2023-04-29 16:38:35.000000 p2pd-2.3.6/p2pd.egg-info/top_level.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      305 2023-04-28 06:42:33.000000 p2pd-2.3.6/requirements.txt
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)       38 2023-04-29 16:38:35.299638 p2pd-2.3.6/setup.cfg
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1161 2023-04-29 16:23:03.000000 p2pd-2.3.6/setup.py
-drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-04-29 16:38:35.299638 p2pd-2.3.6/tests/
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1090 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_address.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4111 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_bind.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      735 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_clock_skew.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5211 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_cmd.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5111 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_daemon.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_interface.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5161 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_ip_range.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7449 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_nat.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2016 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_net.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2038 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_net_afs.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      394 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_p2p_addr.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8187 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_p2p_pipe.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2759 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_p2pd_server.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9323 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_route.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1618 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_route_table.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1406 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_rudp.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1377 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_signaling.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1545 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_sock.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      992 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_sorted_search.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3355 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_stun_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5617 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_tcp_punch.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3537 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_turn_client.py
--rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2823 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_win_netifaces.py
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-01 10:41:31.788418 p2pd-2.4.0/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1570 2023-04-28 06:42:33.000000 p2pd-2.4.0/CREDITS.md
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1072 2023-04-28 06:42:33.000000 p2pd-2.4.0/LICENSE
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      106 2023-04-29 16:38:16.000000 p2pd-2.4.0/MANIFEST.in
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-05-01 10:41:31.788418 p2pd-2.4.0/PKG-INFO
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2707 2023-04-30 09:46:56.000000 p2pd-2.4.0/README.md
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-01 10:41:31.780418 p2pd-2.4.0/p2pd/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1196 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/__init__.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7065 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/ack_udp.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6437 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/address.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    30486 2023-04-30 16:44:28.000000 p2pd-2.4.0/p2pd/base_stream.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8028 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/clock_skew.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8004 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/cmd_tools.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7896 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/daemon.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      303 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/echo_server.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      222 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/errors.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2465 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/http_client_lib.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5968 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/http_server_lib.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    19527 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/interface.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    11971 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/ip_range.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    27256 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/nat.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    22921 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/net.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4438 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/netiface_extra.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13979 2023-04-30 16:20:59.000000 p2pd-2.4.0/p2pd/ntp_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6624 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/p2p_addr.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13522 2023-04-30 18:20:16.000000 p2pd-2.4.0/p2pd/p2p_node.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    26320 2023-04-30 18:46:46.000000 p2pd-2.4.0/p2pd/p2p_pipe.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    15517 2023-04-30 18:46:55.000000 p2pd-2.4.0/p2pd/p2p_protocol.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3072 2023-04-30 18:51:57.000000 p2pd-2.4.0/p2pd/p2p_utils.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13146 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/rest_api.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    32854 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/route.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5992 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/route_table.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7128 2023-05-01 10:13:00.000000 p2pd-2.4.0/p2pd/settings.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/signaling.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    42083 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/stun_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    40903 2023-04-30 18:50:50.000000 p2pd-2.4.0/p2pd/tcp_punch.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4366 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/test_init.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    17104 2023-04-30 16:09:18.000000 p2pd-2.4.0/p2pd/turn_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13940 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/turn_defs.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    10862 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/turn_process.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13894 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/upnp.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16306 2023-04-30 18:46:00.000000 p2pd-2.4.0/p2pd/utils.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1027 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/var_names.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4220 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/win_net.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16718 2023-04-28 06:42:33.000000 p2pd-2.4.0/p2pd/win_netifaces.py
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-01 10:41:31.780418 p2pd-2.4.0/p2pd.egg-info/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3248 2023-05-01 10:41:31.000000 p2pd-2.4.0/p2pd.egg-info/PKG-INFO
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1508 2023-05-01 10:41:31.000000 p2pd-2.4.0/p2pd.egg-info/SOURCES.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        1 2023-05-01 10:41:31.000000 p2pd-2.4.0/p2pd.egg-info/dependency_links.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      103 2023-05-01 10:41:31.000000 p2pd-2.4.0/p2pd.egg-info/requires.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        5 2023-05-01 10:41:31.000000 p2pd-2.4.0/p2pd.egg-info/top_level.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      305 2023-04-28 06:42:33.000000 p2pd-2.4.0/requirements.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)       38 2023-05-01 10:41:31.788418 p2pd-2.4.0/setup.cfg
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1161 2023-04-30 08:33:33.000000 p2pd-2.4.0/setup.py
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-05-01 10:41:31.788418 p2pd-2.4.0/tests/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1090 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_address.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4111 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_bind.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      735 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_clock_skew.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5211 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_cmd.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5111 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_daemon.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_interface.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5161 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_ip_range.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7449 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_nat.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2016 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_net.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2793 2023-05-01 10:08:47.000000 p2pd-2.4.0/tests/test_net_afs.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      394 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_p2p_addr.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8499 2023-05-01 10:27:39.000000 p2pd-2.4.0/tests/test_p2p_pipe.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2759 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_p2pd_server.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1214 2023-04-30 19:03:31.000000 p2pd-2.4.0/tests/test_py_examples.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9323 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_route.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1618 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_route_table.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1406 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_rudp.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1443 2023-05-01 10:23:09.000000 p2pd-2.4.0/tests/test_signaling.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1544 2023-04-30 19:07:17.000000 p2pd-2.4.0/tests/test_sock.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      992 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_sorted_search.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3355 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_stun_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5614 2023-04-30 19:14:54.000000 p2pd-2.4.0/tests/test_tcp_punch.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3559 2023-05-01 10:20:05.000000 p2pd-2.4.0/tests/test_turn_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2823 2023-04-28 06:42:33.000000 p2pd-2.4.0/tests/test_win_netifaces.py
```

### Comparing `p2pd-2.3.6/CREDITS.md` & `p2pd-2.4.0/CREDITS.md`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/LICENSE` & `p2pd-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/__init__.py` & `p2pd-2.4.0/p2pd/__init__.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/ack_udp.py` & `p2pd-2.4.0/p2pd/ack_udp.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/address.py` & `p2pd-2.4.0/p2pd/address.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/base_stream.py` & `p2pd-2.4.0/p2pd/base_stream.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/clock_skew.py` & `p2pd-2.4.0/p2pd/clock_skew.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/cmd_tools.py` & `p2pd-2.4.0/p2pd/cmd_tools.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/daemon.py` & `p2pd-2.4.0/p2pd/daemon.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/http_client_lib.py` & `p2pd-2.4.0/p2pd/http_client_lib.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/http_server_lib.py` & `p2pd-2.4.0/p2pd/http_server_lib.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/interface.py` & `p2pd-2.4.0/p2pd/interface.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/ip_range.py` & `p2pd-2.4.0/p2pd/ip_range.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/nat.py` & `p2pd-2.4.0/p2pd/nat.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/net.py` & `p2pd-2.4.0/p2pd/net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/netiface_extra.py` & `p2pd-2.4.0/p2pd/netiface_extra.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/ntp_client.py` & `p2pd-2.4.0/p2pd/ntp_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,20 +307,20 @@
 
             # wait for the response - check the source address
             response_packet = await pipe.recv(timeout=timeout)
 
             # build the destination timestamp
             dest_timestamp = system_to_ntp_time(time.time())
         except asyncio.TimeoutError:
-            await pipe.close()
             raise NTPException("No response received from %s." % host)
         except Exception as e:
             log_exception()
         finally:
-            await pipe.close()
+            if pipe is not None:
+                await pipe.close()
 
         # construct corresponding statistics
         stats = NTPStats()
         stats.from_data(response_packet)
         stats.dest_timestamp = dest_timestamp
         return stats
```

### Comparing `p2pd-2.3.6/p2pd/p2p_addr.py` & `p2pd-2.4.0/p2pd/p2p_addr.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/p2p_node.py` & `p2pd-2.4.0/p2pd/p2p_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import gc
 from concurrent.futures import ProcessPoolExecutor
 import multiprocessing
 from decimal import Decimal as Dec
 from .p2p_pipe import *
 from .daemon import *
 from .p2p_protocol import *
 from .signaling import *
@@ -317,14 +318,25 @@
         # Try close the process pool executor.
         try:
             if self.pp_executor is not None:
                 self.pp_executor.shutdown()
         except Exception:
             pass
 
+        """
+        Node close will throw: 
+        Exception ignored in: <function BaseEventLoop.__del__
+        with socket error -1
+
+        So you need to make sure to wrap coroutines for exceptions.
+        """
+        self.mp_manager = None
+        self.pp_executor = None
+        await asyncio.sleep(.25)
+
 if __name__ == "__main__": # pragma: no cover
     from .p2p_pipe import P2PPipe, P2P_DIRECT, P2P_REVERSE, P2P_PUNCH, P2P_RELAY
     from .nat import *
     async def test_p2p_node():
         sys_clock = SysClock(Dec("-0.02839018452552057081653225806"))
         pp_executor = ProcessPoolExecutor()
         mp_manager = multiprocessing.Manager()
```

### Comparing `p2pd-2.3.6/p2pd/p2p_pipe.py` & `p2pd-2.4.0/p2pd/p2p_pipe.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/p2p_protocol.py` & `p2pd-2.4.0/p2pd/p2p_protocol.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/p2p_utils.py` & `p2pd-2.4.0/p2pd/p2p_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,17 @@
     # Make selector default event loop.
     # On Windows this changes it from proactor to selector.
     asyncio.set_event_loop_policy(SelectorEventPolicy())
 
     # Create new event loop in the process.
     loop = asyncio.get_event_loop()
 
+    # Handle exceptions on close.
+    loop.set_exception_handler(handle_exceptions)
+
 async def get_pp_executors(workers=2):
     try:
         pp_executor = ProcessPoolExecutor(max_workers=workers)
     except Exception:
         """
         Not all platform have a working implementation of sem_open / semaphores.
         Android is one such platform. It does support multiprocessing but
@@ -29,15 +32,15 @@
         tasks.append(loop.run_in_executor(
             pp_executor, init_process_pool
         ))
     await asyncio.gather(*tasks)
     return pp_executor
 
 # delay with sys clock and get_pp_executors.
-async def start_p2p_node(port=NODE_PORT, node_id=None, ifs=None, clock_skew=Dec(0), ip=None, pp_executors=None, enable_upnp=False, signal_offsets=None, netifaces=None):
+async def start_p2p_node(port=NODE_PORT, node_id=None, ifs=None, clock_skew=Dec(0), ip=None, pp_executors=False, enable_upnp=False, signal_offsets=None, netifaces=None):
     # Load NAT info for interface.
     ifs = ifs or await load_interfaces(netifaces=netifaces)
     assert(len(ifs))
     for interface in ifs:
         # Don't set NAT details if already set.
         if interface.resolved:
             continue
```

### Comparing `p2pd-2.3.6/p2pd/rest_api.py` & `p2pd-2.4.0/p2pd/rest_api.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/route.py` & `p2pd-2.4.0/p2pd/route.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/route_table.py` & `p2pd-2.4.0/p2pd/route_table.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/settings.py` & `p2pd-2.4.0/p2pd/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from .net import IP4, IP6
 
+P2PD_TEST_INFRASTRUCTURE = False
+
 """
 To keep things simple P2PD uses a number of services to
 help facilitate peer-to-peer connections. At the moment
 there is no massive list of servers to use because
 (as I've learned) -- you need to also have a way to
 monitor the integrity of servers to provide high-quality
 server lists to peers. That would be too complex to provide
```

### Comparing `p2pd-2.3.6/p2pd/signaling.py` & `p2pd-2.4.0/p2pd/signaling.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/stun_client.py` & `p2pd-2.4.0/p2pd/stun_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/tcp_punch.py` & `p2pd-2.4.0/p2pd/tcp_punch.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/test_init.py` & `p2pd-2.4.0/p2pd/test_init.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/turn_client.py` & `p2pd-2.4.0/p2pd/turn_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,20 @@
         self.state = state
 
     def new_node_event(self, node_id):
         self.node_events[to_s(node_id)] = asyncio.Event()
 
     # Overwrite the BaseProto send method and require ACKs.
     async def send(self, data, dest_tup):
+        # Detect invalid self-send.
+        if self.relay_tup_future.done():
+            relay_tup = await self.relay_tup_future
+            if dest_tup == relay_tup:
+                raise Exception("Coturn doesn't support self-send.")
+
         # Make sure the channel is setup before continuing.
         task = asyncio.create_task(
             async_wrap_errors(
                 self.stream.ack_send(
                     data,
                     dest_tup
                 )
```

### Comparing `p2pd-2.3.6/p2pd/turn_defs.py` & `p2pd-2.4.0/p2pd/turn_defs.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/turn_process.py` & `p2pd-2.4.0/p2pd/turn_process.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/upnp.py` & `p2pd-2.4.0/p2pd/upnp.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/utils.py` & `p2pd-2.4.0/p2pd/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -532,26 +532,35 @@
         else:
             loop = asyncio.get_event_loop()
     else:
         loop = loop()
 
     return loop
 
+# Handle stray exceptions in the event loop.
+def handle_exceptions(loop, context):
+    pass
+
 # Will be used in sample code to avoid boilerplate.
 def async_test(f, args=[], loop=None):
     #uvloop.install()
     loop = get_loop(loop)
     #if IS_DEBUG:
     #    loop.set_debug(True)
     loop.set_debug(False)
-    if len(args):
-        loop.run_until_complete(f(*args))
-    else:
-        loop.run_until_complete(f())
-    loop.close()
+
+    # Can have cleanup errors.
+    try:
+        if len(args):
+            loop.run_until_complete(async_wrap_errors(f(*args)))
+        else:
+            loop.run_until_complete(async_wrap_errors(f()))
+        loop.close()
+    except:
+        log_exception()
 
 async def return_true(result=None):
     return True
             
 # If there's an error that its already in a loop
 # Run nest_asyncio.apply()
 def async_to_sync(f, params=None, loop=None):
```

### Comparing `p2pd-2.3.6/p2pd/var_names.py` & `p2pd-2.4.0/p2pd/var_names.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/win_net.py` & `p2pd-2.4.0/p2pd/win_net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd/win_netifaces.py` & `p2pd-2.4.0/p2pd/win_netifaces.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/p2pd.egg-info/SOURCES.txt` & `p2pd-2.4.0/p2pd.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 tests/test_ip_range.py
 tests/test_nat.py
 tests/test_net.py
 tests/test_net_afs.py
 tests/test_p2p_addr.py
 tests/test_p2p_pipe.py
 tests/test_p2pd_server.py
+tests/test_py_examples.py
 tests/test_route.py
 tests/test_route_table.py
 tests/test_rudp.py
 tests/test_signaling.py
 tests/test_sock.py
 tests/test_sorted_search.py
 tests/test_stun_client.py
```

### Comparing `p2pd-2.3.6/setup.py` & `p2pd-2.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     install_reqs = f.read().splitlines()
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
-    version='2.3.6',
+    version='2.4.0',
     name='p2pd',
     description='Asynchronous P2P networking library and service',
     keywords=('NAT traversal, TCP hole punching, simultaneous open, UPnP, STUN, TURN, SIP, DHCP, add IP to interface, NATPMP, P2P, Peer-to-peer networking library, python'),
     long_description_content_type="text/markdown",
     long_description=long_description,
     url='http://github.com/robertsdotpm/p2pd',
     author='Matthew Roberts',
```

### Comparing `p2pd-2.3.6/tests/test_address.py` & `p2pd-2.4.0/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/tests/test_bind.py` & `p2pd-2.4.0/tests/test_bind.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/tests/test_clock_skew.py` & `p2pd-2.4.0/tests/test_clock_skew.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/tests/test_cmd.py` & `p2pd-2.4.0/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/tests/test_daemon.py` & `p2pd-2.4.0/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/tests/test_interface.py` & `p2pd-2.4.0/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/tests/test_ip_range.py` & `p2pd-2.4.0/tests/test_ip_range.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/tests/test_nat.py` & `p2pd-2.4.0/tests/test_nat.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/tests/test_net.py` & `p2pd-2.4.0/tests/test_net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/tests/test_net_afs.py` & `p2pd-2.4.0/tests/test_net_afs.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,57 +12,84 @@
 from p2pd import IPRange, Bind, Route, Interface, pipe_open
 from p2pd import Address
 from p2pd.net import BLACK_HOLE_IPS, ip_norm, DUEL_STACK, IP6, IP4
 from p2pd.net import NIC_BIND, EXT_BIND, VALID_AFS, TCP, UDP
 from p2pd.base_stream import SUB_ALL
 
 asyncio.set_event_loop_policy(SelectorEventPolicy())
+
 class TestAFsWork(unittest.IsolatedAsyncioTestCase):
     async def test_afs(self):
-        # Public IPs.
         # The BSD inetd seems broken for echo / udp / localhost bind.
         await init_p2pd()
-        echo_ip = {
-            IP4: P2PD_NET_V4_IP,
-            IP6: P2PD_NET_V6_IP
+
+        # List of public echo servers.
+        addr = {
+            UDP: {
+                IP4: {
+                    "host": "52.43.121.77",
+                    "port": 10001
+                },
+                # TODO: Find IPv6 UDP public echo server.
+            },
+            TCP: {
+                IP4: {
+                    "host": "tcpbin.com",
+                    "port": 4242
+                },
+                IP6: {
+                    "host": "tcpbin.com",
+                    "port": 4242
+                }
+            }
         }
 
+        # Test all available AFs + protos.
         one_worked = False
         for af in VALID_AFS:
             try:
                 # Get default Interface for AF type.
                 i = Interface(af)
                 rp = use_fixed_rp(i)
                 await i.start(rp)
                 one_worked = True
             except Exception:
                 # Skip test if not supported.
                 continue
 
             # Echo server address.
             route = await i.route(af).bind()
-            echo_dest = await Address(echo_ip[af], 7, route).res()
 
             # Test echo server with AF.
-            msg = b"echo test\r\n"
+            msg = b"echo test"
             for proto in [TCP, UDP]:
+                # No server for this AF + proto.
+                if af not in addr[proto]:
+                    continue
+
+                # Set destination of echo server.
+                echo_dest = await Address(
+                    addr[proto][af]["host"],
+                    addr[proto][af]["port"],
+                    route
+                ).res()
+
+                # Open pipe to echo server.
                 pipe = await pipe_open(proto, echo_dest, route)
                 
                 # Interested in any message.
                 pipe.subscribe(SUB_ALL)
 
                 # Send data down the pipe.
-                await pipe.send(msg, echo_dest.tup)
+                for i in range(0, 4):
+                    await pipe.send(msg + b"\r\n", echo_dest.tup)
 
                 # Receive data back.
                 data = await pipe.recv(SUB_ALL, 4)
-                self.assertEqual(data, msg)
-
-                # Test block match.
-                await pipe.send(msg, echo_dest.tup)
+                assert(msg in data)
 
                 # Cleanup.
                 await pipe.close()
 
         self.assertTrue(one_worked)
 
 if __name__ == '__main__':
```

### Comparing `p2pd-2.3.6/tests/test_p2p_pipe.py` & `p2pd-2.4.0/tests/test_p2p_pipe.py`

 * *Files 16% similar despite different names*

```diff
@@ -62,15 +62,17 @@
     return node_a, node_b
 
 async def test_cleanup(node_a, node_b):
     await node_a.close()
     await node_b.close()
 
 class TestP2PPipe(unittest.IsolatedAsyncioTestCase):
+    # Self connect won't work due to Coturn changes.
     async def test_self_turn_connect(self):
+        return
         log(">>> test_self_turn_connect")
         node_a, node_b = await test_setup()
         pipe, _ = await node_a.connect(
             node_b.address(),
             strategies=[P2P_RELAY]
         )
 
@@ -140,14 +142,17 @@
         # Test pipe is valid.
         pipe_okay = await check_pipe(pipe)
         self.assertTrue(pipe_okay)
         await pipe.close()
         await test_cleanup(node_a, node_b)
 
     async def test_remote_direct_connect(self):
+        if not P2PD_TEST_INFRASTRUCTURE:
+            return
+
         # Test direct connect
         log(">>> test_remote_direct_connect")
         node_a, node_b = await test_setup()
         pipe, _ = await node_a.connect(
             P2PD_NET_ADDR_BYTES,
             strategies=[P2P_DIRECT]
         )
@@ -176,14 +181,17 @@
             print("Test is optional but mentioning it.")
 
         if pipe is not None:
             await pipe.close()
         await test_cleanup(node_a, node_b)
 
     async def test_remote_reverse_connect(self):
+        if not P2PD_TEST_INFRASTRUCTURE:
+            return
+
         # Test reverse connect.
         log(">>> test_remote_reverse_connect")
         node_a, node_b = await test_setup()
         found_open = False
         for interface in node_a.if_list:
             if interface.nat["type"] == OPEN_INTERNET:
                 pipe, _ = await node_a.connect(
@@ -202,14 +210,17 @@
         if not found_open:
             print("> Skipping reverse connect test")
             print("> NAT type is not open.\r\n")
 
         await test_cleanup(node_a, node_b)
 
     async def test_remote_punch(self):
+        if not P2PD_TEST_INFRASTRUCTURE:
+            return
+
         # If P2PD_NET_ADDR_BYTES is not us then test punching to it.
         log(">>> test_remote_punch")
         node_a, node_b = await test_setup()
         if not is_p2p_addr_us(P2PD_NET_ADDR_BYTES, node_a.if_list):
             # Connect to p2pd.net test server.
             pipe, _ = await node_a.connect(
                 P2PD_NET_ADDR_BYTES,
@@ -223,14 +234,17 @@
             await pipe.close()
         else:
             print("> p2pd net addr is us. Skipping remote punch test.")
 
         await test_cleanup(node_a, node_b)
 
     async def test_remote_turn_connect(self):
+        if not P2PD_TEST_INFRASTRUCTURE:
+            return
+
         log(">>> test_remote_turn_connect")
         node_a, node_b = await test_setup()
         pipe, _ = await node_a.connect(
             P2PD_NET_ADDR_BYTES,
             strategies=[P2P_RELAY]
         )
```

### Comparing `p2pd-2.3.6/tests/test_p2pd_server.py` & `p2pd-2.4.0/tests/test_p2pd_server.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/tests/test_route.py` & `p2pd-2.4.0/tests/test_route.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/tests/test_route_table.py` & `p2pd-2.4.0/tests/test_route_table.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/tests/test_rudp.py` & `p2pd-2.4.0/tests/test_rudp.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/tests/test_signaling.py` & `p2pd-2.4.0/tests/test_signaling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from p2pd.test_init import *
 from p2pd.settings import *
 from p2pd.signaling import SignalMock
 from p2pd.utils import rand_plain, to_s
 
 class TestSignaling(unittest.IsolatedAsyncioTestCase):
-    async def test_signaling(self):
+    async def test_node_signaling(self):
+        if not P2PD_TEST_INFRASTRUCTURE:
+            return
+
         # Channel that the test node subs to.
         await init_p2pd()
         dest_id = "p2pd_test_node"
         msg = "msggg"
         f = asyncio.Future()
 
         # Receive a message from our MQTT channel (node ID.)
```

### Comparing `p2pd-2.3.6/tests/test_sock.py` & `p2pd-2.4.0/tests/test_sock.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 
     async def test_socket_factory_connect(self):
         await init_p2pd()
         loop = asyncio.get_event_loop()
         i = await Interface().start_local()
         af = i.supported()[0]
         r = await i.route(af).bind()
-        d = await Address("p2pd.net", 34780, r, UDP).res()
-        s = await socket_factory(r, dest_addr=d, sock_type=UDP)
+        d = await Address("google.com", 80, r, TCP).res()
+        s = await socket_factory(r, dest_addr=d, sock_type=TCP)
         await loop.sock_connect(
             s, 
             d.tup
         )
 
         if s is not None:
             s.close()
```

### Comparing `p2pd-2.3.6/tests/test_sorted_search.py` & `p2pd-2.4.0/tests/test_sorted_search.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/tests/test_stun_client.py` & `p2pd-2.4.0/tests/test_stun_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.6/tests/test_tcp_punch.py` & `p2pd-2.4.0/tests/test_tcp_punch.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,30 +115,30 @@
             their_maps=r_maps,
             stun_client=stun_client
         )
 
         #print(i_client.state)
 
         try:
-            results = await asyncio.wrait_for(
+            results = await asyncio.wait_for(
                 asyncio.gather(
                     async_wrap_errors(
                         i_client.proto_do_punching(PUNCH_INITIATOR, r_node_id, pipe_id)
                     ),
                     async_wrap_errors(
                         r_client.proto_do_punching(PUNCH_RECIPIENT, i_node_id, pipe_id)
                     )
                 ),
                 10
             )
         except Exception:
             results = []
 
-        #print("Got results = ")
-        #print(results)
+        print("Got results = ")
+        print(results)
 
         async def process_results(results):
             if len(results) != 2:
                 return False
 
             msg = b"a test msg"
             for pipe in results:
```

### Comparing `p2pd-2.3.6/tests/test_turn_client.py` & `p2pd-2.4.0/tests/test_turn_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,20 @@
 from p2pd.http_client_lib import *
 
 asyncio.set_event_loop_policy(SelectorEventPolicy())
 class TestTurn(unittest.IsolatedAsyncioTestCase):
     async def test_turn(self):
         #print(sys.modules.keys())
         # Network interface details.
-        await init_p2pd()
         log(">>> test_turn")
         n = 0
-        i = await Interface().start_local()
+        netifaces = await init_p2pd()
+        i = await Interface(netifaces=netifaces).start_local()
         af = i.supported()[0]
         r = await i.route(af).bind()
-        
-        # Will be used to send packets from.
-        dest_p2pd = await Address(
-            "p2pd.net",
-            20000,
-            r
-        ).res()
 
         # Address of a TURN server.
         dest = await Address(
             TURN_SERVERS[n]["host"],
             TURN_SERVERS[n]["port"],
             r
         ).res()
@@ -51,65 +44,66 @@
 
         # The external address of ourself seen by the TURN server.
         client_tup = await client.client_tup_future
 
         # The relay address used to reach our peer at the TURN server.
         relay_tup = await client.relay_tup_future
 
-        # Whitelist rest API.
-        p2pd_tup = dest_p2pd.tup
-        await client.accept_peer(p2pd_tup, p2pd_tup)
-
-        # Interested in any messages to queue.
-        client.subscribe(SUB_ALL)
+        if P2PD_TEST_INFRASTRUCTURE:
+            # Will be used to send packets from.
+            dest_p2pd = await Address(
+                "p2pd.net",
+                20000,
+                r
+            ).res()
+
+            # Whitelist rest API.
+            p2pd_tup = dest_p2pd.tup
+            await client.accept_peer(p2pd_tup, p2pd_tup)
+
+            # Interested in any messages to queue.
+            client.subscribe(SUB_ALL)
+
+            #await client.accept_peer(client_tup, relay_tup)
+            #await client.accept_peer(relay_tup, relay_tup)
+            """
+            m = TurnMessage(msg_type=TurnMessageMethod.SendResponse, msg_code=TurnMessageCode.Request)
+            m.write_attr(
+                TurnAttribute.Data,
+                b"test message to send."
+            )
+            buf, _ = TurnMessage.unpack(m.encode())
+            buf.write_credential(client.turn_user, client.realm, client.nonce)
+            buf.write_hmac(client.key)
+            """
+
+
+            # Attempt to get a reply at our relay address.
+            # Do it up to 3 times due to UDP being unreliable.
+            got_reply = False
+            for i in range(0, 3):
+                http_route = copy.deepcopy(r)
+                await http_route.bind()
+                rest_path = f"/hello/udp/{relay_tup[0]}/{relay_tup[1]}/{dest_p2pd.tup[0]}/63248"
+                _, resp = await http_req(http_route, dest_p2pd, rest_path)
+
+                # Attempt to read the message back.
+                out = await client.recv(SUB_ALL, 2)
+                if out == b"hello":
+                    got_reply = True
+                    break
 
-        
-        #await client.accept_peer(client_tup, relay_tup)
-        #await client.accept_peer(relay_tup, relay_tup)
-        """
-        m = TurnMessage(msg_type=TurnMessageMethod.SendResponse, msg_code=TurnMessageCode.Request)
-        m.write_attr(
-            TurnAttribute.Data,
-            b"test message to send."
-        )
-        buf, _ = TurnMessage.unpack(m.encode())
-        buf.write_credential(client.turn_user, client.realm, client.nonce)
-        buf.write_hmac(client.key)
-        """
-
-        
-        # Attempt to get a reply at our relay address.
-        # Do it up to 3 times due to UDP being unreliable.
-        got_reply = False
-        for i in range(0, 3):
-            http_route = copy.deepcopy(r)
-            await http_route.bind()
-            rest_path = f"/hello/udp/{relay_tup[0]}/{relay_tup[1]}/{dest_p2pd.tup[0]}/63248"
-            _, resp = await http_req(http_route, dest_p2pd, rest_path)
-
-            # Attempt to read the message back.
-            out = await client.recv(SUB_ALL, 2)
-            if out == b"hello":
-                got_reply = True
-                break
-
-        # Make sure we got a valid reply.
-        self.assertTrue(got_reply)
-
-        # If refresh is done too soon it can error.
-        # await asyncio.sleep(2)
+            # Make sure we got a valid reply.
+            self.assertTrue(got_reply)
         
         # Test refresh.
         client.lifetime = 0
         await async_retry(
             lambda: client.refresh_allocation(), count=3, timeout=5
         )
         self.assertTrue(client.lifetime)
 
-        # Permission refresh.
-        await client.accept_peer(client_tup, relay_tup)
-
         # Cleanup the client.
         await client.close()
 
 if __name__ == '__main__':
     main()
```

### Comparing `p2pd-2.3.6/tests/test_win_netifaces.py` & `p2pd-2.4.0/tests/test_win_netifaces.py`

 * *Files identical despite different names*

