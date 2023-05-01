# Comparing `tmp/nonebot_plugin_xiuxian_2-2.9.1.0.tar.gz` & `tmp/nonebot_plugin_xiuxian_2-2.9.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_xiuxian_2-2.9.1.0.tar", last modified: Sat Apr 29 15:10:04 2023, max compression
+gzip compressed data, was "nonebot_plugin_xiuxian_2-2.9.2.1.tar", last modified: Mon May  1 09:00:46 2023, max compression
```

## Comparing `nonebot_plugin_xiuxian_2-2.9.1.0.tar` & `nonebot_plugin_xiuxian_2-2.9.2.1.tar`

### file list

```diff
@@ -1,76 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.332736 nonebot_plugin_xiuxian_2-2.9.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-29 15:10:04.332736 nonebot_plugin_xiuxian_2-2.9.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.320736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/download_xiuxian_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/item_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/lay_out.py
--rw-r--r--   0 runner    (1001) docker     (123)    54783 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/player_fight.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/read_buff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49555 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian2_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.320736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_back/
--rw-r--r--   0 runner    (1001) docker     (123)    72789 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_back/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21934 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_back/back_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_back/backconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.320736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_bank/
--rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_bank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_bank/bankconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.324736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_base/
--rw-r--r--   0 runner    (1001) docker     (123)    60905 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.324736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/
--rw-r--r--   0 runner    (1001) docker     (123)    35642 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/bossconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/makeboss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/old_boss_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.324736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_buff/
--rw-r--r--   0 runner    (1001) docker     (123)    45638 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_buff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_buff/two_exp_cd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.324736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/
--rw-r--r--   0 runner    (1001) docker     (123)    18822 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_uitls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.324736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/
--rw-r--r--   0 runner    (1001) docker     (123)    19054 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/impart_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/impart_pk_uitls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/xu_world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.328736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/draw_user_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/send_image_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.328736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/
--rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/mix_elixir_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/mixelixirutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_opertion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.328736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/
--rw-r--r--   0 runner    (1001) docker     (123)    20739 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/jsondata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/old_rift_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/riftconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/riftmake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.328736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_sect/
--rw-r--r--   0 runner    (1001) docker     (123)    98636 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_sect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_sect/sectconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.328736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/
--rw-r--r--   0 runner    (1001) docker     (123)    24909 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/reward_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/work_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/workmake.py
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xn_xiuxian_impart.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xn_xiuxian_impart_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.320736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-29 15:10:04.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-29 15:10:04.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:10:04.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-29 15:10:04.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-29 15:10:04.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:10:04.332736 nonebot_plugin_xiuxian_2-2.9.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.309723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.313723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/download_xiuxian_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/item_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/lay_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54783 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/player_fight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/read_buff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49555 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian2_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.313723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/
+-rw-r--r--   0 runner    (1001) docker     (123)    72789 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21934 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/back_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/backconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.317723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/xiuxian_back/
+-rw-r--r--   0 runner    (1001) docker     (123)    72776 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/xiuxian_back/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21934 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/xiuxian_back/back_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.317723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/bankconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.317723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_base/
+-rw-r--r--   0 runner    (1001) docker     (123)    60905 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.317723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/
+-rw-r--r--   0 runner    (1001) docker     (123)    35642 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/bossconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/makeboss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/old_boss_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.317723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/
+-rw-r--r--   0 runner    (1001) docker     (123)    45638 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/two_exp_cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/
+-rw-r--r--   0 runner    (1001) docker     (123)    18822 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_uitls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/
+-rw-r--r--   0 runner    (1001) docker     (123)    19054 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/impart_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/impart_pk_uitls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/xu_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/draw_user_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/send_image_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/
+-rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/mix_elixir_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/mixelixirutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_opertion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/
+-rw-r--r--   0 runner    (1001) docker     (123)    20739 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/jsondata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/old_rift_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/riftconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/riftmake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/
+-rw-r--r--   0 runner    (1001) docker     (123)    98636 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/sectconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/
+-rw-r--r--   0 runner    (1001) docker     (123)    24909 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/reward_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/work_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/workmake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xn_xiuxian_impart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xn_xiuxian_impart_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 09:00:46.309723 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-01 09:00:46.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-01 09:00:46.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 09:00:46.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-01 09:00:46.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-01 09:00:46.000000 nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 09:00:46.321723 nonebot_plugin_xiuxian_2-2.9.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-01 09:00:31.000000 nonebot_plugin_xiuxian_2-2.9.2.1/setup.py
```

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/PKG-INFO` & `nonebot_plugin_xiuxian_2-2.9.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_xiuxian_2
-Version: 2.9.1.0
+Version: 2.9.2.1
 Summary: 修仙插件
 Home-page: https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 Author: QingmuCat
 Author-email: 1242550160@qq.com
 Keywords: pip,nonebot2,文游,修仙
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_xiuxian_2 Version: 2.9.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_xiuxian_2 Version: 2.9.2.1 Summary:
 ä¿®ä»æä»¶ Home-page: https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 Author: QingmuCat Author-email: 1242550160@qq.com Keywords:
 pip,nonebot2,ææ¸¸,ä¿®ä» Platform: any Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified) Description-
 Content-Type: text/markdown
                              [NoneBotPluginLogo]
```

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/README.md` & `nonebot_plugin_xiuxian_2-2.9.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 #!usr/bin/env python3
 # -*- coding: utf-8 -*-
-import nonebot
-from nonebot import require, get_driver
-from nonebot.log import logger
+from .download_xiuxian_data import download_xiuxian_data
 from nonebot.plugin import PluginMetadata
+from nonebot.log import logger
 from nonebot.message import event_preprocessor, IgnoredException
-from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent
-
+from nonebot.adapters.onebot.v11 import (
+    Bot,
+    GroupMessageEvent
+)
+from nonebot import get_driver
+from .xiuxian_config import XiuConfig
 from pathlib import Path
 from pkgutil import iter_modules
-
-from .download_xiuxian_data import download_xiuxian_data
-from .xiuxian_config import XiuConfig
+from nonebot.log import logger
+from nonebot import require, load_all_plugins, get_plugin_by_module_name
 from .config import config as _config
 
 
 DRIVER = get_driver()
 
 try:
     NICKNAME: str = list(DRIVER.config.nickname)[0]
 except Exception as e:
     logger.info(f"缺少超级用户配置文件，{e}!")
-    NICKNAME = "bot"
+    NICKNAME = 'bot'
 
 try:
     download_xiuxian_data()
 except Exception as e:
     logger.info(f"下载配置文件失败，修仙插件无法加载，{e}!")
     raise ImportError
 
@@ -33,23 +35,43 @@
 shield_group = XiuConfig().shield_group
 
 try:
     put_bot_ = put_bot[0]
 except:
     logger.info(f"修仙插件没有配置put_bot,如果有多个qq和nb链接,请务必配置put_bot,具体介绍参考【风控帮助】！")
 
-require("nonebot_plugin_apscheduler")
+require('nonebot_plugin_apscheduler')
 
-nonebot.load_plugins(str(Path(__file__).parent.resolve()))
+if get_plugin_by_module_name("xiuxian"):
+    logger.info("推荐直接加载 xiuxian 仓库文件夹")
+    load_all_plugins(
+        [
+            f"xiuxian.{module.name}"
+            for module in iter_modules([str(Path(__file__).parent)])
+            if module.ispkg
+            and (
+                (name := module.name[11:]) == "meta"
+                or name not in _config.disabled_plugins
+            )
+            # module.name[:11] == xiuxian_
+        ],
+        [],
+    )
 
 __plugin_meta__ = PluginMetadata(
-    name="修仙模拟器",
-    description="修仙游戏",
-    usage=("必死之境机逢仙缘，修仙之路波澜壮阔！\n" " 输入 < /修仙帮助 > 获取仙界信息"),
-    extra={"show": True, "priority": 15},
+    name='修仙模拟器',
+    description='',
+    usage=(
+        "必死之境机逢仙缘，修仙之路波澜壮阔！\n"
+        " 输入 < 修仙帮助 > 获取仙界信息"
+    ),
+    extra={
+        "show": True,
+        "priority": 15
+    }
 )
 
 
 @event_preprocessor
 async def do_something(bot: Bot, event: GroupMessageEvent):
     global put_bot
     if not put_bot:
@@ -58,7 +80,9 @@
         if str(bot.self_id) in put_bot:
             if str(event.group_id) in shield_group:
                 raise IgnoredException("为屏蔽群消息,已忽略")
             else:
                 pass
         else:
             raise IgnoredException("非主bot信息,已忽略")
+
+
```

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/data_source.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/download_xiuxian_data.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/download_xiuxian_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/item_json.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/item_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/lay_out.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/lay_out.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/player_fight.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/player_fight.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/read_buff.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/read_buff.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/utils.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian2_handle.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian2_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_back/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_back/back_util.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/back_util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_back/backconfig.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/backconfig.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_bank/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_bank/bankconfig.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/bankconfig.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_base/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_base/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/bossconfig.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/bossconfig.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/makeboss.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/makeboss.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/old_boss_info.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/old_boss_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_buff/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_buff/two_exp_cd.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/two_exp_cd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_config.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_all.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_all.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_data.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_uitls.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_uitls.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/impart_pk.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/impart_pk.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/impart_pk_uitls.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/impart_pk_uitls.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/xu_world.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/xu_world.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/download.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/draw_user_info.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/draw_user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/send_image_tool.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/mixelixirutil.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/mixelixirutil.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_opertion.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_opertion.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/jsondata.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/jsondata.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/old_rift_info.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/old_rift_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/riftconfig.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/riftconfig.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/riftmake.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/riftmake.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_sect/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_sect/sectconfig.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/sectconfig.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/reward_data_source.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/reward_data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/work_handle.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/work_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/workmake.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/workmake.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xn_xiuxian_impart.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xn_xiuxian_impart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xn_xiuxian_impart_config.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2/xiuxian/xn_xiuxian_impart_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/PKG-INFO` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-xiuxian-2
-Version: 2.9.1.0
+Version: 2.9.2.1
 Summary: 修仙插件
 Home-page: https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 Author: QingmuCat
 Author-email: 1242550160@qq.com
 Keywords: pip,nonebot2,文游,修仙
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-xiuxian-2 Version: 2.9.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-xiuxian-2 Version: 2.9.2.1 Summary:
 ä¿®ä»æä»¶ Home-page: https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 Author: QingmuCat Author-email: 1242550160@qq.com Keywords:
 pip,nonebot2,ææ¸¸,ä¿®ä» Platform: any Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified) Description-
 Content-Type: text/markdown
                              [NoneBotPluginLogo]
```

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/SOURCES.txt` & `nonebot_plugin_xiuxian_2-2.9.2.1/nonebot_plugin_xiuxian_2.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 README.md
 setup.py
 nonebot_plugin_xiuxian_2/__init__.py
-nonebot_plugin_xiuxian_2/config.py
-nonebot_plugin_xiuxian_2/data_source.py
-nonebot_plugin_xiuxian_2/download_xiuxian_data.py
-nonebot_plugin_xiuxian_2/item_json.py
-nonebot_plugin_xiuxian_2/lay_out.py
-nonebot_plugin_xiuxian_2/player_fight.py
-nonebot_plugin_xiuxian_2/read_buff.py
-nonebot_plugin_xiuxian_2/utils.py
-nonebot_plugin_xiuxian_2/xiuxian2_handle.py
-nonebot_plugin_xiuxian_2/xiuxian_config.py
-nonebot_plugin_xiuxian_2/xiuxian_opertion.py
-nonebot_plugin_xiuxian_2/xn_xiuxian_impart.py
-nonebot_plugin_xiuxian_2/xn_xiuxian_impart_config.py
 nonebot_plugin_xiuxian_2.egg-info/PKG-INFO
 nonebot_plugin_xiuxian_2.egg-info/SOURCES.txt
 nonebot_plugin_xiuxian_2.egg-info/dependency_links.txt
 nonebot_plugin_xiuxian_2.egg-info/requires.txt
 nonebot_plugin_xiuxian_2.egg-info/top_level.txt
-nonebot_plugin_xiuxian_2/xiuxian_back/__init__.py
-nonebot_plugin_xiuxian_2/xiuxian_back/back_util.py
-nonebot_plugin_xiuxian_2/xiuxian_back/backconfig.py
-nonebot_plugin_xiuxian_2/xiuxian_bank/__init__.py
-nonebot_plugin_xiuxian_2/xiuxian_bank/bankconfig.py
-nonebot_plugin_xiuxian_2/xiuxian_base/__init__.py
-nonebot_plugin_xiuxian_2/xiuxian_boss/__init__.py
-nonebot_plugin_xiuxian_2/xiuxian_boss/bossconfig.py
-nonebot_plugin_xiuxian_2/xiuxian_boss/makeboss.py
-nonebot_plugin_xiuxian_2/xiuxian_boss/old_boss_info.py
-nonebot_plugin_xiuxian_2/xiuxian_buff/__init__.py
-nonebot_plugin_xiuxian_2/xiuxian_buff/two_exp_cd.py
-nonebot_plugin_xiuxian_2/xiuxian_impart/__init__.py
-nonebot_plugin_xiuxian_2/xiuxian_impart/impart_all.py
-nonebot_plugin_xiuxian_2/xiuxian_impart/impart_data.py
-nonebot_plugin_xiuxian_2/xiuxian_impart/impart_uitls.py
-nonebot_plugin_xiuxian_2/xiuxian_impart_pk/__init__.py
-nonebot_plugin_xiuxian_2/xiuxian_impart_pk/impart_pk.py
-nonebot_plugin_xiuxian_2/xiuxian_impart_pk/impart_pk_uitls.py
-nonebot_plugin_xiuxian_2/xiuxian_impart_pk/xu_world.py
-nonebot_plugin_xiuxian_2/xiuxian_info/__init__.py
-nonebot_plugin_xiuxian_2/xiuxian_info/download.py
-nonebot_plugin_xiuxian_2/xiuxian_info/draw_user_info.py
-nonebot_plugin_xiuxian_2/xiuxian_info/send_image_tool.py
-nonebot_plugin_xiuxian_2/xiuxian_mixelixir/__init__.py
-nonebot_plugin_xiuxian_2/xiuxian_mixelixir/mix_elixir_config.py
-nonebot_plugin_xiuxian_2/xiuxian_mixelixir/mixelixirutil.py
-nonebot_plugin_xiuxian_2/xiuxian_rift/__init__.py
-nonebot_plugin_xiuxian_2/xiuxian_rift/jsondata.py
-nonebot_plugin_xiuxian_2/xiuxian_rift/old_rift_info.py
-nonebot_plugin_xiuxian_2/xiuxian_rift/riftconfig.py
-nonebot_plugin_xiuxian_2/xiuxian_rift/riftmake.py
-nonebot_plugin_xiuxian_2/xiuxian_sect/__init__.py
-nonebot_plugin_xiuxian_2/xiuxian_sect/sectconfig.py
-nonebot_plugin_xiuxian_2/xiuxian_work/__init__.py
-nonebot_plugin_xiuxian_2/xiuxian_work/reward_data_source.py
-nonebot_plugin_xiuxian_2/xiuxian_work/work_handle.py
-nonebot_plugin_xiuxian_2/xiuxian_work/workmake.py
+nonebot_plugin_xiuxian_2/xiuxian/__init__.py
+nonebot_plugin_xiuxian_2/xiuxian/config.py
+nonebot_plugin_xiuxian_2/xiuxian/data_source.py
+nonebot_plugin_xiuxian_2/xiuxian/download_xiuxian_data.py
+nonebot_plugin_xiuxian_2/xiuxian/item_json.py
+nonebot_plugin_xiuxian_2/xiuxian/lay_out.py
+nonebot_plugin_xiuxian_2/xiuxian/player_fight.py
+nonebot_plugin_xiuxian_2/xiuxian/read_buff.py
+nonebot_plugin_xiuxian_2/xiuxian/utils.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian2_handle.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_config.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_opertion.py
+nonebot_plugin_xiuxian_2/xiuxian/xn_xiuxian_impart.py
+nonebot_plugin_xiuxian_2/xiuxian/xn_xiuxian_impart_config.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/__init__.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/back_util.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/backconfig.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/xiuxian_back/__init__.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_back/xiuxian_back/back_util.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/__init__.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_bank/bankconfig.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_base/__init__.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/__init__.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/bossconfig.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/makeboss.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_boss/old_boss_info.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/__init__.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_buff/two_exp_cd.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/__init__.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_all.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_data.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart/impart_uitls.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/__init__.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/impart_pk.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/impart_pk_uitls.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_impart_pk/xu_world.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/__init__.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/download.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/draw_user_info.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_info/send_image_tool.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/__init__.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/mix_elixir_config.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_mixelixir/mixelixirutil.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/__init__.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/jsondata.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/old_rift_info.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/riftconfig.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_rift/riftmake.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/__init__.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_sect/sectconfig.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/__init__.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/reward_data_source.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/work_handle.py
+nonebot_plugin_xiuxian_2/xiuxian/xiuxian_work/workmake.py
```

### Comparing `nonebot_plugin_xiuxian_2-2.9.1.0/setup.py` & `nonebot_plugin_xiuxian_2-2.9.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
-
 import setuptools
 
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as f:
     long_description = f.read()
     setuptools.setup(
     name='nonebot_plugin_xiuxian_2',
-    version='2.9.1.0',
+    version='2.9.2.1',
     author='QingmuCat',
     author_email='1242550160@qq.com',
     keywords=["pip", "nonebot2", "文游", "修仙"],
     url='https://github.com/QingMuCat/nonebot_plugin_xiuxian_2',
     description='''修仙插件''',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

