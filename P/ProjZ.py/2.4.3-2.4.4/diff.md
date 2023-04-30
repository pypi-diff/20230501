# Comparing `tmp/ProjZ.py-2.4.3.tar.gz` & `tmp/ProjZ.py-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjZ.py-2.4.3.tar", last modified: Sat Apr 29 22:44:41 2023, max compression
+gzip compressed data, was "ProjZ.py-2.4.4.tar", last modified: Sun Apr 30 22:26:00 2023, max compression
```

## Comparing `ProjZ.py-2.4.3.tar` & `ProjZ.py-2.4.4.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:41.002530 ProjZ.py-2.4.3/
--rw-rw-rw-   0        0        0     4049 2023-04-29 22:44:41.002530 ProjZ.py-2.4.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.211450 ProjZ.py-2.4.3/ProjZ.py.egg-info/
--rw-rw-rw-   0        0        0     4049 2023-04-29 22:44:40.000000 ProjZ.py-2.4.3/ProjZ.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2325 2023-04-29 22:44:40.000000 ProjZ.py-2.4.3/ProjZ.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 22:44:40.000000 ProjZ.py-2.4.3/ProjZ.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-29 22:44:40.000000 ProjZ.py-2.4.3/ProjZ.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-29 22:44:40.000000 ProjZ.py-2.4.3/ProjZ.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3640 2023-04-29 17:20:16.000000 ProjZ.py-2.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.239629 ProjZ.py-2.4.3/projz/
--rw-rw-rw-   0        0        0      112 2023-04-29 17:24:41.000000 ProjZ.py-2.4.3/projz/__init__.py
--rw-rw-rw-   0        0        0     7167 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.251616 ProjZ.py-2.4.3/projz/api/
--rw-rw-rw-   0        0        0      120 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.274564 ProjZ.py-2.4.3/projz/api/control/
--rw-rw-rw-   0        0        0       22 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/api/control/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/api/control/rpc.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.306444 ProjZ.py-2.4.3/projz/api/headers/
--rw-rw-rw-   0        0        0      101 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/api/headers/__init__.py
--rw-rw-rw-   0        0        0      969 2023-04-29 12:23:08.000000 ProjZ.py-2.4.3/projz/api/headers/abc_headers_provider.py
--rw-rw-rw-   0        0        0     2334 2023-04-29 15:38:12.000000 ProjZ.py-2.4.3/projz/api/headers/headers_provider.py
--rw-rw-rw-   0        0        0     4789 2023-04-29 20:52:00.000000 ProjZ.py-2.4.3/projz/api/request_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.318419 ProjZ.py-2.4.3/projz/api/secret/
--rw-rw-rw-   0        0        0      661 2023-04-29 17:19:39.000000 ProjZ.py-2.4.3/projz/api/secret/__init__.py
--rw-rw-rw-   0        0        0    11964 2023-04-29 15:20:01.000000 ProjZ.py-2.4.3/projz/api/secret/data.txt
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.339165 ProjZ.py-2.4.3/projz/api/util/
--rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/api/util/__init__.py
--rw-rw-rw-   0        0        0      289 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/api/util/copy_to_buffer_writer.py
--rw-rw-rw-   0        0        0    58016 2023-04-29 22:00:27.000000 ProjZ.py-2.4.3/projz/client.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.510447 ProjZ.py-2.4.3/projz/enum/
--rw-rw-rw-   0        0        0      641 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/__init__.py
--rw-rw-rw-   0        0        0      179 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/auth_purpose.py
--rw-rw-rw-   0        0        0       87 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/auth_type.py
--rw-rw-rw-   0        0        0      165 2023-04-29 20:27:50.000000 ProjZ.py-2.4.3/projz/enum/chat_message_type.py
--rw-rw-rw-   0        0        0      181 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/chat_query_type.py
--rw-rw-rw-   0        0        0      109 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/chat_thread_type.py
--rw-rw-rw-   0        0        0      158 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/circle_filter_type.py
--rw-rw-rw-   0        0        0      112 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/circle_members_query_type.py
--rw-rw-rw-   0        0        0       82 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/comment_type.py
--rw-rw-rw-   0        0        0      221 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/content_region.py
--rw-rw-rw-   0        0        0      108 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/currency_type.py
--rw-rw-rw-   0        0        0       95 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/gender.py
--rw-rw-rw-   0        0        0      149 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/object_type.py
--rw-rw-rw-   0        0        0       85 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/party_query_type.py
--rw-rw-rw-   0        0        0      210 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/upload_target.py
--rw-rw-rw-   0        0        0      212 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/user_task_type.py
--rw-rw-rw-   0        0        0       98 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/enum/ws_event_type.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.539845 ProjZ.py-2.4.3/projz/error/
--rw-rw-rw-   0        0        0       24 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/error/__init__.py
--rw-rw-rw-   0        0        0     1620 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/error/classes.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.817526 ProjZ.py-2.4.3/projz/model/
--rw-rw-rw-   0        0        0     1140 2023-04-29 21:59:15.000000 ProjZ.py-2.4.3/projz/model/__init__.py
--rw-rw-rw-   0        0        0      967 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/account.py
--rw-rw-rw-   0        0        0      577 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/blocked_item_wrapper.py
--rw-rw-rw-   0        0        0     1388 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/blog.py
--rw-rw-rw-   0        0        0     1796 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/category.py
--rw-rw-rw-   0        0        0     2260 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/chat.py
--rw-rw-rw-   0        0        0      952 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/chat_message.py
--rw-rw-rw-   0        0        0     2093 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/circle.py
--rw-rw-rw-   0        0        0      768 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/comment.py
--rw-rw-rw-   0        0        0      584 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/currency.py
--rw-rw-rw-   0        0        0      663 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/default_background_media.py
--rw-rw-rw-   0        0        0      433 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/dice.py
--rw-rw-rw-   0        0        0     1194 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/gift_box.py
--rw-rw-rw-   0        0        0      415 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/link_info.py
--rw-rw-rw-   0        0        0      602 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/media.py
--rw-rw-rw-   0        0        0      540 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/member_title.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.864850 ProjZ.py-2.4.3/projz/model/parse/
--rw-rw-rw-   0        0        0       27 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/parse/__init__.py
--rw-rw-rw-   0        0        0     1033 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/parse/parseutils.py
--rw-rw-rw-   0        0        0      409 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/party.py
--rw-rw-rw-   0        0        0      840 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/poll.py
--rw-rw-rw-   0        0        0     1004 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/qi_vote_full_info.py
--rw-rw-rw-   0        0        0      594 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/qi_vote_info.py
--rw-rw-rw-   0        0        0      561 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/reaction.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.904379 ProjZ.py-2.4.3/projz/model/response/
--rw-rw-rw-   0        0        0      198 2023-04-29 21:59:15.000000 ProjZ.py-2.4.3/projz/model/response/__init__.py
--rw-rw-rw-   0        0        0      447 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/response/auth_result.py
--rw-rw-rw-   0        0        0      363 2023-04-29 21:58:26.000000 ProjZ.py-2.4.3/projz/model/response/block_users_info.py
--rw-rw-rw-   0        0        0      513 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/response/member_titles_info.py
--rw-rw-rw-   0        0        0      738 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/response/multi_invitation_code_info.py
--rw-rw-rw-   0        0        0     2872 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/rich_format.py
--rw-rw-rw-   0        0        0      280 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/sticker.py
--rw-rw-rw-   0        0        0     1134 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/transfer_order.py
--rw-rw-rw-   0        0        0     3484 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/user.py
--rw-rw-rw-   0        0        0      632 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/user_task.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.951558 ProjZ.py-2.4.3/projz/model/util/
--rw-rw-rw-   0        0        0      156 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/util/__init__.py
--rw-rw-rw-   0        0        0      339 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/util/paginated_list.py
--rw-rw-rw-   0        0        0     4388 2023-04-29 17:46:35.000000 ProjZ.py-2.4.3/projz/model/util/rich_format_builder.py
--rw-rw-rw-   0        0        0     4790 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/util/rich_format_text_builder.py
--rw-rw-rw-   0        0        0     1685 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/model/wallet.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.973505 ProjZ.py-2.4.3/projz/util/
--rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/util/__init__.py
--rw-rw-rw-   0        0        0     1492 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/util/subscription_handler.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:44:40.997555 ProjZ.py-2.4.3/projz/websocket/
--rw-rw-rw-   0        0        0       51 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/websocket/__init__.py
--rw-rw-rw-   0        0        0     3753 2023-04-29 10:11:44.000000 ProjZ.py-2.4.3/projz/websocket/websocket_listener.py
--rw-rw-rw-   0        0        0       42 2023-04-29 22:44:41.005523 ProjZ.py-2.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1929 2023-04-29 22:44:20.000000 ProjZ.py-2.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.690834 ProjZ.py-2.4.4/
+-rw-rw-rw-   0        0        0     4076 2023-04-30 22:26:00.690834 ProjZ.py-2.4.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.061927 ProjZ.py-2.4.4/ProjZ.py.egg-info/
+-rw-rw-rw-   0        0        0     4076 2023-04-30 22:25:59.000000 ProjZ.py-2.4.4/ProjZ.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2325 2023-04-30 22:25:59.000000 ProjZ.py-2.4.4/ProjZ.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 22:25:59.000000 ProjZ.py-2.4.4/ProjZ.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-04-30 22:25:59.000000 ProjZ.py-2.4.4/ProjZ.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-30 22:25:59.000000 ProjZ.py-2.4.4/ProjZ.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3640 2023-04-29 17:20:16.000000 ProjZ.py-2.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.110101 ProjZ.py-2.4.4/projz/
+-rw-rw-rw-   0        0        0      112 2023-04-30 20:29:06.000000 ProjZ.py-2.4.4/projz/__init__.py
+-rw-rw-rw-   0        0        0     7271 2023-04-30 10:53:19.000000 ProjZ.py-2.4.4/projz/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.120485 ProjZ.py-2.4.4/projz/api/
+-rw-rw-rw-   0        0        0      120 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.136525 ProjZ.py-2.4.4/projz/api/control/
+-rw-rw-rw-   0        0        0       22 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/api/control/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/api/control/rpc.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.154662 ProjZ.py-2.4.4/projz/api/headers/
+-rw-rw-rw-   0        0        0      101 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/api/headers/__init__.py
+-rw-rw-rw-   0        0        0      969 2023-04-29 12:23:08.000000 ProjZ.py-2.4.4/projz/api/headers/abc_headers_provider.py
+-rw-rw-rw-   0        0        0     2334 2023-04-29 15:38:12.000000 ProjZ.py-2.4.4/projz/api/headers/headers_provider.py
+-rw-rw-rw-   0        0        0     4789 2023-04-30 22:24:02.000000 ProjZ.py-2.4.4/projz/api/request_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.160173 ProjZ.py-2.4.4/projz/api/secret/
+-rw-rw-rw-   0        0        0      661 2023-04-30 20:41:57.000000 ProjZ.py-2.4.4/projz/api/secret/__init__.py
+-rw-rw-rw-   0        0        0    11964 2023-04-29 15:20:01.000000 ProjZ.py-2.4.4/projz/api/secret/data.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.168846 ProjZ.py-2.4.4/projz/api/util/
+-rw-rw-rw-   0        0        0       55 2023-04-30 20:41:25.000000 ProjZ.py-2.4.4/projz/api/util/__init__.py
+-rw-rw-rw-   0        0        0      289 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/api/util/copy_to_buffer_writer.py
+-rw-rw-rw-   0        0        0    58016 2023-04-29 22:00:27.000000 ProjZ.py-2.4.4/projz/client.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.279593 ProjZ.py-2.4.4/projz/enum/
+-rw-rw-rw-   0        0        0      641 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/__init__.py
+-rw-rw-rw-   0        0        0      179 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/auth_purpose.py
+-rw-rw-rw-   0        0        0       87 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/auth_type.py
+-rw-rw-rw-   0        0        0      165 2023-04-29 20:27:50.000000 ProjZ.py-2.4.4/projz/enum/chat_message_type.py
+-rw-rw-rw-   0        0        0      181 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/chat_query_type.py
+-rw-rw-rw-   0        0        0      109 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/chat_thread_type.py
+-rw-rw-rw-   0        0        0      158 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/circle_filter_type.py
+-rw-rw-rw-   0        0        0      112 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/circle_members_query_type.py
+-rw-rw-rw-   0        0        0       82 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/comment_type.py
+-rw-rw-rw-   0        0        0      221 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/content_region.py
+-rw-rw-rw-   0        0        0      108 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/currency_type.py
+-rw-rw-rw-   0        0        0       95 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/gender.py
+-rw-rw-rw-   0        0        0      149 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/object_type.py
+-rw-rw-rw-   0        0        0       85 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/party_query_type.py
+-rw-rw-rw-   0        0        0      210 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/upload_target.py
+-rw-rw-rw-   0        0        0      212 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/user_task_type.py
+-rw-rw-rw-   0        0        0       98 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/enum/ws_event_type.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.290914 ProjZ.py-2.4.4/projz/error/
+-rw-rw-rw-   0        0        0       24 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/error/__init__.py
+-rw-rw-rw-   0        0        0     1620 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/error/classes.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.501891 ProjZ.py-2.4.4/projz/model/
+-rw-rw-rw-   0        0        0     1140 2023-04-29 21:59:15.000000 ProjZ.py-2.4.4/projz/model/__init__.py
+-rw-rw-rw-   0        0        0      967 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/account.py
+-rw-rw-rw-   0        0        0      577 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/blocked_item_wrapper.py
+-rw-rw-rw-   0        0        0     1388 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/blog.py
+-rw-rw-rw-   0        0        0     1796 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/category.py
+-rw-rw-rw-   0        0        0     2260 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/chat.py
+-rw-rw-rw-   0        0        0      952 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/chat_message.py
+-rw-rw-rw-   0        0        0     2093 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/circle.py
+-rw-rw-rw-   0        0        0      768 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/comment.py
+-rw-rw-rw-   0        0        0      584 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/currency.py
+-rw-rw-rw-   0        0        0      663 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/default_background_media.py
+-rw-rw-rw-   0        0        0      433 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/dice.py
+-rw-rw-rw-   0        0        0     1194 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/gift_box.py
+-rw-rw-rw-   0        0        0      415 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/link_info.py
+-rw-rw-rw-   0        0        0      602 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/media.py
+-rw-rw-rw-   0        0        0      540 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/member_title.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.593876 ProjZ.py-2.4.4/projz/model/parse/
+-rw-rw-rw-   0        0        0       27 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/parse/__init__.py
+-rw-rw-rw-   0        0        0     1033 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/parse/parseutils.py
+-rw-rw-rw-   0        0        0      409 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/party.py
+-rw-rw-rw-   0        0        0      840 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/poll.py
+-rw-rw-rw-   0        0        0     1004 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/qi_vote_full_info.py
+-rw-rw-rw-   0        0        0      594 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/qi_vote_info.py
+-rw-rw-rw-   0        0        0      561 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/reaction.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.636795 ProjZ.py-2.4.4/projz/model/response/
+-rw-rw-rw-   0        0        0      198 2023-04-29 21:59:15.000000 ProjZ.py-2.4.4/projz/model/response/__init__.py
+-rw-rw-rw-   0        0        0      447 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/response/auth_result.py
+-rw-rw-rw-   0        0        0      363 2023-04-29 21:58:26.000000 ProjZ.py-2.4.4/projz/model/response/block_users_info.py
+-rw-rw-rw-   0        0        0      513 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/response/member_titles_info.py
+-rw-rw-rw-   0        0        0      738 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/response/multi_invitation_code_info.py
+-rw-rw-rw-   0        0        0     2872 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/rich_format.py
+-rw-rw-rw-   0        0        0      280 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/sticker.py
+-rw-rw-rw-   0        0        0     1134 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/transfer_order.py
+-rw-rw-rw-   0        0        0     3484 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/user.py
+-rw-rw-rw-   0        0        0      632 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/user_task.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.666953 ProjZ.py-2.4.4/projz/model/util/
+-rw-rw-rw-   0        0        0      156 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/util/__init__.py
+-rw-rw-rw-   0        0        0      339 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/util/paginated_list.py
+-rw-rw-rw-   0        0        0     4388 2023-04-29 17:46:35.000000 ProjZ.py-2.4.4/projz/model/util/rich_format_builder.py
+-rw-rw-rw-   0        0        0     4790 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/util/rich_format_text_builder.py
+-rw-rw-rw-   0        0        0     1685 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/model/wallet.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.677834 ProjZ.py-2.4.4/projz/util/
+-rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/util/__init__.py
+-rw-rw-rw-   0        0        0     1492 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/util/subscription_handler.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:26:00.687782 ProjZ.py-2.4.4/projz/websocket/
+-rw-rw-rw-   0        0        0       51 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/websocket/__init__.py
+-rw-rw-rw-   0        0        0     3753 2023-04-29 10:11:44.000000 ProjZ.py-2.4.4/projz/websocket/websocket_listener.py
+-rw-rw-rw-   0        0        0       42 2023-04-30 22:26:00.695823 ProjZ.py-2.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1980 2023-04-30 20:29:06.000000 ProjZ.py-2.4.4/setup.py
```

### Comparing `ProjZ.py-2.4.3/PKG-INFO` & `ProjZ.py-2.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ProjZ.py
-Version: 2.4.3
+Version: 2.4.4
 Summary: An asynchronous library for creating scripts and chatbots in Project Z.
-Home-page: UNKNOWN
+Home-page: https://github.com/D4rkwat3r/ProjZ
 Author: D4rkwat3r
 Author-email: ktoya170214@gmail.com
 License: UNKNOWN
 Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-bot,projz-bots,projz-api
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ProjZ.py-2.4.3/ProjZ.py.egg-info/PKG-INFO` & `ProjZ.py-2.4.4/ProjZ.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ProjZ.py
-Version: 2.4.3
+Version: 2.4.4
 Summary: An asynchronous library for creating scripts and chatbots in Project Z.
-Home-page: UNKNOWN
+Home-page: https://github.com/D4rkwat3r/ProjZ
 Author: D4rkwat3r
 Author-email: ktoya170214@gmail.com
 License: UNKNOWN
 Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-bot,projz-bots,projz-api
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ProjZ.py-2.4.3/ProjZ.py.egg-info/SOURCES.txt` & `ProjZ.py-2.4.4/ProjZ.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/README.md` & `ProjZ.py-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/__main__.py` & `ProjZ.py-2.4.4/projz/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from argparse import ArgumentParser
 from asyncio import get_event_loop
 from asyncio import create_task
 from asyncio import gather
 from inspect import iscoroutinefunction
+from inspect import signature
 from sys import exit as sys_exit
 from . import *
 
 parser = ArgumentParser(description="ProjZ.py library command line interface")
 parser.add_argument("action", type=str, help="The action to be performed. "
                                              "You can view the list of possible actions by "
                                              "setting the value \"list-actions\"")
@@ -30,21 +31,26 @@
                 else func(*args, **kwargs)
         except Exception as e:
             print(f"Error: {e}")
 
     return wrapper
 
 
-def authenticated(func):
+def authenticated(func: Callable):
     def wrapper(*args, **kwargs):
         if cli_args.login is None or cli_args.password is None or cli_args.auth_type is None:
             print("Specify login, password and auth type.")
             return
-        return get_event_loop().run_until_complete(func(*args, **kwargs)) if iscoroutinefunction(func) \
+        loop = get_event_loop()
+        auth_result = loop.run_until_complete(login())
+        if len(signature(func).parameters) > 0:
+            args = (auth_result,) + args
+        return loop.run_until_complete(func(*args, **kwargs)) if iscoroutinefunction(func) \
             else func(*args, **kwargs)
+
     return wrapper
 
 
 async def login() -> AuthResult:
     return await (
         client.login_email if cli_args.auth_type == "email"
         else client.login_phone_number
@@ -62,16 +68,15 @@
 def action_list_actions():
     for i, key in enumerate(action_mapping, start=1):
         print(f"{i}. {key} - {action_mapping[key][1]}")
 
 
 @print_error
 @authenticated
-async def action_login():
-    auth = await login()
+async def action_login(auth: AuthResult):
     print(f"[+] Session ID: {auth.sid}")
     print(f"[+] Refresh token (secret): {auth.secret}")
     print("[+] Account:")
     print(f"    -- Email: {auth.account.email or '-'}")
     print(f"    -- Phone number: {auth.account.phone_number or '-'}")
     print(f"    -- Registration time: {auth.account.created_time or '-'}")
     print(f"    -- Registered IPv4: {auth.account.registered_ipv4 or '-'}")
@@ -93,15 +98,14 @@
 
 @print_error
 @authenticated
 async def action_link_info():
     if cli_args.info is None:
         print("Specify --info.")
         return
-    await login()
     info = await client.get_link_info(cli_args.info)
     print(f"[+] Path: {info.path or '-'}")
     print(f"[+] Object ID: {info.object_id or '-'}")
     print(f"[+] Object type: {info.object_type or '-'}")
     print(f"[+] Share link: {info.share_link or '-'}")
     print(f"[+] Parent type: {info.parent_type or '-'}")
 
@@ -111,52 +115,47 @@
 async def action_send_message():
     if cli_args.thread is None or cli_args.message is None or cli_args.repeat is None:
         print("Specify --thread, --message and --repeat.")
         return
     if cli_args.repeat == 0:
         print("Illegal argument (repeat=0).")
         return
-    await login()
 
     chat_id = (await client.get_link_info(cli_args.thread)).object_id
     results = await gather(*[create_task(safe_send_chat_message(chat_id)) for _ in range(cli_args.repeat)])
     sent = list(filter(lambda x: x, results))
 
     print(f"[{'+' if any(results) else '-'}] Sent: {len(sent)}/{len(results)}")
 
 
 @print_error
 @authenticated
 async def action_join_circle():
     if cli_args.circle is None:
         print("Specify --circle.")
         return
-    await login()
 
     await client.join_circle(cli_args.circle)
     print(f"[+] Joined successfully.")
 
 
 @print_error
 @authenticated
 async def action_leave_circle():
     if cli_args.circle is None:
         print("Specify --circle.")
         return
-    await login()
 
     await client.leave_circle(cli_args.circle)
     print(f"[+] Left successfully.")
 
 
 @print_error
 @authenticated
 async def action_listen():
-    await login()
-
     client.register_chat_message_handler(
         lambda x: print(f"{x.author.nickname}: {x.content}"),
         lambda x: x.content is not None and x.author is not None
     )
     print(f"[+] Waiting for the messages...")
 
 action_mapping = {
```

### Comparing `ProjZ.py-2.4.3/projz/api/control/rpc.py` & `ProjZ.py-2.4.4/projz/api/control/rpc.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/api/headers/abc_headers_provider.py` & `ProjZ.py-2.4.4/projz/api/headers/abc_headers_provider.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/api/headers/headers_provider.py` & `ProjZ.py-2.4.4/projz/api/headers/headers_provider.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/api/request_manager.py` & `ProjZ.py-2.4.4/projz/api/request_manager.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/api/secret/__init__.py` & `ProjZ.py-2.4.4/projz/api/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/api/secret/data.txt` & `ProjZ.py-2.4.4/projz/api/secret/data.txt`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/client.py` & `ProjZ.py-2.4.4/projz/client.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/enum/__init__.py` & `ProjZ.py-2.4.4/projz/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/error/classes.py` & `ProjZ.py-2.4.4/projz/error/classes.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/__init__.py` & `ProjZ.py-2.4.4/projz/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/account.py` & `ProjZ.py-2.4.4/projz/model/account.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/blocked_item_wrapper.py` & `ProjZ.py-2.4.4/projz/model/blocked_item_wrapper.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/blog.py` & `ProjZ.py-2.4.4/projz/model/blog.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/category.py` & `ProjZ.py-2.4.4/projz/model/category.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/chat.py` & `ProjZ.py-2.4.4/projz/model/chat.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/chat_message.py` & `ProjZ.py-2.4.4/projz/model/chat_message.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/circle.py` & `ProjZ.py-2.4.4/projz/model/circle.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/comment.py` & `ProjZ.py-2.4.4/projz/model/comment.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/currency.py` & `ProjZ.py-2.4.4/projz/model/currency.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/default_background_media.py` & `ProjZ.py-2.4.4/projz/model/default_background_media.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/gift_box.py` & `ProjZ.py-2.4.4/projz/model/gift_box.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/media.py` & `ProjZ.py-2.4.4/projz/model/media.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/member_title.py` & `ProjZ.py-2.4.4/projz/model/member_title.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/parse/parseutils.py` & `ProjZ.py-2.4.4/projz/model/parse/parseutils.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/poll.py` & `ProjZ.py-2.4.4/projz/model/poll.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/qi_vote_full_info.py` & `ProjZ.py-2.4.4/projz/model/qi_vote_full_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/qi_vote_info.py` & `ProjZ.py-2.4.4/projz/model/qi_vote_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/reaction.py` & `ProjZ.py-2.4.4/projz/model/reaction.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/response/member_titles_info.py` & `ProjZ.py-2.4.4/projz/model/response/member_titles_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/response/multi_invitation_code_info.py` & `ProjZ.py-2.4.4/projz/model/response/multi_invitation_code_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/rich_format.py` & `ProjZ.py-2.4.4/projz/model/rich_format.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/transfer_order.py` & `ProjZ.py-2.4.4/projz/model/transfer_order.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/user.py` & `ProjZ.py-2.4.4/projz/model/user.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/user_task.py` & `ProjZ.py-2.4.4/projz/model/user_task.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/util/rich_format_builder.py` & `ProjZ.py-2.4.4/projz/model/util/rich_format_builder.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/util/rich_format_text_builder.py` & `ProjZ.py-2.4.4/projz/model/util/rich_format_text_builder.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/model/wallet.py` & `ProjZ.py-2.4.4/projz/model/wallet.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/util/subscription_handler.py` & `ProjZ.py-2.4.4/projz/util/subscription_handler.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/projz/websocket/websocket_listener.py` & `ProjZ.py-2.4.4/projz/websocket/websocket_listener.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.4.3/setup.py` & `ProjZ.py-2.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,18 @@
             else:
                 print("Failed to install Sox. The stability of the library is not guaranteed.")
         else:
             print("Sox found, no installation required.")
 
     setup(
         name="ProjZ.py",
-        version="2.4.3",
+        version="2.4.4",
         author="D4rkwat3r",
         description="An asynchronous library for creating scripts and chatbots in Project Z.",
+        url="https://github.com/D4rkwat3r/ProjZ",
         packages=find_packages(),
         author_email="ktoya170214@gmail.com",
         install_requires=get_requirements(),
         long_description=get_readme(),
         long_description_content_type="text/markdown",
         python_requires=">=3.7",
         package_data={"projz": ["api/secret/data.txt"]},
```

