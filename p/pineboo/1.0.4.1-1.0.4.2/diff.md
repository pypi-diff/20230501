# Comparing `tmp/pineboo-1.0.4.1.tar.gz` & `tmp/pineboo-1.0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pineboo-1.0.4.1.tar", last modified: Thu Apr 20 15:59:31 2023, max compression
+gzip compressed data, was "pineboo-1.0.4.2.tar", last modified: Mon May  1 18:17:34 2023, max compression
```

## Comparing `pineboo-1.0.4.1.tar` & `pineboo-1.0.4.2.tar`

### file list

```diff
@@ -1,736 +1,736 @@
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.244355 pineboo-1.0.4.1/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1078 2019-07-27 10:21:43.000000 pineboo-1.0.4.1/LICENSE.mit
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5923 2023-04-20 15:59:31.244355 pineboo-1.0.4.1/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4673 2023-04-04 09:45:23.000000 pineboo-1.0.4.1/README.rst
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.128349 pineboo-1.0.4.1/pineboo.egg-info/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5923 2023-04-20 15:59:30.000000 pineboo-1.0.4.1/pineboo.egg-info/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    28782 2023-04-20 15:59:31.000000 pineboo-1.0.4.1/pineboo.egg-info/SOURCES.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-04-20 15:59:30.000000 pineboo-1.0.4.1/pineboo.egg-info/dependency_links.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      386 2023-04-20 15:59:30.000000 pineboo-1.0.4.1/pineboo.egg-info/entry_points.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      584 2023-04-20 15:59:30.000000 pineboo-1.0.4.1/pineboo.egg-info/requires.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-04-20 15:59:30.000000 pineboo-1.0.4.1/pineboo.egg-info/top_level.txt
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.128349 pineboo-1.0.4.1/pineboolib/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      179 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.132350 pineboo-1.0.4.1/pineboolib/application/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1515 2023-04-20 15:58:52.000000 pineboo-1.0.4.1/pineboolib/application/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.132350 pineboo-1.0.4.1/pineboolib/application/acls/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       20 2019-09-08 08:23:19.000000 pineboo-1.0.4.1/pineboolib/application/acls/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9234 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/acls/pnaccesscontrol.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7411 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/acls/pnaccesscontrolfactory.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9900 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/acls/pnaccesscontrollists.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1554 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/acls/pnboolflagstate.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.132350 pineboo-1.0.4.1/pineboolib/application/acls/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      269 2020-08-26 10:35:25.000000 pineboo-1.0.4.1/pineboolib/application/acls/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    24412 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/acls/tests/test_acls.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      970 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/acls/tests/test_pnaccesscontrol.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9013 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/connections.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.132350 pineboo-1.0.4.1/pineboolib/application/database/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      210 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/database/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.132350 pineboo-1.0.4.1/pineboolib/application/database/orm/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       43 2020-05-06 20:13:13.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5021 2022-06-12 18:52:01.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/alembic_tools.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    38001 2023-04-19 12:33:57.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/basemodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6348 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/dummy_cursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1083 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/dummy_signal.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.136350 pineboo-1.0.4.1/pineboolib/application/database/orm/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-06-24 11:26:48.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    12845 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_basemodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2510 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_bytearray.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4361 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_consistency.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3575 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_dummycursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4074 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_query_orm.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4354 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_relationships.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5465 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_sessions.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4746 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_signals.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2524 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_thread_session.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1736 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_utils.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1080 2020-10-15 10:56:54.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_view.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10720 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/database/orm/utils.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8355 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/database/pnbuffer.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    22022 2023-04-20 15:54:14.000000 pineboo-1.0.4.1/pineboolib/application/database/pnconnection.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17300 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/database/pnconnectionmanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    40279 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/database/pncursortablemodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      541 2020-06-29 10:01:24.000000 pineboo-1.0.4.1/pineboolib/application/database/pngroupbyquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      984 2020-01-10 07:21:12.000000 pineboo-1.0.4.1/pineboolib/application/database/pnparameterquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1340 2021-03-09 11:41:24.000000 pineboo-1.0.4.1/pineboolib/application/database/pnsignals.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   122391 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/database/pnsqlcursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5770 2023-04-18 17:17:33.000000 pineboo-1.0.4.1/pineboolib/application/database/pnsqldriversmanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    30552 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/database/pnsqlquery.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.136350 pineboo-1.0.4.1/pineboolib/application/database/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      276 2019-12-02 11:03:25.000000 pineboo-1.0.4.1/pineboolib/application/database/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5986 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/database/tests/test_pnbuffer.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8510 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/database/tests/test_pnconnection.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4011 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/database/tests/test_pnconnection_manager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8048 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/database/tests/test_pncursortablemodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      413 2019-08-28 09:29:35.000000 pineboo-1.0.4.1/pineboolib/application/database/tests/test_pngroupbyquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      600 2019-08-28 09:29:35.000000 pineboo-1.0.4.1/pineboolib/application/database/tests/test_pnparameterquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    42304 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/database/tests/test_pnsqlcursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1170 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/database/tests/test_pnsqldriversmanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    28221 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/database/tests/test_pnsqlquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3072 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/database/tests/test_utils.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15831 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/database/utils.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1475 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/file.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11435 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/load_script.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.136350 pineboo-1.0.4.1/pineboolib/application/metadata/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      166 2019-07-30 14:11:28.000000 pineboo-1.0.4.1/pineboolib/application/metadata/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4940 2021-01-20 09:16:39.000000 pineboo-1.0.4.1/pineboolib/application/metadata/pnaction.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2325 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/metadata/pncompoundkeymetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    33263 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/metadata/pnfieldmetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7344 2021-08-22 09:38:16.000000 pineboo-1.0.4.1/pineboolib/application/metadata/pnrelationmetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    25771 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/metadata/pntablemetadata.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.136350 pineboo-1.0.4.1/pineboolib/application/metadata/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       36 2019-08-03 08:33:48.000000 pineboo-1.0.4.1/pineboolib/application/metadata/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1217 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/metadata/tests/test_pnaction.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2311 2020-02-05 09:39:18.000000 pineboo-1.0.4.1/pineboolib/application/metadata/tests/test_pncompoundkeymetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    16137 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/metadata/tests/test_pnfieldmetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4190 2021-08-23 10:27:07.000000 pineboo-1.0.4.1/pineboolib/application/metadata/tests/test_pnrelationmetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7444 2021-01-21 09:59:47.000000 pineboo-1.0.4.1/pineboolib/application/metadata/tests/test_pntablemetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2862 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/module.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4141 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/moduleactions.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       47 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/modules_tree.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.136350 pineboo-1.0.4.1/pineboolib/application/packager/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      122 2019-07-31 07:36:22.000000 pineboo-1.0.4.1/pineboolib/application/packager/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10703 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/packager/pnpackager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1947 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/packager/pnunpacker.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.136350 pineboo-1.0.4.1/pineboolib/application/packager/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-01-21 10:44:31.000000 pineboo-1.0.4.1/pineboolib/application/packager/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1763 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/packager/tests/test_pnpackager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1519 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/packager/tests/test_pnunpaker.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.136350 pineboo-1.0.4.1/pineboolib/application/parsers/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       70 2019-07-29 14:08:13.000000 pineboo-1.0.4.1/pineboolib/application/parsers/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.140350 pineboo-1.0.4.1/pineboolib/application/parsers/parser_kut/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       56 2020-04-23 09:34:52.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_kut/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    14822 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_kut/kparsertools.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    43978 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_kut/kut2fpdf.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.140350 pineboo-1.0.4.1/pineboolib/application/parsers/parser_kut/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      291 2020-04-23 09:34:52.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_kut/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10578 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_kut/tests/test_parser_kut.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.140350 pineboo-1.0.4.1/pineboolib/application/parsers/parser_mtd/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       50 2020-04-23 09:34:52.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_mtd/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    14324 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_mtd/pnmtdparser.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5406 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_mtd/pnormmodelsfactory.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.140350 pineboo-1.0.4.1/pineboolib/application/parsers/parser_mtd/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2020-04-23 09:34:52.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_mtd/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1885 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_mtd/tests/test_parser_mtd.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.140350 pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      587 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/flex.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    31513 2023-04-05 17:06:58.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/flscriptparse.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3400 2020-04-23 09:34:52.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/lextab.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    28469 2023-04-05 17:06:58.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/postparse.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8654 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/pyconvert.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    91905 2023-04-07 16:35:34.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/pytnyzer.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.140350 pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      502 2020-04-23 09:34:52.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    16289 2023-04-07 15:09:35.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/tests/test_parser_qsa.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6174 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/token_rules.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.140350 pineboo-1.0.4.1/pineboolib/application/parsers/parser_ui/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      101 2020-04-23 09:34:52.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_ui/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    49421 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_ui/qt3ui.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.140350 pineboo-1.0.4.1/pineboolib/application/parsers/parser_ui/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       33 2020-04-23 09:34:52.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_ui/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1627 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/parsers/parser_ui/tests/test_parser_ui.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    34668 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/pnapplication.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      371 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/pncore.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6753 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/process.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    27110 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/projectmodule.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3641 2021-03-30 10:58:34.000000 pineboo-1.0.4.1/pineboolib/application/proxy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6876 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/qsadictmodules.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.140350 pineboo-1.0.4.1/pineboolib/application/qsatypes/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       28 2019-08-01 20:49:12.000000 pineboo-1.0.4.1/pineboolib/application/qsatypes/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7965 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/qsatypes/date.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    20095 2023-04-18 17:17:37.000000 pineboo-1.0.4.1/pineboolib/application/qsatypes/sysbasetype.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.140350 pineboo-1.0.4.1/pineboolib/application/qsatypes/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       36 2019-08-06 06:55:22.000000 pineboo-1.0.4.1/pineboolib/application/qsatypes/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1853 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/qsatypes/tests/test_date.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5455 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/qsatypes/tests/test_sysbasetype.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3461 2021-03-29 11:28:24.000000 pineboo-1.0.4.1/pineboolib/application/safeqsa.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.140350 pineboo-1.0.4.1/pineboolib/application/signatures/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       26 2020-12-25 17:46:05.000000 pineboo-1.0.4.1/pineboolib/application/signatures/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6312 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/signatures/pdf_digest.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8187 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/signatures/pdf_qr.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.140350 pineboo-1.0.4.1/pineboolib/application/signatures/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      286 2021-01-18 11:51:09.000000 pineboo-1.0.4.1/pineboolib/application/signatures/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3440 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/signatures/tests/test_signatures.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9298 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/signatures/xml_digest.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.140350 pineboo-1.0.4.1/pineboolib/application/staticloader/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       28 2019-10-04 20:53:14.000000 pineboo-1.0.4.1/pineboolib/application/staticloader/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    14695 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/staticloader/pnmodulesstaticloader.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.140350 pineboo-1.0.4.1/pineboolib/application/staticloader/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      289 2020-09-07 08:35:55.000000 pineboo-1.0.4.1/pineboolib/application/staticloader/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2491 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/staticloader/tests/test_static_loader.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.140350 pineboo-1.0.4.1/pineboolib/application/staticloader/ui/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2020-08-17 12:14:19.000000 pineboo-1.0.4.1/pineboolib/application/staticloader/ui/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7299 2020-03-10 09:40:23.000000 pineboo-1.0.4.1/pineboolib/application/staticloader/ui/static_loader.ui
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.144350 pineboo-1.0.4.1/pineboolib/application/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      287 2019-10-09 06:29:09.000000 pineboo-1.0.4.1/pineboolib/application/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1627 2020-06-10 19:38:58.000000 pineboo-1.0.4.1/pineboolib/application/tests/test_application.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1350 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/tests/test_load_script.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1309 2020-09-21 07:02:30.000000 pineboo-1.0.4.1/pineboolib/application/tests/test_process.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1259 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/tests/test_projectmodule.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      686 2020-09-04 08:27:19.000000 pineboo-1.0.4.1/pineboolib/application/tests/test_proxy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    16925 2023-04-07 15:43:24.000000 pineboo-1.0.4.1/pineboolib/application/tests/test_types.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1319 2020-09-07 08:35:55.000000 pineboo-1.0.4.1/pineboolib/application/tests/test_xmlaction.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.144350 pineboo-1.0.4.1/pineboolib/application/translator/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       26 2020-04-05 08:54:23.000000 pineboo-1.0.4.1/pineboolib/application/translator/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5405 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/translator/pntranslator.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.144350 pineboo-1.0.4.1/pineboolib/application/translator/test/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       34 2020-12-01 12:01:44.000000 pineboo-1.0.4.1/pineboolib/application/translator/test/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      802 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/translator/test/test_pntranslator.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    22047 2023-04-09 14:08:33.000000 pineboo-1.0.4.1/pineboolib/application/types.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.144350 pineboo-1.0.4.1/pineboolib/application/utils/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      182 2019-07-31 08:47:54.000000 pineboo-1.0.4.1/pineboolib/application/utils/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1548 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/utils/check_dependencies.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2245 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/utils/convert_flaction.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2430 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/utils/date_conversion.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6310 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/application/utils/flfiles_dir.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1120 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/utils/geometry.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1949 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/utils/mobilemode.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2296 2023-04-20 15:55:05.000000 pineboo-1.0.4.1/pineboolib/application/utils/modules.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1626 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/utils/path.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4727 2020-11-25 10:48:38.000000 pineboo-1.0.4.1/pineboolib/application/utils/service.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    23037 2023-04-19 12:18:00.000000 pineboo-1.0.4.1/pineboolib/application/utils/sql_tools.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1307 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/utils/xpm.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15051 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/application/xmlaction.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.144350 pineboo-1.0.4.1/pineboolib/core/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      268 2021-03-29 11:28:24.000000 pineboo-1.0.4.1/pineboolib/core/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8761 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/core/decorators.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      746 2020-10-16 07:17:25.000000 pineboo-1.0.4.1/pineboolib/core/exceptions.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.144350 pineboo-1.0.4.1/pineboolib/core/fonts/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2019-09-17 09:33:15.000000 pineboo-1.0.4.1/pineboolib/core/fonts/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.144350 pineboo-1.0.4.1/pineboolib/core/fonts/noto_sans/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2020-03-09 09:55:39.000000 pineboo-1.0.4.1/pineboolib/core/fonts/noto_sans/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2578 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/core/garbage_collector.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.144350 pineboo-1.0.4.1/pineboolib/core/images/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-09-17 09:33:15.000000 pineboo-1.0.4.1/pineboolib/core/images/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.164351 pineboo-1.0.4.1/pineboolib/core/images/icono_pi/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      960 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Pi-symbol.svg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)  1464366 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi.psd
--rw-rw-r--   0 aulla     (1000) aulla     (1000)  9487782 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi2.xcf
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   476635 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi2_1024.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    50853 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi2_256.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   147180 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi2_512.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    50737 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi_1024.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15871 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi_256.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    29321 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi_512.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       25 2019-09-17 09:33:15.000000 pineboo-1.0.4.1/pineboolib/core/images/icono_pi/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.192352 pineboo-1.0.4.1/pineboolib/core/images/icons/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2019-09-17 09:33:15.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/__init__.py
--rwxrwxr-x   0 aulla     (1000) aulla     (1000)      892 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/about.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1230 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/aboutqt.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      853 2019-10-01 07:14:24.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/cancel.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      571 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/consola.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      669 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/date.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2199 2019-09-30 08:28:48.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/delete.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2562 2019-10-01 07:14:24.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/down.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2069 2019-09-30 08:28:48.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/edit.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2237 2020-01-15 08:29:51.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/edit_file.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1657 2020-01-15 08:29:51.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/edit_file_xml.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      934 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/estilo.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      870 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/exit.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      464 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/flfielddb.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      691 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/fltable-clean.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      526 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/fltable-data.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      464 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/fltable-filter.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      727 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/fltable-odf.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      459 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/folder.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      615 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/folder_update.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      563 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/font.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1263 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/go-bottom.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1187 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/go-down.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/go-first.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1774 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/go-home.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/go-jump.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/go-last.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/go-next.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/go-previous.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1293 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/go-top.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1193 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/go-up.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      601 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-add.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1624 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-bold.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1927 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-cancel.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1682 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-clear.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      723 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-copy.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2087 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-cut.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2049 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-delete.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2104 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-find-and-replace.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1636 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-find.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1256 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-fullscreen.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-go-back-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-go-back-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1187 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-go-down.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-go-forward-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-go-forward-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1193 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-go-up.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1263 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-goto-bottom.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-goto-first-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-goto-first-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-goto-last-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-goto-last-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1293 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-goto-top.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1774 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-home.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      766 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-indent-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      767 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-indent-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1338 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-italic.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-jump-to-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-jump-to-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      526 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-justify-center.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      517 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-justify-fill.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      515 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-justify-left.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      541 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-justify-right.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1205 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-forward-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1074 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-forward-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1225 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-next-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1236 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-next-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      481 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-pause.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1028 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-play-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1236 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-previous-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1225 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-previous-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1266 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-record.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1074 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-rewind-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1205 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-rewind-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      571 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-stop.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1008 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-new.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1550 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-open.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1027 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-paste.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1719 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-print-preview.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1013 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-print.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1115 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-properties.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1502 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-redo-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-refresh.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      317 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-remove.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1837 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-save-as.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1971 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-save.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      631 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-select-all.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1927 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-stop.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1445 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-strikethrough.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1550 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-underline.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1601 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-undo-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      767 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-unindent-ltr.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      766 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-unindent-rtl.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      911 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/help_index.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1854 2019-09-30 08:28:48.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/insert.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      711 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/lock.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      579 2019-10-01 07:14:24.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/ok.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1997 2019-09-30 08:28:48.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/paste.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6800 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-128.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      857 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-16.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1406 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-24.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15871 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-256.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1941 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-32.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2991 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-48.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3482 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-57.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3243 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-64.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3641 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-72.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6800 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19949 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo-128.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1216 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo-16.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1720 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo-24.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    52103 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo-256.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2568 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo-32.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4552 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo-48.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7028 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo-64.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17588 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2019-09-30 08:28:48.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/print.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      885 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/reload.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    22869 2022-07-06 21:01:18.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/signed_stamp.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1930 2019-10-02 12:19:59.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/sys_ebcomportamiento.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1571 2019-10-02 12:19:59.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flareas.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2952 2019-10-02 12:19:59.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/sys_fldumpdb.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1133 2019-10-02 12:19:59.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flgroups.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1871 2019-10-02 12:19:59.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flloadmod.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2404 2019-10-02 12:19:59.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flloadmodpkg.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1335 2019-10-02 12:19:59.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flmodules.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2010 2019-10-02 12:19:59.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flmrproper.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2334 2019-10-02 12:19:59.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flreinit.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2771 2019-10-02 12:19:59.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flreloadbatch.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1731 2019-10-02 12:19:59.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flreloadlast.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2194 2019-10-02 12:19:59.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flusers.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    35029 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/terminal.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      638 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/unlock.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2635 2019-10-01 07:14:24.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/up.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2325 2019-09-30 08:28:48.000000 pineboo-1.0.4.1/pineboolib/core/images/icons/zoom.png
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.196353 pineboo-1.0.4.1/pineboolib/core/images/splashscreen/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-09-17 09:33:15.000000 pineboo-1.0.4.1/pineboolib/core/images/splashscreen/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    72306 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/splashscreen/dbadmin240.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   187209 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/splashscreen/dbadmin480.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    71281 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/splashscreen/quick240.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   185547 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/splashscreen/quick480.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       52 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/splashscreen/readme
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    66162 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/splashscreen/splash.png
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   109093 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/core/images/splashscreen/splash.svg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1150 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/core/message_manager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4314 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/core/settings.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      426 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/core/system.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.196353 pineboo-1.0.4.1/pineboolib/core/test/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2020-09-21 07:02:47.000000 pineboo-1.0.4.1/pineboolib/core/test/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1215 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/core/test/test_settings.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      211 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/core/translate.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.196353 pineboo-1.0.4.1/pineboolib/core/utils/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      114 2019-07-28 13:56:09.000000 pineboo-1.0.4.1/pineboolib/core/utils/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3203 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/core/utils/check_dependencies.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3140 2020-03-10 08:41:03.000000 pineboo-1.0.4.1/pineboolib/core/utils/logging.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      540 2019-07-28 13:56:09.000000 pineboo-1.0.4.1/pineboolib/core/utils/singleton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3720 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/core/utils/struct.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.196353 pineboo-1.0.4.1/pineboolib/core/utils/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       46 2019-08-04 20:13:49.000000 pineboo-1.0.4.1/pineboolib/core/utils/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2331 2020-03-09 12:29:25.000000 pineboo-1.0.4.1/pineboolib/core/utils/tests/test_utils_base.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1819 2020-09-21 06:32:29.000000 pineboo-1.0.4.1/pineboolib/core/utils/tests/test_version.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15945 2023-04-19 12:18:00.000000 pineboo-1.0.4.1/pineboolib/core/utils/utils_base.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4686 2021-03-08 21:10:30.000000 pineboo-1.0.4.1/pineboolib/core/utils/version.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.204353 pineboo-1.0.4.1/pineboolib/fllegacy/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      111 2019-07-31 21:01:09.000000 pineboo-1.0.4.1/pineboolib/fllegacy/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.208353 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       77 2019-07-31 16:14:18.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      349 2019-11-28 09:34:37.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqboolflagstate.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      580 2020-11-10 11:32:00.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqformdb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      984 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqobjectquerylist.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13444 2022-07-05 09:51:12.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqods.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6753 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      521 2020-03-09 11:54:38.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqsbuttongroup.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      243 2019-07-31 20:16:08.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqsettings.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      337 2019-11-18 12:56:58.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqshttp.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      167 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqsignalmapper.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      241 2019-07-31 20:16:08.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqsmtpclient.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1531 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqsobjectfactory.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18185 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqsql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      273 2019-11-28 09:34:37.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqsqlcursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      255 2019-07-31 20:16:08.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqsqlquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      734 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqssproject.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      343 2020-09-14 10:30:41.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqutil.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.208353 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-08-29 15:57:47.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1300 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/tests/test_aqobjectquerylist.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1201 2020-12-01 12:01:57.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/tests/test_aqods.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1907 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/tests/test_aqs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      554 2020-04-21 15:32:44.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/tests/test_aqsbuttongroup.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1194 2020-08-07 17:51:40.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/tests/test_aqsql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      953 2020-02-11 09:11:31.000000 pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/tests/test_aqutil.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      358 2019-09-19 09:51:37.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flaction.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      171 2020-04-02 16:10:18.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flapplication.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      446 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flcheckbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    12411 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flcodbar.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    29167 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/fldatatable.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1657 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/fldateedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2319 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/fldoublevalidator.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2020-08-24 08:14:25.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flfastcgi.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   143170 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flfielddb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    31497 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flformdb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    34481 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flformrecorddb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    14097 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flformsearchdb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      185 2019-08-01 06:59:07.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flgroupbyquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1361 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flintvalidator.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      161 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/fljasperengine.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      103 2020-08-19 14:34:59.000000 pineboo-1.0.4.1/pineboolib/fllegacy/fljasperviewer.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5497 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/fllineedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3892 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/fllistviewitem.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    52856 2023-04-19 12:33:57.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flmanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    28979 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flmanagermodules.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4403 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flnetwork.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      196 2019-08-17 07:43:18.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flparameterquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4300 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flpixmapview.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3702 2020-08-24 09:53:53.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flposprinter.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13824 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flreportengine.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    22476 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flreportviewer.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      403 2019-11-14 09:39:09.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flscripteditor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5273 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flserialport.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1620 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flsettings.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13515 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flsmtpclient.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      895 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flspinbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      267 2020-03-05 11:36:30.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flsqlconnections.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      167 2019-08-17 07:43:18.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flsqlcursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      161 2019-08-17 07:43:18.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flsqlquery.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      686 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/fltable.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)   108501 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/fltabledb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      875 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/fltimeedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1092 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/fluintvalidator.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    41598 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flutil.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1876 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flvar.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      549 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      315 2019-08-13 07:00:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/flworkspace.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.208353 pineboo-1.0.4.1/pineboolib/fllegacy/forms/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    48049 2020-12-24 07:51:30.000000 pineboo-1.0.4.1/pineboolib/fllegacy/forms/FLWidgetReportViewer.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       67 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/forms/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67146 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/systype.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.208353 pineboo-1.0.4.1/pineboolib/fllegacy/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2019-12-02 11:03:25.000000 pineboo-1.0.4.1/pineboolib/fllegacy/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1455 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flcodbar.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1664 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_fldatatable.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      991 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_fldateedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8825 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flfielddb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      939 2020-09-21 06:32:29.000000 pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flform.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2286 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flformrecorddb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3065 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flformsearch.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2289 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flmanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      902 2020-12-22 09:37:36.000000 pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flreportengine.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    12536 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_fltabledb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8666 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flutil.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1592 2020-09-01 07:21:14.000000 pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_settings.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1192 2020-09-01 07:21:14.000000 pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_smtp.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8560 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_systype.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.212353 pineboo-1.0.4.1/pineboolib/interfaces/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      331 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/interfaces/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      172 2019-07-31 18:05:01.000000 pineboo-1.0.4.1/pineboolib/interfaces/cursoraccessmode.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      228 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/interfaces/dgi_schema.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10886 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/interfaces/iconnection.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5925 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/interfaces/ifieldmetadata.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2999 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/interfaces/imainwindow.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5542 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/interfaces/imanager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/interfaces/isession.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    21668 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/interfaces/isqlcursor.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    50302 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/interfaces/isqldriver.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3292 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/interfaces/itablemetadata.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.212353 pineboo-1.0.4.1/pineboolib/loader/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       92 2019-08-04 07:50:46.000000 pineboo-1.0.4.1/pineboolib/loader/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/loader/connection.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1546 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/loader/dgi.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.212353 pineboo-1.0.4.1/pineboolib/loader/dlgconnect/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      104 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/loader/dlgconnect/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      716 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/loader/dlgconnect/conn_dialog.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15802 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/loader/dlgconnect/dlgconnect.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    24027 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/loader/dlgconnect/dlgconnect.ui
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.212353 pineboo-1.0.4.1/pineboolib/loader/dlgconnect/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       57 2020-12-02 18:09:30.000000 pineboo-1.0.4.1/pineboolib/loader/dlgconnect/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2544 2020-11-09 16:02:09.000000 pineboo-1.0.4.1/pineboolib/loader/dlgconnect/tests/test_dlgconnect.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2870 2023-04-20 08:48:34.000000 pineboo-1.0.4.1/pineboolib/loader/init_project.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18287 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/loader/main.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5772 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/loader/options.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1311 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/loader/preload.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17570 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/loader/projectconfig.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.212353 pineboo-1.0.4.1/pineboolib/loader/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      477 2019-08-05 15:23:25.000000 pineboo-1.0.4.1/pineboolib/loader/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2495 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/loader/tests/test_connection.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      827 2021-03-08 11:35:13.000000 pineboo-1.0.4.1/pineboolib/loader/tests/test_main.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4314 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/loader/tests/test_projectconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3682 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/loader/utils.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.212353 pineboo-1.0.4.1/pineboolib/plugins/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       23 2019-08-18 15:38:56.000000 pineboo-1.0.4.1/pineboolib/plugins/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.212353 pineboo-1.0.4.1/pineboolib/plugins/custom_widgets/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      282 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/custom_widgets/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      462 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/custom_widgets/flfielddb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      456 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/custom_widgets/fltable.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      462 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/custom_widgets/fltabledb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      456 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/custom_widgets/pncore.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.216354 pineboo-1.0.4.1/pineboolib/plugins/dgi/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       19 2019-08-18 15:38:56.000000 pineboo-1.0.4.1/pineboolib/plugins/dgi/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.216354 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_fcgi/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2019-08-18 15:38:56.000000 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_fcgi/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2848 2020-03-24 12:23:10.000000 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_fcgi/dgi_fcgi.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.216354 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-08-18 15:38:56.000000 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.216354 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_objects/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2019-08-18 15:38:56.000000 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_objects/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.216354 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       25 2019-08-18 15:38:56.000000 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2014 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9496 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2190 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1452 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_objects/splash_screen.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      604 2020-04-02 16:10:18.000000 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_objects/status_help_msg.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4643 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_qt.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5507 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_schema.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.216354 pineboo-1.0.4.1/pineboolib/plugins/mainform/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      177 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/mainform/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.216354 pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       78 2019-07-30 09:20:57.000000 pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    55893 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo/eneboo.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4184 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo/mainform.ui
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.216354 pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      276 2019-11-04 08:30:07.000000 pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5085 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo/tests/test_eneboo.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.216354 pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo_mdi/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       82 2019-07-30 09:20:57.000000 pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo_mdi/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    49501 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo_mdi/eneboo_mdi.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1500 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo_mdi/mainform.ui
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.216354 pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo_mdi/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      280 2019-11-04 08:30:07.000000 pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo_mdi/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3263 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo_mdi/tests/test_eneboo_mdi.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.216354 pineboo-1.0.4.1/pineboolib/plugins/sql/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-08-18 13:55:56.000000 pineboo-1.0.4.1/pineboolib/plugins/sql/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      483 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/sql/flmysql_innodb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    12024 2023-04-19 12:33:54.000000 pineboo-1.0.4.1/pineboolib/plugins/sql/flmysql_myisam.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11877 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/plugins/sql/flpymssql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      825 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/sql/flpyodbc.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13367 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/sql/flqpsql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11393 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/plugins/sql/flsqlite.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.220354 pineboo-1.0.4.1/pineboolib/plugins/sql/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       31 2020-09-17 10:11:16.000000 pineboo-1.0.4.1/pineboolib/plugins/sql/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2172 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/sql/tests/test_flmysql_innodb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2958 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/sql/tests/test_flmysql_myisam.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2861 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/sql/tests/test_flpymssql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2087 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/sql/tests/test_flpyodbc.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4517 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/sql/tests/test_flsqlite.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2095 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/sql/tests/test_qpsql.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9177 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/plugins/sql/tests/test_stress.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2019-07-27 10:21:43.000000 pineboo-1.0.4.1/pineboolib/py.typed
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.228354 pineboo-1.0.4.1/pineboolib/q3widgets/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       94 2019-09-27 15:43:59.000000 pineboo-1.0.4.1/pineboolib/q3widgets/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1761 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/checkbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      142 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/combobox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1398 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/dateedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3877 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/dialog.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1634 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/filedialog.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      482 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/groupbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      118 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/line.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1061 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/lineedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3554 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/messagebox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2758 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/numberedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      443 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/picture.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      134 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/pixmap.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1109 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qaction.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      887 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qbuttongroup.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1541 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qbytearray.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      774 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qcheckbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2176 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qcombobox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      138 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qdataview.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2262 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qdateedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      147 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qdatetime.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1663 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qdialog.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      237 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qdir.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      316 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qeventloop.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1138 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qframe.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3328 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qgroupbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      656 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qhboxlayout.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      348 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qhbuttongroup.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17321 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qhttp.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      231 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qiconset.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2061 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qlabel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      144 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qlayoutwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1099 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qline.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1767 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qlineedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5684 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qlistview.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      173 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qlistviewwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      445 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qmainwindow.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      137 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qmenu.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      153 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qmessagebox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1668 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qobject.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      153 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qpopupmenu.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3111 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qpushbutton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1975 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qradiobutton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      149 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qspinbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    12608 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qtable.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1741 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qtabwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2013 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qtextedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      463 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qtextstream.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      926 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qtimeedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      404 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qtoolbar.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2255 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qtoolbutton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      654 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qvboxlayout.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      348 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qvbuttongroup.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1231 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/qwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      184 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/radiobutton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      128 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/rect.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      128 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/size.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1731 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/spinbox.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.228354 pineboo-1.0.4.1/pineboolib/q3widgets/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      278 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      470 2019-12-19 10:11:59.000000 pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_dateedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1411 2020-12-02 18:08:18.000000 pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_messagebox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      646 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_qbytearray.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2638 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_qhttp.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      719 2019-09-27 15:43:59.000000 pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_qpushbutton.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1163 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_qradiobuttons.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1131 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_qtabwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1046 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_qtextstream.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      532 2020-09-21 08:32:33.000000 pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_spinbox.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/textedit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/q3widgets/timeedit.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.232354 pineboo-1.0.4.1/pineboolib/qsa/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       95 2019-08-02 07:28:39.000000 pineboo-1.0.4.1/pineboolib/qsa/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     5934 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/qsa/decorators.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1321 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/qsa/emptyscript.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7457 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/qsa/formdbwidget.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2035 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/qsa/input.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1439 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/qsa/object_class.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11935 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/qsa/pncontrolsfactory.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8336 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/qsa/qsa.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.232354 pineboo-1.0.4.1/pineboolib/qsa/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      496 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/qsa/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      744 2020-06-22 11:35:54.000000 pineboo-1.0.4.1/pineboolib/qsa/tests/test_class.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4169 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/qsa/tests/test_classes.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    17795 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/qsa/tests/test_knownbugs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6680 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/qsa/tests/test_orm.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1563 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/qsa/tests/test_query_values.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1723 2023-04-05 17:06:58.000000 pineboo-1.0.4.1/pineboolib/qsa/tests/test_require.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7893 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/qsa/tests/test_utils.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    20220 2023-04-05 17:06:58.000000 pineboo-1.0.4.1/pineboolib/qsa/utils.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.232354 pineboo-1.0.4.1/pineboolib/system_module/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       29 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/system_module/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.236354 pineboo-1.0.4.1/pineboolib/system_module/forms/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9153 2019-09-30 08:28:05.000000 pineboo-1.0.4.1/pineboolib/system_module/forms/FLWidgetMasterTable.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-09-17 09:33:15.000000 pineboo-1.0.4.1/pineboolib/system_module/forms/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    28933 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/forms/ebcomportamiento.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1368 2019-10-01 07:14:24.000000 pineboo-1.0.4.1/pineboolib/system_module/forms/flareas.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2994 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/forms/flfiles.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8007 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/forms/flgroups.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    16760 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/forms/flmodulos.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3150 2020-07-06 10:29:58.000000 pineboo-1.0.4.1/pineboolib/system_module/forms/fltest.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1214 2019-10-01 07:14:24.000000 pineboo-1.0.4.1/pineboolib/system_module/forms/flusers.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8877 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/forms/master.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10189 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/forms/master_copy.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9932 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/forms/master_print.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11619 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/forms/master_print_copy.ui
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    11760 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/forms/sys.ui
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.240355 pineboo-1.0.4.1/pineboolib/system_module/models/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2020-04-27 09:01:43.000000 pineboo-1.0.4.1/pineboolib/system_module/models/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1441 2020-07-16 10:23:10.000000 pineboo-1.0.4.1/pineboolib/system_module/models/flareas_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3270 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/system_module/models/flfiles_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1238 2020-07-16 10:23:10.000000 pineboo-1.0.4.1/pineboolib/system_module/models/flgroups_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1192 2020-07-16 10:23:10.000000 pineboo-1.0.4.1/pineboolib/system_module/models/fllarge_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1313 2020-07-16 10:23:10.000000 pineboo-1.0.4.1/pineboolib/system_module/models/flmetadata_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3296 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/models/flmodules_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1292 2020-07-16 10:23:10.000000 pineboo-1.0.4.1/pineboolib/system_module/models/flseqs_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1007 2020-07-16 10:23:10.000000 pineboo-1.0.4.1/pineboolib/system_module/models/flserial_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1023 2020-07-16 10:23:10.000000 pineboo-1.0.4.1/pineboolib/system_module/models/flsettings_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2369 2020-07-16 10:23:10.000000 pineboo-1.0.4.1/pineboolib/system_module/models/fltest2_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1769 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/models/fltest3_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1859 2020-07-16 10:23:10.000000 pineboo-1.0.4.1/pineboolib/system_module/models/fltest4_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2296 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/models/fltest5_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2659 2020-10-13 15:24:00.000000 pineboo-1.0.4.1/pineboolib/system_module/models/fltest_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3548 2020-07-16 10:23:10.000000 pineboo-1.0.4.1/pineboolib/system_module/models/flupdates_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1450 2020-07-16 10:23:10.000000 pineboo-1.0.4.1/pineboolib/system_module/models/flusers_model.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1718 2020-07-16 10:23:10.000000 pineboo-1.0.4.1/pineboolib/system_module/models/flvar_model.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.240355 pineboo-1.0.4.1/pineboolib/system_module/queries/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2019-09-17 09:33:15.000000 pineboo-1.0.4.1/pineboolib/system_module/queries/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      636 2020-10-15 10:53:48.000000 pineboo-1.0.4.1/pineboolib/system_module/queries/fltest2.qry
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.240355 pineboo-1.0.4.1/pineboolib/system_module/scripts/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15186 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/ebcomportamiento.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      234 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/fldumpdb.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      859 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/flfiles.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2430 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/flloadmod.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      246 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/flloadmodpkg.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      427 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/flmasterareas.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18788 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/flmodules.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      243 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/flmrproper.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      238 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/flreinit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3958 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/flreloadbatch.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6038 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/flreloadlast.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      138 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/fltest6.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4351 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/sys.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.244355 pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-03-26 18:29:13.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1104 2020-09-17 09:48:31.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_ebcomportamiento.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2155 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_flfiles.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      646 2020-09-09 10:25:36.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_flloadmodpkg.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4238 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_flmodules.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      843 2020-09-09 10:25:36.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_flmrproper.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      851 2020-09-09 10:25:36.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_flreinit.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4322 2023-04-20 08:16:40.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_reload_last.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1564 2019-09-26 11:40:44.000000 pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_sys.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2411 2020-12-05 19:13:31.000000 pineboo-1.0.4.1/pineboolib/system_module/sys.xml
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6505 2019-08-23 10:35:06.000000 pineboo-1.0.4.1/pineboolib/system_module/sys.xpm
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.244355 pineboo-1.0.4.1/pineboolib/system_module/translations/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       29 2019-09-17 09:33:15.000000 pineboo-1.0.4.1/pineboolib/system_module/translations/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-04-20 15:59:22.000000 pineboo-1.0.4.1/pineboolib/system_module/translations/sys.ca.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-04-20 15:59:24.000000 pineboo-1.0.4.1/pineboolib/system_module/translations/sys.de.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-04-20 15:59:20.000000 pineboo-1.0.4.1/pineboolib/system_module/translations/sys.en.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    68138 2023-04-20 15:59:19.000000 pineboo-1.0.4.1/pineboolib/system_module/translations/sys.es.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-04-20 15:59:25.000000 pineboo-1.0.4.1/pineboolib/system_module/translations/sys.fr.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-04-20 15:59:27.000000 pineboo-1.0.4.1/pineboolib/system_module/translations/sys.gl.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-04-20 15:59:29.000000 pineboo-1.0.4.1/pineboolib/system_module/translations/sys.it.ts
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-04-20 15:59:30.000000 pineboo-1.0.4.1/pineboolib/system_module/translations/sys.pt.ts
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-20 15:59:31.244355 pineboo-1.0.4.1/pymodules/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2020-11-25 08:02:11.000000 pineboo-1.0.4.1/pymodules/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      283 2023-04-20 15:59:31.244355 pineboo-1.0.4.1/setup.cfg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4086 2023-04-04 09:45:24.000000 pineboo-1.0.4.1/setup.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.985617 pineboo-1.0.4.2/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1078 2019-07-27 10:21:43.000000 pineboo-1.0.4.2/LICENSE.mit
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5923 2023-05-01 18:17:34.985617 pineboo-1.0.4.2/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4673 2023-04-04 09:45:23.000000 pineboo-1.0.4.2/README.rst
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.901615 pineboo-1.0.4.2/pineboo.egg-info/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5923 2023-05-01 18:17:34.000000 pineboo-1.0.4.2/pineboo.egg-info/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    28782 2023-05-01 18:17:34.000000 pineboo-1.0.4.2/pineboo.egg-info/SOURCES.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-05-01 18:17:34.000000 pineboo-1.0.4.2/pineboo.egg-info/dependency_links.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      386 2023-05-01 18:17:34.000000 pineboo-1.0.4.2/pineboo.egg-info/entry_points.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      584 2023-05-01 18:17:34.000000 pineboo-1.0.4.2/pineboo.egg-info/requires.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-05-01 18:17:34.000000 pineboo-1.0.4.2/pineboo.egg-info/top_level.txt
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.901615 pineboo-1.0.4.2/pineboolib/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      179 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.901615 pineboo-1.0.4.2/pineboolib/application/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1515 2023-05-01 18:17:00.000000 pineboo-1.0.4.2/pineboolib/application/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.901615 pineboo-1.0.4.2/pineboolib/application/acls/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       20 2019-09-08 08:23:19.000000 pineboo-1.0.4.2/pineboolib/application/acls/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9234 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/acls/pnaccesscontrol.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7411 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/acls/pnaccesscontrolfactory.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9900 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/acls/pnaccesscontrollists.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1554 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/acls/pnboolflagstate.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.901615 pineboo-1.0.4.2/pineboolib/application/acls/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      269 2020-08-26 10:35:25.000000 pineboo-1.0.4.2/pineboolib/application/acls/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    24412 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/acls/tests/test_acls.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      970 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/acls/tests/test_pnaccesscontrol.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9013 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/connections.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.901615 pineboo-1.0.4.2/pineboolib/application/database/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      210 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/database/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.901615 pineboo-1.0.4.2/pineboolib/application/database/orm/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       43 2020-05-06 20:13:13.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5021 2022-06-12 18:52:01.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/alembic_tools.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    38001 2023-04-19 12:33:57.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/basemodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6348 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/dummy_cursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1083 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/dummy_signal.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.905615 pineboo-1.0.4.2/pineboolib/application/database/orm/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-06-24 11:26:48.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    12845 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_basemodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2510 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_bytearray.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4361 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_consistency.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3575 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_dummycursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4074 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_query_orm.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4354 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_relationships.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5465 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_sessions.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4746 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_signals.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2524 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_thread_session.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1736 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_utils.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1080 2020-10-15 10:56:54.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_view.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10720 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/database/orm/utils.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8355 2023-04-30 08:30:37.000000 pineboo-1.0.4.2/pineboolib/application/database/pnbuffer.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    22022 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/database/pnconnection.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17300 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/database/pnconnectionmanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    40279 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/database/pncursortablemodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      541 2020-06-29 10:01:24.000000 pineboo-1.0.4.2/pineboolib/application/database/pngroupbyquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      984 2020-01-10 07:21:12.000000 pineboo-1.0.4.2/pineboolib/application/database/pnparameterquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1340 2021-03-09 11:41:24.000000 pineboo-1.0.4.2/pineboolib/application/database/pnsignals.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   122391 2023-05-01 17:34:43.000000 pineboo-1.0.4.2/pineboolib/application/database/pnsqlcursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5770 2023-04-18 17:17:33.000000 pineboo-1.0.4.2/pineboolib/application/database/pnsqldriversmanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    30552 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/database/pnsqlquery.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.905615 pineboo-1.0.4.2/pineboolib/application/database/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      276 2019-12-02 11:03:25.000000 pineboo-1.0.4.2/pineboolib/application/database/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5986 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/database/tests/test_pnbuffer.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8510 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/database/tests/test_pnconnection.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4011 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/database/tests/test_pnconnection_manager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8048 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/database/tests/test_pncursortablemodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      413 2019-08-28 09:29:35.000000 pineboo-1.0.4.2/pineboolib/application/database/tests/test_pngroupbyquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      600 2019-08-28 09:29:35.000000 pineboo-1.0.4.2/pineboolib/application/database/tests/test_pnparameterquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    42304 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/database/tests/test_pnsqlcursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1170 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/database/tests/test_pnsqldriversmanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    28221 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/database/tests/test_pnsqlquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3072 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/database/tests/test_utils.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15831 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/database/utils.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1475 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/file.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11435 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/load_script.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.905615 pineboo-1.0.4.2/pineboolib/application/metadata/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      166 2019-07-30 14:11:28.000000 pineboo-1.0.4.2/pineboolib/application/metadata/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4940 2021-01-20 09:16:39.000000 pineboo-1.0.4.2/pineboolib/application/metadata/pnaction.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2325 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/metadata/pncompoundkeymetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    33263 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/metadata/pnfieldmetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7344 2021-08-22 09:38:16.000000 pineboo-1.0.4.2/pineboolib/application/metadata/pnrelationmetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    25771 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/metadata/pntablemetadata.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.905615 pineboo-1.0.4.2/pineboolib/application/metadata/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       36 2019-08-03 08:33:48.000000 pineboo-1.0.4.2/pineboolib/application/metadata/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1217 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/metadata/tests/test_pnaction.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2311 2020-02-05 09:39:18.000000 pineboo-1.0.4.2/pineboolib/application/metadata/tests/test_pncompoundkeymetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    16137 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/metadata/tests/test_pnfieldmetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4190 2021-08-23 10:27:07.000000 pineboo-1.0.4.2/pineboolib/application/metadata/tests/test_pnrelationmetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7444 2021-01-21 09:59:47.000000 pineboo-1.0.4.2/pineboolib/application/metadata/tests/test_pntablemetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2862 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/module.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4141 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/moduleactions.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       47 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/modules_tree.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.905615 pineboo-1.0.4.2/pineboolib/application/packager/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      122 2019-07-31 07:36:22.000000 pineboo-1.0.4.2/pineboolib/application/packager/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10703 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/packager/pnpackager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1947 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/packager/pnunpacker.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.905615 pineboo-1.0.4.2/pineboolib/application/packager/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-01-21 10:44:31.000000 pineboo-1.0.4.2/pineboolib/application/packager/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1763 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/packager/tests/test_pnpackager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1519 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/packager/tests/test_pnunpaker.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.905615 pineboo-1.0.4.2/pineboolib/application/parsers/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       70 2019-07-29 14:08:13.000000 pineboo-1.0.4.2/pineboolib/application/parsers/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.909615 pineboo-1.0.4.2/pineboolib/application/parsers/parser_kut/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       56 2020-04-23 09:34:52.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_kut/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    14822 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_kut/kparsertools.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    43978 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_kut/kut2fpdf.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.909615 pineboo-1.0.4.2/pineboolib/application/parsers/parser_kut/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      291 2020-04-23 09:34:52.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_kut/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10578 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_kut/tests/test_parser_kut.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.909615 pineboo-1.0.4.2/pineboolib/application/parsers/parser_mtd/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       50 2020-04-23 09:34:52.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_mtd/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    14324 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_mtd/pnmtdparser.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5406 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_mtd/pnormmodelsfactory.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.909615 pineboo-1.0.4.2/pineboolib/application/parsers/parser_mtd/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2020-04-23 09:34:52.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_mtd/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1885 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_mtd/tests/test_parser_mtd.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.909615 pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      167 2023-05-01 17:08:12.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      587 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/flex.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    31580 2023-04-28 10:51:35.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/flscriptparse.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3400 2020-04-23 09:34:52.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/lextab.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    28374 2023-05-01 17:43:29.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/postparse.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8675 2023-05-01 17:45:21.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/pyconvert.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    91788 2023-05-01 17:35:12.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/pytnyzer.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.909615 pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      502 2020-04-23 09:34:52.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    16732 2023-05-01 17:45:55.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/tests/test_parser_qsa.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6174 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/token_rules.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.909615 pineboo-1.0.4.2/pineboolib/application/parsers/parser_ui/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      101 2020-04-23 09:34:52.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_ui/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    49421 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_ui/qt3ui.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.909615 pineboo-1.0.4.2/pineboolib/application/parsers/parser_ui/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       33 2020-04-23 09:34:52.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_ui/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1627 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/parsers/parser_ui/tests/test_parser_ui.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    34668 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/pnapplication.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      371 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/pncore.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6753 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/process.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    27059 2023-05-01 18:12:46.000000 pineboo-1.0.4.2/pineboolib/application/projectmodule.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3641 2021-03-30 10:58:34.000000 pineboo-1.0.4.2/pineboolib/application/proxy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6876 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/qsadictmodules.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.909615 pineboo-1.0.4.2/pineboolib/application/qsatypes/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       28 2019-08-01 20:49:12.000000 pineboo-1.0.4.2/pineboolib/application/qsatypes/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7965 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/qsatypes/date.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    20095 2023-04-18 17:17:37.000000 pineboo-1.0.4.2/pineboolib/application/qsatypes/sysbasetype.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.909615 pineboo-1.0.4.2/pineboolib/application/qsatypes/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       36 2019-08-06 06:55:22.000000 pineboo-1.0.4.2/pineboolib/application/qsatypes/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1853 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/qsatypes/tests/test_date.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5455 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/qsatypes/tests/test_sysbasetype.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3461 2021-03-29 11:28:24.000000 pineboo-1.0.4.2/pineboolib/application/safeqsa.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.913615 pineboo-1.0.4.2/pineboolib/application/signatures/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       26 2020-12-25 17:46:05.000000 pineboo-1.0.4.2/pineboolib/application/signatures/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6312 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/signatures/pdf_digest.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8187 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/signatures/pdf_qr.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.913615 pineboo-1.0.4.2/pineboolib/application/signatures/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      286 2021-01-18 11:51:09.000000 pineboo-1.0.4.2/pineboolib/application/signatures/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3440 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/signatures/tests/test_signatures.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9298 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/signatures/xml_digest.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.913615 pineboo-1.0.4.2/pineboolib/application/staticloader/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       28 2019-10-04 20:53:14.000000 pineboo-1.0.4.2/pineboolib/application/staticloader/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    14695 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/staticloader/pnmodulesstaticloader.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.913615 pineboo-1.0.4.2/pineboolib/application/staticloader/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      289 2020-09-07 08:35:55.000000 pineboo-1.0.4.2/pineboolib/application/staticloader/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2491 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/staticloader/tests/test_static_loader.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.913615 pineboo-1.0.4.2/pineboolib/application/staticloader/ui/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2020-08-17 12:14:19.000000 pineboo-1.0.4.2/pineboolib/application/staticloader/ui/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7299 2020-03-10 09:40:23.000000 pineboo-1.0.4.2/pineboolib/application/staticloader/ui/static_loader.ui
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.913615 pineboo-1.0.4.2/pineboolib/application/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      287 2019-10-09 06:29:09.000000 pineboo-1.0.4.2/pineboolib/application/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1627 2020-06-10 19:38:58.000000 pineboo-1.0.4.2/pineboolib/application/tests/test_application.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1350 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/tests/test_load_script.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1309 2020-09-21 07:02:30.000000 pineboo-1.0.4.2/pineboolib/application/tests/test_process.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1259 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/tests/test_projectmodule.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      686 2020-09-04 08:27:19.000000 pineboo-1.0.4.2/pineboolib/application/tests/test_proxy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    16925 2023-04-07 15:43:24.000000 pineboo-1.0.4.2/pineboolib/application/tests/test_types.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1319 2020-09-07 08:35:55.000000 pineboo-1.0.4.2/pineboolib/application/tests/test_xmlaction.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.913615 pineboo-1.0.4.2/pineboolib/application/translator/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       26 2020-04-05 08:54:23.000000 pineboo-1.0.4.2/pineboolib/application/translator/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5405 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/translator/pntranslator.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.913615 pineboo-1.0.4.2/pineboolib/application/translator/test/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       34 2020-12-01 12:01:44.000000 pineboo-1.0.4.2/pineboolib/application/translator/test/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      802 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/translator/test/test_pntranslator.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    22047 2023-04-09 14:08:33.000000 pineboo-1.0.4.2/pineboolib/application/types.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.917615 pineboo-1.0.4.2/pineboolib/application/utils/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      182 2019-07-31 08:47:54.000000 pineboo-1.0.4.2/pineboolib/application/utils/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1548 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/utils/check_dependencies.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2245 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/utils/convert_flaction.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2430 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/utils/date_conversion.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6310 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/application/utils/flfiles_dir.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1120 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/utils/geometry.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1949 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/utils/mobilemode.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2258 2023-05-01 17:36:31.000000 pineboo-1.0.4.2/pineboolib/application/utils/modules.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1626 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/utils/path.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4727 2020-11-25 10:48:38.000000 pineboo-1.0.4.2/pineboolib/application/utils/service.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    23037 2023-04-19 12:18:00.000000 pineboo-1.0.4.2/pineboolib/application/utils/sql_tools.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1307 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/utils/xpm.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15051 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/application/xmlaction.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.917615 pineboo-1.0.4.2/pineboolib/core/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      268 2021-03-29 11:28:24.000000 pineboo-1.0.4.2/pineboolib/core/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8761 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/core/decorators.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      746 2020-10-16 07:17:25.000000 pineboo-1.0.4.2/pineboolib/core/exceptions.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.917615 pineboo-1.0.4.2/pineboolib/core/fonts/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2019-09-17 09:33:15.000000 pineboo-1.0.4.2/pineboolib/core/fonts/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.917615 pineboo-1.0.4.2/pineboolib/core/fonts/noto_sans/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2020-03-09 09:55:39.000000 pineboo-1.0.4.2/pineboolib/core/fonts/noto_sans/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2578 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/core/garbage_collector.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.917615 pineboo-1.0.4.2/pineboolib/core/images/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-09-17 09:33:15.000000 pineboo-1.0.4.2/pineboolib/core/images/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.933616 pineboo-1.0.4.2/pineboolib/core/images/icono_pi/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      960 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Pi-symbol.svg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)  1464366 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi.psd
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)  9487782 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi2.xcf
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   476635 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi2_1024.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    50853 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi2_256.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   147180 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi2_512.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    50737 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi_1024.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15871 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi_256.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    29321 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi_512.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       25 2019-09-17 09:33:15.000000 pineboo-1.0.4.2/pineboolib/core/images/icono_pi/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.945616 pineboo-1.0.4.2/pineboolib/core/images/icons/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2019-09-17 09:33:15.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/__init__.py
+-rwxrwxr-x   0 aulla     (1000) aulla     (1000)      892 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/about.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1230 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/aboutqt.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      853 2019-10-01 07:14:24.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/cancel.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      571 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/consola.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      669 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/date.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2199 2019-09-30 08:28:48.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/delete.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2562 2019-10-01 07:14:24.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/down.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2069 2019-09-30 08:28:48.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/edit.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2237 2020-01-15 08:29:51.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/edit_file.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1657 2020-01-15 08:29:51.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/edit_file_xml.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      934 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/estilo.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      870 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/exit.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      464 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/flfielddb.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      691 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/fltable-clean.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      526 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/fltable-data.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      464 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/fltable-filter.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      727 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/fltable-odf.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      459 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/folder.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      615 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/folder_update.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      563 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/font.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1263 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/go-bottom.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1187 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/go-down.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/go-first.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1774 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/go-home.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/go-jump.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/go-last.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/go-next.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/go-previous.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1293 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/go-top.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1193 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/go-up.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      601 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-add.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1624 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-bold.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1927 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-cancel.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1682 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-clear.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      723 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-copy.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2087 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-cut.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2049 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-delete.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2104 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-find-and-replace.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1636 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-find.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1256 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-fullscreen.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-go-back-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-go-back-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1187 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-go-down.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1219 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-go-forward-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-go-forward-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1193 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-go-up.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1263 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-goto-bottom.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-goto-first-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-goto-first-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1342 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-goto-last-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1331 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-goto-last-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1293 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-goto-top.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1774 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-home.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      766 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-indent-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      767 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-indent-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1338 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-italic.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-jump-to-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1491 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-jump-to-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      526 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-justify-center.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      517 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-justify-fill.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      515 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-justify-left.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      541 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-justify-right.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1205 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-forward-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1074 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-forward-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1225 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-next-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1236 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-next-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      481 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-pause.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1028 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-play-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1236 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-previous-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1225 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-previous-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1266 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-record.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1074 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-rewind-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1205 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-rewind-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      571 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-stop.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1008 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-new.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1550 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-open.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1027 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-paste.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1719 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-print-preview.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1013 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-print.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1115 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-properties.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1502 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-redo-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-refresh.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      317 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-remove.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1837 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-save-as.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1971 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-save.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      631 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-select-all.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1927 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-stop.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1445 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-strikethrough.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1550 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-underline.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1601 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-undo-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      767 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-unindent-ltr.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      766 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-unindent-rtl.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      911 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/help_index.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1854 2019-09-30 08:28:48.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/insert.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      711 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/lock.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      579 2019-10-01 07:14:24.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/ok.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1997 2019-09-30 08:28:48.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/paste.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6800 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-128.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      857 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-16.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1406 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-24.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15871 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-256.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1941 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-32.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2991 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-48.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3482 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-57.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3243 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-64.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3641 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-72.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6800 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19949 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo-128.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1216 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo-16.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1720 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo-24.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    52103 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo-256.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2568 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo-32.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4552 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo-48.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7028 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo-64.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17588 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2019-09-30 08:28:48.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/print.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      885 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/reload.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    22869 2022-07-06 21:01:18.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/signed_stamp.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1930 2019-10-02 12:19:59.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/sys_ebcomportamiento.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1571 2019-10-02 12:19:59.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flareas.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2952 2019-10-02 12:19:59.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/sys_fldumpdb.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1133 2019-10-02 12:19:59.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flgroups.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1871 2019-10-02 12:19:59.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flloadmod.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2404 2019-10-02 12:19:59.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flloadmodpkg.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1335 2019-10-02 12:19:59.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flmodules.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2010 2019-10-02 12:19:59.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flmrproper.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2334 2019-10-02 12:19:59.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flreinit.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2771 2019-10-02 12:19:59.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flreloadbatch.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1731 2019-10-02 12:19:59.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flreloadlast.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2194 2019-10-02 12:19:59.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flusers.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    35029 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/terminal.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      638 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/unlock.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2635 2019-10-01 07:14:24.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/up.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2325 2019-09-30 08:28:48.000000 pineboo-1.0.4.2/pineboolib/core/images/icons/zoom.png
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.949616 pineboo-1.0.4.2/pineboolib/core/images/splashscreen/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-09-17 09:33:15.000000 pineboo-1.0.4.2/pineboolib/core/images/splashscreen/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    72306 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/splashscreen/dbadmin240.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   187209 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/splashscreen/dbadmin480.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    71281 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/splashscreen/quick240.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   185547 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/splashscreen/quick480.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       52 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/splashscreen/readme
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    66162 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/splashscreen/splash.png
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   109093 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/core/images/splashscreen/splash.svg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1150 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/core/message_manager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4314 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/core/settings.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      426 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/core/system.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.949616 pineboo-1.0.4.2/pineboolib/core/test/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2020-09-21 07:02:47.000000 pineboo-1.0.4.2/pineboolib/core/test/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1215 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/core/test/test_settings.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      211 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/core/translate.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.949616 pineboo-1.0.4.2/pineboolib/core/utils/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      114 2019-07-28 13:56:09.000000 pineboo-1.0.4.2/pineboolib/core/utils/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3203 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/core/utils/check_dependencies.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3140 2020-03-10 08:41:03.000000 pineboo-1.0.4.2/pineboolib/core/utils/logging.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      540 2019-07-28 13:56:09.000000 pineboo-1.0.4.2/pineboolib/core/utils/singleton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3720 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/core/utils/struct.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.949616 pineboo-1.0.4.2/pineboolib/core/utils/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       46 2019-08-04 20:13:49.000000 pineboo-1.0.4.2/pineboolib/core/utils/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2331 2020-03-09 12:29:25.000000 pineboo-1.0.4.2/pineboolib/core/utils/tests/test_utils_base.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1819 2020-09-21 06:32:29.000000 pineboo-1.0.4.2/pineboolib/core/utils/tests/test_version.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15945 2023-04-19 12:18:00.000000 pineboo-1.0.4.2/pineboolib/core/utils/utils_base.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4686 2021-03-08 21:10:30.000000 pineboo-1.0.4.2/pineboolib/core/utils/version.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.953616 pineboo-1.0.4.2/pineboolib/fllegacy/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      111 2019-07-31 21:01:09.000000 pineboo-1.0.4.2/pineboolib/fllegacy/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.957616 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       77 2019-07-31 16:14:18.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      349 2019-11-28 09:34:37.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqboolflagstate.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      580 2020-11-10 11:32:00.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqformdb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      984 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqobjectquerylist.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13444 2022-07-05 09:51:12.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqods.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6753 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      521 2020-03-09 11:54:38.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqsbuttongroup.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      243 2019-07-31 20:16:08.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqsettings.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      337 2019-11-18 12:56:58.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqshttp.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      167 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqsignalmapper.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      241 2019-07-31 20:16:08.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqsmtpclient.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1531 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqsobjectfactory.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18185 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqsql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      273 2019-11-28 09:34:37.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqsqlcursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      255 2019-07-31 20:16:08.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqsqlquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      734 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqssproject.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      343 2020-09-14 10:30:41.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqutil.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.957616 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-08-29 15:57:47.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1300 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/tests/test_aqobjectquerylist.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1201 2020-12-01 12:01:57.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/tests/test_aqods.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1907 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/tests/test_aqs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      554 2020-04-21 15:32:44.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/tests/test_aqsbuttongroup.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1194 2020-08-07 17:51:40.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/tests/test_aqsql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      953 2020-02-11 09:11:31.000000 pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/tests/test_aqutil.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      358 2019-09-19 09:51:37.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flaction.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      171 2020-04-02 16:10:18.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flapplication.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      446 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flcheckbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    12411 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flcodbar.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    29167 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/fldatatable.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1657 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/fldateedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2319 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/fldoublevalidator.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1200 2020-08-24 08:14:25.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flfastcgi.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   143170 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flfielddb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    31497 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flformdb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    34481 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flformrecorddb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    14097 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flformsearchdb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      185 2019-08-01 06:59:07.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flgroupbyquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1361 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flintvalidator.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      161 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/fljasperengine.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      103 2020-08-19 14:34:59.000000 pineboo-1.0.4.2/pineboolib/fllegacy/fljasperviewer.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5497 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/fllineedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3892 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/fllistviewitem.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    52856 2023-04-19 12:33:57.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flmanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    28979 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flmanagermodules.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4403 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flnetwork.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      196 2019-08-17 07:43:18.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flparameterquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4300 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flpixmapview.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3702 2020-08-24 09:53:53.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flposprinter.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13824 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flreportengine.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    22476 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flreportviewer.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      403 2019-11-14 09:39:09.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flscripteditor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5273 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flserialport.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1620 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flsettings.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13515 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flsmtpclient.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      895 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flspinbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      267 2020-03-05 11:36:30.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flsqlconnections.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      167 2019-08-17 07:43:18.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flsqlcursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      161 2019-08-17 07:43:18.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flsqlquery.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      686 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/fltable.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)   108501 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/fltabledb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      875 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/fltimeedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1092 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/fluintvalidator.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    41598 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flutil.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1876 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flvar.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      549 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      315 2019-08-13 07:00:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/flworkspace.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.957616 pineboo-1.0.4.2/pineboolib/fllegacy/forms/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    48049 2020-12-24 07:51:30.000000 pineboo-1.0.4.2/pineboolib/fllegacy/forms/FLWidgetReportViewer.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       67 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/forms/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67146 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/systype.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.957616 pineboo-1.0.4.2/pineboolib/fllegacy/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2019-12-02 11:03:25.000000 pineboo-1.0.4.2/pineboolib/fllegacy/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1455 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flcodbar.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1664 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_fldatatable.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      991 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_fldateedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8825 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flfielddb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      939 2020-09-21 06:32:29.000000 pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flform.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2286 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flformrecorddb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3065 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flformsearch.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2289 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flmanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      902 2020-12-22 09:37:36.000000 pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flreportengine.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    12536 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_fltabledb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8666 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flutil.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1592 2020-09-01 07:21:14.000000 pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_settings.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1192 2020-09-01 07:21:14.000000 pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_smtp.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8560 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_systype.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.957616 pineboo-1.0.4.2/pineboolib/interfaces/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      331 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/interfaces/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      172 2019-07-31 18:05:01.000000 pineboo-1.0.4.2/pineboolib/interfaces/cursoraccessmode.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      228 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/interfaces/dgi_schema.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10886 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/interfaces/iconnection.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5925 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/interfaces/ifieldmetadata.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2999 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/interfaces/imainwindow.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5542 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/interfaces/imanager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/interfaces/isession.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    21668 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/interfaces/isqlcursor.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    50302 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/interfaces/isqldriver.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3292 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/interfaces/itablemetadata.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.957616 pineboo-1.0.4.2/pineboolib/loader/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       92 2019-08-04 07:50:46.000000 pineboo-1.0.4.2/pineboolib/loader/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2024 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/loader/connection.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1546 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/loader/dgi.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.961617 pineboo-1.0.4.2/pineboolib/loader/dlgconnect/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      104 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/loader/dlgconnect/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      716 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/loader/dlgconnect/conn_dialog.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15802 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/loader/dlgconnect/dlgconnect.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    24027 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/loader/dlgconnect/dlgconnect.ui
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.961617 pineboo-1.0.4.2/pineboolib/loader/dlgconnect/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       57 2020-12-02 18:09:30.000000 pineboo-1.0.4.2/pineboolib/loader/dlgconnect/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2544 2020-11-09 16:02:09.000000 pineboo-1.0.4.2/pineboolib/loader/dlgconnect/tests/test_dlgconnect.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2870 2023-04-20 16:01:15.000000 pineboo-1.0.4.2/pineboolib/loader/init_project.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18287 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/loader/main.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5772 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/loader/options.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1311 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/loader/preload.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17570 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/loader/projectconfig.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.961617 pineboo-1.0.4.2/pineboolib/loader/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      477 2019-08-05 15:23:25.000000 pineboo-1.0.4.2/pineboolib/loader/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2495 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/loader/tests/test_connection.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      827 2021-03-08 11:35:13.000000 pineboo-1.0.4.2/pineboolib/loader/tests/test_main.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4314 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/loader/tests/test_projectconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3682 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/loader/utils.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.961617 pineboo-1.0.4.2/pineboolib/plugins/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       23 2019-08-18 15:38:56.000000 pineboo-1.0.4.2/pineboolib/plugins/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.961617 pineboo-1.0.4.2/pineboolib/plugins/custom_widgets/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      282 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/custom_widgets/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      462 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/custom_widgets/flfielddb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      456 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/custom_widgets/fltable.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      462 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/custom_widgets/fltabledb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      456 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/custom_widgets/pncore.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.961617 pineboo-1.0.4.2/pineboolib/plugins/dgi/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       19 2019-08-18 15:38:56.000000 pineboo-1.0.4.2/pineboolib/plugins/dgi/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.961617 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_fcgi/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2019-08-18 15:38:56.000000 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_fcgi/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2848 2020-03-24 12:23:10.000000 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_fcgi/dgi_fcgi.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.961617 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-08-18 15:38:56.000000 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.961617 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       30 2019-08-18 15:38:56.000000 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.961617 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       25 2019-08-18 15:38:56.000000 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2014 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9496 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2190 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1452 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/splash_screen.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      604 2020-04-02 16:10:18.000000 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/status_help_msg.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4643 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_qt.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5507 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_schema.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.961617 pineboo-1.0.4.2/pineboolib/plugins/mainform/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      177 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/mainform/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.961617 pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       78 2019-07-30 09:20:57.000000 pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    55893 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo/eneboo.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4184 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo/mainform.ui
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.961617 pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      276 2019-11-04 08:30:07.000000 pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5085 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo/tests/test_eneboo.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.961617 pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo_mdi/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       82 2019-07-30 09:20:57.000000 pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo_mdi/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    49501 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo_mdi/eneboo_mdi.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1500 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo_mdi/mainform.ui
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.961617 pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo_mdi/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      280 2019-11-04 08:30:07.000000 pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo_mdi/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3263 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo_mdi/tests/test_eneboo_mdi.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.965617 pineboo-1.0.4.2/pineboolib/plugins/sql/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       27 2019-08-18 13:55:56.000000 pineboo-1.0.4.2/pineboolib/plugins/sql/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      483 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/sql/flmysql_innodb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    12024 2023-04-19 12:33:54.000000 pineboo-1.0.4.2/pineboolib/plugins/sql/flmysql_myisam.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11877 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/plugins/sql/flpymssql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      825 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/sql/flpyodbc.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13367 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/sql/flqpsql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11393 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/plugins/sql/flsqlite.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.965617 pineboo-1.0.4.2/pineboolib/plugins/sql/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       31 2020-09-17 10:11:16.000000 pineboo-1.0.4.2/pineboolib/plugins/sql/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2172 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/sql/tests/test_flmysql_innodb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2958 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/sql/tests/test_flmysql_myisam.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2861 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/sql/tests/test_flpymssql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2087 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/sql/tests/test_flpyodbc.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4517 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/sql/tests/test_flsqlite.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2095 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/sql/tests/test_qpsql.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9177 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/plugins/sql/tests/test_stress.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2019-07-27 10:21:43.000000 pineboo-1.0.4.2/pineboolib/py.typed
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.969617 pineboo-1.0.4.2/pineboolib/q3widgets/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       94 2019-09-27 15:43:59.000000 pineboo-1.0.4.2/pineboolib/q3widgets/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1761 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/checkbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      142 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/combobox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1398 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/dateedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3877 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/dialog.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1634 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/filedialog.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      482 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/groupbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      118 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/line.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1061 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/lineedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3570 2023-04-28 10:51:28.000000 pineboo-1.0.4.2/pineboolib/q3widgets/messagebox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2758 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/numberedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      443 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/picture.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      134 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/pixmap.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1109 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qaction.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      887 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qbuttongroup.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1541 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qbytearray.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      774 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qcheckbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2176 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qcombobox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      138 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qdataview.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2262 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qdateedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      147 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qdatetime.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1663 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qdialog.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      237 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qdir.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      316 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qeventloop.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1138 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qframe.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3328 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qgroupbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      656 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qhboxlayout.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      348 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qhbuttongroup.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17321 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qhttp.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      231 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qiconset.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2061 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qlabel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      144 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qlayoutwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1099 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qline.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1767 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qlineedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5684 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qlistview.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      173 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qlistviewwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      445 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qmainwindow.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      137 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qmenu.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      153 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qmessagebox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1668 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qobject.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      153 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qpopupmenu.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3111 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qpushbutton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1975 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qradiobutton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      149 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qspinbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    12608 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qtable.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1741 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qtabwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2013 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qtextedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      463 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qtextstream.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      926 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qtimeedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      404 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qtoolbar.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2255 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qtoolbutton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      654 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qvboxlayout.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      348 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qvbuttongroup.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1231 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/qwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      184 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/radiobutton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      128 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/rect.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      128 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/size.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1731 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/spinbox.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.973617 pineboo-1.0.4.2/pineboolib/q3widgets/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      278 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      470 2019-12-19 10:11:59.000000 pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_dateedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1411 2020-12-02 18:08:18.000000 pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_messagebox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      646 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_qbytearray.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2638 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_qhttp.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      719 2019-09-27 15:43:59.000000 pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_qpushbutton.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1163 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_qradiobuttons.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1131 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_qtabwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1046 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_qtextstream.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      532 2020-09-21 08:32:33.000000 pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_spinbox.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/textedit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      141 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/q3widgets/timeedit.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.973617 pineboo-1.0.4.2/pineboolib/qsa/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       95 2019-08-02 07:28:39.000000 pineboo-1.0.4.2/pineboolib/qsa/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     5934 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/qsa/decorators.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1321 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/qsa/emptyscript.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7457 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/qsa/formdbwidget.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2035 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/qsa/input.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1439 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/qsa/object_class.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11935 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/qsa/pncontrolsfactory.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8336 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/qsa/qsa.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.973617 pineboo-1.0.4.2/pineboolib/qsa/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      496 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/qsa/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      744 2020-06-22 11:35:54.000000 pineboo-1.0.4.2/pineboolib/qsa/tests/test_class.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4169 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/qsa/tests/test_classes.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    17795 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/qsa/tests/test_knownbugs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6680 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/qsa/tests/test_orm.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1563 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/qsa/tests/test_query_values.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1716 2023-05-01 17:35:40.000000 pineboo-1.0.4.2/pineboolib/qsa/tests/test_require.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7893 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/qsa/tests/test_utils.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    20373 2023-05-01 17:39:28.000000 pineboo-1.0.4.2/pineboolib/qsa/utils.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.973617 pineboo-1.0.4.2/pineboolib/system_module/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       29 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/system_module/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.977617 pineboo-1.0.4.2/pineboolib/system_module/forms/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9153 2019-09-30 08:28:05.000000 pineboo-1.0.4.2/pineboolib/system_module/forms/FLWidgetMasterTable.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-09-17 09:33:15.000000 pineboo-1.0.4.2/pineboolib/system_module/forms/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    28933 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/forms/ebcomportamiento.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1368 2019-10-01 07:14:24.000000 pineboo-1.0.4.2/pineboolib/system_module/forms/flareas.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2994 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/forms/flfiles.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8007 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/forms/flgroups.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    16760 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/forms/flmodulos.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3150 2020-07-06 10:29:58.000000 pineboo-1.0.4.2/pineboolib/system_module/forms/fltest.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1214 2019-10-01 07:14:24.000000 pineboo-1.0.4.2/pineboolib/system_module/forms/flusers.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8877 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/forms/master.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10189 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/forms/master_copy.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9932 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/forms/master_print.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11619 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/forms/master_print_copy.ui
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    11760 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/forms/sys.ui
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.977617 pineboo-1.0.4.2/pineboolib/system_module/models/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2020-04-27 09:01:43.000000 pineboo-1.0.4.2/pineboolib/system_module/models/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1441 2020-07-16 10:23:10.000000 pineboo-1.0.4.2/pineboolib/system_module/models/flareas_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3270 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/system_module/models/flfiles_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1238 2020-07-16 10:23:10.000000 pineboo-1.0.4.2/pineboolib/system_module/models/flgroups_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1192 2020-07-16 10:23:10.000000 pineboo-1.0.4.2/pineboolib/system_module/models/fllarge_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1313 2020-07-16 10:23:10.000000 pineboo-1.0.4.2/pineboolib/system_module/models/flmetadata_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3296 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/models/flmodules_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1292 2020-07-16 10:23:10.000000 pineboo-1.0.4.2/pineboolib/system_module/models/flseqs_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1007 2020-07-16 10:23:10.000000 pineboo-1.0.4.2/pineboolib/system_module/models/flserial_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1023 2020-07-16 10:23:10.000000 pineboo-1.0.4.2/pineboolib/system_module/models/flsettings_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2369 2020-07-16 10:23:10.000000 pineboo-1.0.4.2/pineboolib/system_module/models/fltest2_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1769 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/models/fltest3_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1859 2020-07-16 10:23:10.000000 pineboo-1.0.4.2/pineboolib/system_module/models/fltest4_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2296 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/models/fltest5_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2659 2020-10-13 15:24:00.000000 pineboo-1.0.4.2/pineboolib/system_module/models/fltest_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3548 2020-07-16 10:23:10.000000 pineboo-1.0.4.2/pineboolib/system_module/models/flupdates_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1450 2020-07-16 10:23:10.000000 pineboo-1.0.4.2/pineboolib/system_module/models/flusers_model.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1718 2020-07-16 10:23:10.000000 pineboo-1.0.4.2/pineboolib/system_module/models/flvar_model.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.977617 pineboo-1.0.4.2/pineboolib/system_module/queries/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       24 2019-09-17 09:33:15.000000 pineboo-1.0.4.2/pineboolib/system_module/queries/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      636 2020-10-15 10:53:48.000000 pineboo-1.0.4.2/pineboolib/system_module/queries/fltest2.qry
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.981617 pineboo-1.0.4.2/pineboolib/system_module/scripts/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       22 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15186 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/ebcomportamiento.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      234 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/fldumpdb.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      859 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/flfiles.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2430 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/flloadmod.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      246 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/flloadmodpkg.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      427 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/flmasterareas.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18788 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/flmodules.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      243 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/flmrproper.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      238 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/flreinit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3958 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/flreloadbatch.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6038 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/flreloadlast.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      138 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/fltest6.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4351 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/sys.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.981617 pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      277 2020-03-26 18:29:13.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1104 2020-09-17 09:48:31.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_ebcomportamiento.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2155 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_flfiles.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      646 2020-09-09 10:25:36.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_flloadmodpkg.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4238 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_flmodules.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      843 2020-09-09 10:25:36.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_flmrproper.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      851 2020-09-09 10:25:36.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_flreinit.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4322 2023-04-30 07:29:58.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_reload_last.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1564 2019-09-26 11:40:44.000000 pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_sys.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2411 2020-12-05 19:13:31.000000 pineboo-1.0.4.2/pineboolib/system_module/sys.xml
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6505 2019-08-23 10:35:06.000000 pineboo-1.0.4.2/pineboolib/system_module/sys.xpm
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.981617 pineboo-1.0.4.2/pineboolib/system_module/translations/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       29 2019-09-17 09:33:15.000000 pineboo-1.0.4.2/pineboolib/system_module/translations/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-01 18:17:26.000000 pineboo-1.0.4.2/pineboolib/system_module/translations/sys.ca.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-01 18:17:28.000000 pineboo-1.0.4.2/pineboolib/system_module/translations/sys.de.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-01 18:17:24.000000 pineboo-1.0.4.2/pineboolib/system_module/translations/sys.en.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    68138 2023-05-01 18:17:23.000000 pineboo-1.0.4.2/pineboolib/system_module/translations/sys.es.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-01 18:17:29.000000 pineboo-1.0.4.2/pineboolib/system_module/translations/sys.fr.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-01 18:17:31.000000 pineboo-1.0.4.2/pineboolib/system_module/translations/sys.gl.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-01 18:17:32.000000 pineboo-1.0.4.2/pineboolib/system_module/translations/sys.it.ts
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    67946 2023-05-01 18:17:34.000000 pineboo-1.0.4.2/pineboolib/system_module/translations/sys.pt.ts
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-05-01 18:17:34.985617 pineboo-1.0.4.2/pymodules/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2020-11-25 08:02:11.000000 pineboo-1.0.4.2/pymodules/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      283 2023-05-01 18:17:34.985617 pineboo-1.0.4.2/setup.cfg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4086 2023-04-04 09:45:24.000000 pineboo-1.0.4.2/setup.py
```

### Comparing `pineboo-1.0.4.1/LICENSE.mit` & `pineboo-1.0.4.2/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/PKG-INFO` & `pineboo-1.0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pineboo
-Version: 1.0.4.1
+Version: 1.0.4.2
 Summary: ERP replacement for Eneboo written in Python
 Home-page: https://github.com/deavid/pineboo
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo accounting sales warehouse
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pineboo-1.0.4.1/README.rst` & `pineboo-1.0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboo.egg-info/PKG-INFO` & `pineboo-1.0.4.2/pineboo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pineboo
-Version: 1.0.4.1
+Version: 1.0.4.2
 Summary: ERP replacement for Eneboo written in Python
 Home-page: https://github.com/deavid/pineboo
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
 Keywords: erp pineboo eneboo accounting sales warehouse
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pineboo-1.0.4.1/pineboo.egg-info/SOURCES.txt` & `pineboo-1.0.4.2/pineboo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboo.egg-info/requires.txt` & `pineboo-1.0.4.2/pineboo.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/__init__.py` & `pineboo-1.0.4.2/pineboolib/application/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 PROJECT = Project()
 
 SERIALIZE_LIST: Dict[int, List[str]] = {}
 FILE_CLASSES: Dict[str, str] = {}
 ID_SESSION: str = ""
 
-PINEBOO_VER = "1.0.4.1"
+PINEBOO_VER = "1.0.4.2"
 
 SHOW_CURSOR_EVENTS: bool = False  # Enable show pnsqlcursor actions debug.
 SHOW_CONNECTION_EVENTS: bool = False  # Enable show debug when connection is closed.
 SHOW_NESTED_WARNING: bool = False  # Enable show nested debug.
 VIRTUAL_DB: bool = True  # Enable :memory: database on pytest.
 LOG_SQL: bool = False  # Enable sqlalchemy logs.
 USE_WEBSOCKET_CHANNEL: bool = False  # Enable websockets features.
```

### Comparing `pineboo-1.0.4.1/pineboolib/application/acls/pnaccesscontrol.py` & `pineboo-1.0.4.2/pineboolib/application/acls/pnaccesscontrol.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/acls/pnaccesscontrolfactory.py` & `pineboo-1.0.4.2/pineboolib/application/acls/pnaccesscontrolfactory.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/acls/pnaccesscontrollists.py` & `pineboo-1.0.4.2/pineboolib/application/acls/pnaccesscontrollists.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/acls/pnboolflagstate.py` & `pineboo-1.0.4.2/pineboolib/application/acls/pnboolflagstate.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/acls/tests/test_acls.py` & `pineboo-1.0.4.2/pineboolib/application/acls/tests/test_acls.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/acls/tests/test_pnaccesscontrol.py` & `pineboo-1.0.4.2/pineboolib/application/acls/tests/test_pnaccesscontrol.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/connections.py` & `pineboo-1.0.4.2/pineboolib/application/connections.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/alembic_tools.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/alembic_tools.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/basemodel.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/basemodel.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/dummy_cursor.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/dummy_cursor.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/dummy_signal.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/dummy_signal.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_basemodel.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_basemodel.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_bytearray.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_bytearray.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_consistency.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_consistency.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_dummycursor.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_dummycursor.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_query_orm.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_query_orm.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_relationships.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_relationships.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_sessions.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_signals.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_thread_session.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_thread_session.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_utils.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/tests/test_view.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/orm/utils.py` & `pineboo-1.0.4.2/pineboolib/application/database/orm/utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/pnbuffer.py` & `pineboo-1.0.4.2/pineboolib/application/database/pnbuffer.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/pnconnection.py` & `pineboo-1.0.4.2/pineboolib/application/database/pnconnection.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/pnconnectionmanager.py` & `pineboo-1.0.4.2/pineboolib/application/database/pnconnectionmanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/pncursortablemodel.py` & `pineboo-1.0.4.2/pineboolib/application/database/pncursortablemodel.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/pngroupbyquery.py` & `pineboo-1.0.4.2/pineboolib/application/database/pngroupbyquery.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/pnparameterquery.py` & `pineboo-1.0.4.2/pineboolib/application/database/pnparameterquery.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/pnsignals.py` & `pineboo-1.0.4.2/pineboolib/application/database/pnsignals.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/pnsqlcursor.py` & `pineboo-1.0.4.2/pineboolib/application/database/pnsqlcursor.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/pnsqldriversmanager.py` & `pineboo-1.0.4.2/pineboolib/application/database/pnsqldriversmanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/pnsqlquery.py` & `pineboo-1.0.4.2/pineboolib/application/database/pnsqlquery.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/tests/test_pnbuffer.py` & `pineboo-1.0.4.2/pineboolib/application/database/tests/test_pnbuffer.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/tests/test_pnconnection.py` & `pineboo-1.0.4.2/pineboolib/application/database/tests/test_pnconnection.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/tests/test_pnconnection_manager.py` & `pineboo-1.0.4.2/pineboolib/application/database/tests/test_pnconnection_manager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/tests/test_pncursortablemodel.py` & `pineboo-1.0.4.2/pineboolib/application/database/tests/test_pncursortablemodel.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/tests/test_pnparameterquery.py` & `pineboo-1.0.4.2/pineboolib/application/database/tests/test_pnparameterquery.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/tests/test_pnsqlcursor.py` & `pineboo-1.0.4.2/pineboolib/application/database/tests/test_pnsqlcursor.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/tests/test_pnsqldriversmanager.py` & `pineboo-1.0.4.2/pineboolib/application/database/tests/test_pnsqldriversmanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/tests/test_pnsqlquery.py` & `pineboo-1.0.4.2/pineboolib/application/database/tests/test_pnsqlquery.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/tests/test_utils.py` & `pineboo-1.0.4.2/pineboolib/application/database/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/database/utils.py` & `pineboo-1.0.4.2/pineboolib/application/database/utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/file.py` & `pineboo-1.0.4.2/pineboolib/application/file.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/load_script.py` & `pineboo-1.0.4.2/pineboolib/application/load_script.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/metadata/pnaction.py` & `pineboo-1.0.4.2/pineboolib/application/metadata/pnaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/metadata/pncompoundkeymetadata.py` & `pineboo-1.0.4.2/pineboolib/application/metadata/pncompoundkeymetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/metadata/pnfieldmetadata.py` & `pineboo-1.0.4.2/pineboolib/application/metadata/pnfieldmetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/metadata/pnrelationmetadata.py` & `pineboo-1.0.4.2/pineboolib/application/metadata/pnrelationmetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/metadata/pntablemetadata.py` & `pineboo-1.0.4.2/pineboolib/application/metadata/pntablemetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/metadata/tests/test_pnaction.py` & `pineboo-1.0.4.2/pineboolib/application/metadata/tests/test_pnaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/metadata/tests/test_pncompoundkeymetadata.py` & `pineboo-1.0.4.2/pineboolib/application/metadata/tests/test_pncompoundkeymetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/metadata/tests/test_pnfieldmetadata.py` & `pineboo-1.0.4.2/pineboolib/application/metadata/tests/test_pnfieldmetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/metadata/tests/test_pnrelationmetadata.py` & `pineboo-1.0.4.2/pineboolib/application/metadata/tests/test_pnrelationmetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/metadata/tests/test_pntablemetadata.py` & `pineboo-1.0.4.2/pineboolib/application/metadata/tests/test_pntablemetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/module.py` & `pineboo-1.0.4.2/pineboolib/application/module.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/moduleactions.py` & `pineboo-1.0.4.2/pineboolib/application/moduleactions.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/packager/pnpackager.py` & `pineboo-1.0.4.2/pineboolib/application/packager/pnpackager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/packager/pnunpacker.py` & `pineboo-1.0.4.2/pineboolib/application/packager/pnunpacker.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/packager/tests/test_pnpackager.py` & `pineboo-1.0.4.2/pineboolib/application/packager/tests/test_pnpackager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/packager/tests/test_pnunpaker.py` & `pineboo-1.0.4.2/pineboolib/application/packager/tests/test_pnunpaker.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_kut/kparsertools.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_kut/kparsertools.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_kut/kut2fpdf.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_kut/kut2fpdf.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_kut/tests/test_parser_kut.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_kut/tests/test_parser_kut.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_mtd/pnmtdparser.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_mtd/pnmtdparser.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_mtd/pnormmodelsfactory.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_mtd/pnormmodelsfactory.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_mtd/tests/test_parser_mtd.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_mtd/tests/test_parser_mtd.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/flex.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/flex.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/flscriptparse.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/flscriptparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,14 +224,15 @@
             | funccall
             | error
 
     identifier : ID
 
     dictobject_value : LBRACE RBRACE
                      | LBRACE dictobject_value_elemlist RBRACE
+                     | LBRACE dictobject_value_elemlist COMMA RBRACE
 
     dictobject_value_elemlist : dictobject_value_elem
                               | dictobject_value_elemlist COMMA dictobject_value_elem
 
     dictobject_value_elem : exprval COLON expression
 
     base_expression     : ternary_operator
@@ -855,15 +856,14 @@
     INPUT_DATA = data
     flex.lexer.lineno = 1
     ERROR_COUNT = 0
     parser_ = parser.parse(data, debug=0, tracking=1, tokenfunc=my_tokenfunc)
     if ERROR_COUNT > 0:
         print("ERRORS (%d)" % ERROR_COUNT)
     if parser_ is not None:
-
         try:
             parser_["error_count"] = ERROR_COUNT
         except Exception as error:
             print(error)
             return None
 
         if parser.error:
@@ -954,15 +954,14 @@
                 sys.stderr.write(" formatting ...")
                 sys.stderr.flush()
                 do_it()
                 sys.stderr.write(" Done.\n")
                 sys.stderr.flush()
 
     else:
-
         line = ""
         while 1:
             try:
                 line1 = input("flscript> ")
                 if line1.startswith("#"):
                     comm = line1[1:].split(" ")
                     if comm[0] == "setstart":
```

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/lextab.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/lextab.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/postparse.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/postparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 #!/usr/bin/python3
 """
 Simplify AST-XML structures for later generation of Python files.
 """
-from importlib.machinery import ModuleSpec
+from importlib import machinery, util
 from optparse import OptionParser
 import os
 import sys
-import importlib
+
 from xml.etree import ElementTree as ET
 from xml.dom import minidom  # type: ignore
 from pineboolib import logging
 from pineboolib.application.parsers.parser_qsa import pytnyzer, flscriptparse
+from pineboolib.application.parsers import parser_qsa
 from typing import List, Type, Optional, Dict, Tuple, Any, Callable, cast, Iterable
 
 
-STRICT_MODE = pytnyzer.STRICT_MODE
-importlib.reload(pytnyzer)
-pytnyzer.STRICT_MODE = STRICT_MODE
-
 TreeData = Dict[str, Any]
 
 LOGGER = logging.get_logger(__name__)
 
 USEFUL_TOKENS = "ID,ICONST,FCONST,SCONST,CCONST,RXCONST,STATIC".split(",")
 
 KNOWN_PARSERS: Dict[str, Type["TagObjectBase"]] = {}
@@ -716,19 +713,19 @@
         """Create Module."""
         self.name = name
         self.path = path
 
     def loadModule(self):
         """Import and return Python file."""
         try:
-            from importlib import util
-
             module_name = self.name[: self.name.find(".")]
             script_name = os.path.join(self.path, self.name)
-            spec: Optional["ModuleSpec"] = util.spec_from_file_location(module_name, script_name)
+            spec: Optional["machinery.ModuleSpec"] = util.spec_from_file_location(
+                module_name, script_name
+            )
             if spec and spec.loader is not None:
                 module = util.module_from_spec(spec)
                 spec.loader.exec_module(module)  # type: ignore [attr-defined]
                 self.module = module
             else:
                 raise Exception(
                     "Module named %s can't be loaded from %s" % (module_name, script_name)
@@ -793,15 +790,15 @@
     )
 
     parser.add_option(
         "--toxml", action="store_true", dest="toxml", default=False, help="write xml file from qs"
     )
 
     parser.add_option(
-        "--full", action="store_true", dest="full", default=False, help="write xml file from qs"
+        "--full", action="store_true", dest="full", default=False, help="write py file from qs"
     )
 
     parser.add_option(
         "--cache",
         action="store_true",
         dest="cache",
         default=False,
@@ -825,15 +822,15 @@
 
     (options, args) = parser.parse_args(argv)
     return (options, args)
 
 
 def main() -> None:
     """Run the program from command line."""
-    pytnyzer.STRICT_MODE = True
+
     log_format = "%(asctime)s - %(levelname)s: %(name)s: %(message)s"
     logging.basicConfig(format=log_format, level=0)
     blib_logger = logging.get_logger("blib2to3.pgen2.driver")
     blib_logger.setLevel(logging.WARNING)
 
     options, args = parse_args(sys.argv[1:])
     execute(options, args)
@@ -883,15 +880,15 @@
     tree_data: TreeData = flscriptparse.calctree(prog, alias_mode=0)
     return post_parse(tree_data)
 
 
 def execute(options: Any, args: List[str]) -> None:
     """Execute conversion orders given by options and args. Can be used to emulate program calls."""
 
-    pytnyzer.STRICT_MODE = options.strict
+    parser_qsa.STRICT_MODE = options.strict
 
     if options.full:
         execpython = options.exec_python
         options.exec_python = False
         options.full = False
         options.toxml = True
         LOGGER.info("Pass 1 - Parse and write XML file . . .")
```

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/pyconvert.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/pyconvert.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 import codecs
 
 import multiprocessing
 from typing import List, Tuple, TypeVar, cast, Dict, Optional
 from xml import etree
 from pineboolib import logging
 from pineboolib.core.utils import struct
-from pineboolib.application.parsers.parser_qsa import postparse, pytnyzer, USE_THREADS
+from pineboolib.application.parsers import parser_qsa
+from pineboolib.application.parsers.parser_qsa import postparse
+
 
 LOGGER = logging.get_logger(__name__)
 
 
 class Action(struct.ActionStruct):
     """Represent actions from XML."""
 
@@ -104,15 +106,15 @@
         self.number = number
         self.len = len
         self.known = known
 
 
 def pythonify_item(item: PythonifyItem) -> bool:
     """Parse QS into Python. For multiprocessing.map."""
-    if USE_THREADS:
+    if parser_qsa.USE_THREADS:
         LOGGER.info("(%.2f%%) Parsing QS %r", 100 * item.number / item.len, item.src_path)
     try:
         pycode = postparse.pythonify2(item.src_path, known_refs=item.known)
     except Exception:
         LOGGER.exception("El fichero %s no se ha podido convertir", item.src_path)
         return False
 
@@ -128,15 +130,14 @@
 
 
 def main() -> None:
     """Get options and start conversion."""
     filter_mod = sys.argv[1] if len(sys.argv) > 1 else None
     filter_file = sys.argv[2] if len(sys.argv) > 2 else None
 
-    pytnyzer.STRICT_MODE = False
     log_format = "%(levelname)s: %(name)s: %(message)s"
     logging.basicConfig(format=log_format, level=0)
     blib_logger = logging.get_logger("blib2to3.pgen2.driver")
     blib_logger.setLevel(logging.WARNING)
     LOGGER.info("Cpu count %d", CPU_COUNT)
     source_folder = "."
     package_name = "pymodules"
@@ -225,15 +226,15 @@
     itemlist = [
         PythonifyItem(src=src, dst=dst, number=number, len=len(qs_files), known=known_modules)
         for number, (src, dst) in enumerate(qs_files)
     ]
 
     pycode_list: List[bool] = []
 
-    if USE_THREADS:
+    if parser_qsa.USE_THREADS:
         with multiprocessing.Pool(CPU_COUNT) as cpu:
             # TODO: Add proper signatures to Python files to avoid reparsing
             pycode_list = cpu.map(pythonify_item, itemlist, chunksize=2)
     else:
         for item in itemlist:
             pycode_list.append(pythonify_item(item))
```

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/pytnyzer.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/pytnyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,31 +8,29 @@
 import copy
 import optparse
 import os
 import pathlib
 import re
 from xml.etree import ElementTree as ET
 from typing import Any, Generator, Tuple, Type, List, Dict, Set, cast, Optional, TextIO, Callable
-
 from pineboolib.core.utils import logging
+from pineboolib.application.parsers import parser_qsa
+
 
 LOGGER = logging.get_logger(__name__)
 ASTGenerator = Generator[Tuple[str, str], None, None]
 
 try:
     import black  # type: ignore
 
     BLACK_FILEMODE = black.FileMode(line_length=120)
 except ImportError:
     black = None  # type: ignore [assignment]
     BLACK_FILEMODE = None  # type: ignore [assignment]
 
-
-STRICT_MODE = False
-
 # To get the following list updated, do:
 # In [1]: from pineboolib.qsa import qsa
 # In [2]: dir(qsa)
 
 QSA_KNOWN_ATTRS = {
     "Application",
     "AQBoolFlagState",
@@ -348,31 +346,29 @@
         name = "arg"
     # if name == "Process":
     #    name = "qsatype.Process"
 
     name = "%s_" % name if name in PYTHON_KEYWORDS else name
 
     if qsa_exclude is not None:
-
         if orig_name in qsa_exclude:
             return name
 
         if orig_name in QSA_KNOWN_ATTRS:
             if name in DISALLOW_CONVERSION_FOR_NONSTRICT:
                 return "self.module_%s" % name if name in ["connect", "disconnect"] else name
             else:
                 return "qsa.%s" % name
 
         if transform and name in transform:
             return transform[name]
 
         if name.startswith("form") and len(name) > 4:
             return 'qsa.from_project("%s")' % name
-
-        return "__undef__%s" % (name) if STRICT_MODE else name
+        return "%s%s" % ("__undef__" if parser_qsa.STRICT_MODE else "", name)
     else:
         return transform[name] if transform and name in transform else name
 
 
 CONT_SWITCH = 0
 CONT_DO_WHILE = 0
 
@@ -648,15 +644,14 @@
                     yield dtype, data
             if not expr:
                 arguments.append("unknownarg")
                 yield "debug", "Argument %d not understood" % number
                 yield "debug", ET.tostring(arg)  # type: ignore
             else:
                 if len(expr) == 1:
-
                     dtype_: Optional[str] = arg.get("type")
                     dtyping_ = ""
                     if dtype_ is not None:
                         if dtype_ == "String":
                             dtyping_ = "str"
                         elif dtype_ == "Number":
                             pass
@@ -776,21 +771,18 @@
                 yield "debug", ET.tostring(arg)  # type: ignore
             else:
                 arg1 = " ".join(expr)
                 arg1 = arg1.replace("( ", "(")
                 arg1 = arg1.replace(" )", ")")
                 arguments.append(arg1)
 
-        comment = ""
-        if not STRICT_MODE and name.startswith("__undef__"):
-            name = name[9:]
-            name = "self.%s" % name
-            comment = ""
+        if not parser_qsa.STRICT_MODE and name.startswith("__undef__"):
+            name = "self.%s" % name[9:]
 
-        yield "expr", "%s(%s)%s" % (name, ", ".join(arguments), comment)
+        yield "expr", "%s(%s)" % (name, ", ".join(arguments))
 
 
 class FunctionAnonExec(FunctionCall):
     """Process FunctionAnonExec XML tags."""
 
     pass
 
@@ -823,15 +815,14 @@
                 yield type_, data_
 
             if not expr:
                 main_expr.append("False")
                 yield "debug", "Expression %d not understood" % number
                 yield "debug", ET.tostring(arg)  # type: ignore
             else:
-
                 if len(expr) == 3:
                     # FIXME: This works if the pattern is alone in the IF. But if it has AND/Or does not work
                     if expr[1] == "==":
                         if expr[2] == "True":
                             expr = [expr[0]]
                         elif expr[2] == "False":
                             expr = ["not", expr[0]]
@@ -1311,15 +1302,14 @@
                     expr += 1
                 yield dtype1, data
             if expr == 0:
                 yield "expr", "None"
 
         if force_value:
             if values == 0:
-
                 if dtype is None:
                     yield "expr", ": Any = None"
                 else:
                     if dtype == "String":
                         yield "expr", ': str = ""'
                     elif dtype == "Number":
                         yield "expr", " = 0"
@@ -1346,15 +1336,14 @@
         identifier = None
         for number, arg in enumerate(self.elem):
             arg.set("parent_", self.elem)  # type: ignore
             expr = []
             for dtype, data in parse_ast(arg, parent=self).generate(
                 isolate=False, is_member=(number == 0)
             ):
-
                 if dtype == "expr":
                     if not data:
                         raise ValueError(ET.tostring(arg))
                     elif data == "[]":
                         data = "qsa.Array()"
                     expr.append(data)
                 else:
@@ -1549,15 +1538,15 @@
                 yield "debug", "Argument %d not understood" % number
                 yield "debug", ET.tostring(arg)  # type: ignore
             else:
                 txtarg = " ".join(expr)
             arguments.append(txtarg)
             arg_expr.append(expr)
 
-        if not STRICT_MODE:
+        if not parser_qsa.STRICT_MODE:
             arguments[0] = arguments[0].replace("__undef__", "")
 
         # Deteccion de llamada a modulo externo
         if (
             len(arguments) >= 2
             and arguments[1] == "iface"
             and arguments[0] != "self"
@@ -1732,15 +1721,14 @@
                         str_value = "str(" + value + ")"
                         if new_part_1.find(str_value) > -1:
                             arguments = [new_part_1]
                         else:
                             new_part_2 = ""
                             if len(part2) > 0:
                                 for i in range(len(part2)):
-
                                     part2[i] = str(part2[i]).replace("arg(", "str(")
                                 new_part_2 = ", " + ", ".join(part2)
                             new_part_1 = re.sub(r"%\d", "%s", new_part_1)
                             arguments = [
                                 "%s %% (str(%s" % (new_part_1, value + ")" + new_part_2 + ")")
                             ]
                     elif member == "join":
@@ -2362,15 +2350,14 @@
                 if dtype == "expr":
                     if data is None:
                         raise ValueError(ET.tostring(var))
                     expr.append(data)
                 else:
                     yield dtype, data
             if is_constructor:
-
                 if expr[0] in list(self.source.locals):
                     if expr[0] not in ["form", "iface"]:
                         # LOGGER.warning("Pasando de %s", expr[0])
                         continue
 
                 expr[0] = "self." + expr[0]
                 # print(1, expr[0], self.elem.get("parent_").tag, self.source.locals)
@@ -2448,17 +2435,14 @@
     """Create a new file template."""
 
     from pineboolib.application import PINEBOO_VER
 
     yield "line", "# -*- coding: utf-8 -*-"
     yield "line", "# Translated with pineboolib %s" % PINEBOO_VER
     yield "line", "from typing import TYPE_CHECKING, Any, Union"
-
-    if not STRICT_MODE:
-        yield "line", "from pineboolib.qsa.qsa import *  # noqa: F403"
     yield "line", "from pineboolib.qsa import qsa"
     # yield "line", "from pineboolib.qsaglobals import *"
     for alias, (path, name) in import_refs.items():
         yield "line", "from %s import %s as %s" % (path, name, alias)
     yield "line", ""
     yield "line", "# /** @file */"
     yield "line", ""
@@ -2491,15 +2475,14 @@
                 def_iface = copy.deepcopy(child)
                 def_iface.set("definition", "1")
                 child.set("constructor", "1")
                 if not only_iface:
                     csource.append(child)
                 mainsource.insert(0, def_iface)
         else:
-
             mainsource.append(child)
 
     for dtype, data in parse_ast(sourceclasses).generate():
         yield dtype, data
 
     # yield "line", ""
     # yield "line", "if TYPE_CHECKING:"
```

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/tests/test_parser_qsa.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/tests/test_parser_qsa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """
 Test QS Snippets.
 """
 from PyQt6 import QtCore, QtWidgets  # type: ignore[import]
 
 import unittest
 from pineboolib.application.parsers.parser_qsa.postparse import pythonify_string as qs2py
-from pineboolib.application.parsers.parser_qsa import pytnyzer
+from pineboolib.application.parsers import parser_qsa
 from pineboolib.application.parsers.parser_qsa.tests import fixture_read, fixture_path
 from pineboolib.loader.main import init_testing, finish_testing
 
 from pineboolib.core.utils import utils_base
-from pineboolib.application.parsers import parser_qsa
-
 import os
 import shutil
 
 
 class TestParser(unittest.TestCase):
     """Test Parsing QS to PY."""
 
     @classmethod
     def setUpClass(cls) -> None:
         """Enable strict parsing."""
-        pytnyzer.STRICT_MODE = True
+
+        parser_qsa.STRICT_MODE = True
         init_testing()
 
     def test_basic(self) -> None:
         """Test basic stuff."""
 
         self.assertEqual(qs2py("x = 0"), "x = 0\n")
 
@@ -109,27 +108,28 @@
         with open(fixture_path("flfacturac.qs.python"), "w") as file_:
             file_.write(flfacturac_qs_py)
 
         self.assertEqual(flfacturac_qs_py, flfacturac_py)
 
     def test_lib_str(self) -> None:
         """Test conveting fixture lib_str."""
-        pytnyzer.STRICT_MODE = False
+
+        parser_qsa.STRICT_MODE = False
         self.maxDiff = None  # pylint: disable=invalid-name
         flfacturac_qs = fixture_read("lib_str.qs")
         flfacturac_py = fixture_read("lib_str.python")
         flfacturac_qs_py = qs2py(flfacturac_qs, parser_template="file_template")
 
         # Delete version translator tag.
         pos_ini = flfacturac_qs_py.find("# Translated with pineboolib ")
         pos_fin = flfacturac_qs_py[pos_ini:].find("\n")
         flfacturac_qs_py = flfacturac_qs_py.replace(
             flfacturac_qs_py[pos_ini : pos_ini + pos_fin + 1], ""
         )
-        pytnyzer.STRICT_MODE = True
+        parser_qsa.STRICT_MODE = True
         # Write onto git so we have an example.
         with open(fixture_path("lib_str.qs.python"), "w") as file_:
             file_.write(flfacturac_qs_py)
 
         self.assertEqual(flfacturac_qs_py, flfacturac_py)
 
     def test_form(self) -> None:
@@ -435,12 +435,25 @@
 
         # Delete version translator tag.
         pos_ini = require_qs_py.find("# Translated with pineboolib ")
         pos_fin = require_qs_py[pos_ini:].find("\n")
         require_qs_py = require_qs_py.replace(require_qs_py[pos_ini : pos_ini + pos_fin + 1], "")
         self.assertEqual(require_qs_py, require_py) """
 
+    def test_dict(self) -> None:
+        """Test dictionary."""
+
+        qsa = """const _i = this.iface;
+
+                const aDatosFactRect = {
+                "codalmacen" : _i.calcularCodAlmacenFacturaRect(cursor, facturaRect),
+                "regimeniva" : _i.calcularRegimenIvaFacturaRect(cursor, facturaRect),
+                "codagente" : _i.calcularCodAgenteFacturaRect(cursor, facturaRect),
+                }"""
+        require_qs_py = qs2py(qsa)
+        self.assertTrue(require_qs_py)
+
     @classmethod
     def tearDownClass(cls) -> None:
         """Ensure test clear all data."""
 
         finish_testing()
```

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_qsa/token_rules.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_qsa/token_rules.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_ui/qt3ui.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_ui/qt3ui.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/parsers/parser_ui/tests/test_parser_ui.py` & `pineboo-1.0.4.2/pineboolib/application/parsers/parser_ui/tests/test_parser_ui.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/pnapplication.py` & `pineboo-1.0.4.2/pineboolib/application/pnapplication.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/process.py` & `pineboo-1.0.4.2/pineboolib/application/process.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/projectmodule.py` & `pineboo-1.0.4.2/pineboolib/application/projectmodule.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,14 @@
                     path_med = os.path.join(*path_build)
                     if not os.path.exists(path_med):
                         os.mkdir(path_med)
             except Exception as error:
                 raise Exception("Error building cache folder (%s) : %s" % (path_build, error))
 
         if os.path.exists(db_cache_folder):
-
             if not os.path.exists(cache_version_file_path):
                 delete_cache = True
             else:
                 cache_ver = ""
                 try:
                     file_ver = open(cache_version_file_path, "r", encoding="UTF8")
                     cache_ver = file_ver.read()
@@ -293,15 +292,14 @@
                         cache_ver,
                         parser_qsa.PARSER_QSA_VERSION,
                     )
                 else:
                     LOGGER.warning("Deleting cache.")
 
         if delete_cache and os.path.exists(db_cache_folder):
-
             self.message_manager().send("splash", "showMessage", ["Borrando caché ..."])
             LOGGER.info("DEVELOP: delete_cache Activado\nBorrando %s", db_cache_folder)
 
             for root, dirs, files in os.walk(db_cache_folder, topdown=False):
                 for name in files:
                     if os.path.exists(os.path.join(root, name)):
                         os.remove(os.path.join(root, name))
@@ -381,15 +379,14 @@
                 object_context.iface, function_name  # type: ignore [union-attr]
             ):
                 object_context = object_context.iface  # type: ignore [union-attr]
 
         function_object = getattr(object_context, function_name, None)
         if function_object is not None:
             try:
-
                 # Controlar numero de argumentos
                 args_num = connections.get_expected_args_num(function_object)
                 while args_num > len(args):
                     args.append(None)
 
                 if args and args_num:
                     args = args[0:args_num]
@@ -437,25 +434,23 @@
                 return False
 
         return True
 
     def parse_script_list(self, path_list: List[str]) -> bool:
         """Convert QS scripts list into Python and stores it in the same folders."""
 
-        from pineboolib.application.parsers.parser_qsa import pytnyzer, pyconvert
+        from pineboolib.application.parsers.parser_qsa import pyconvert
 
         if not path_list:
             return True
 
         for file_path in path_list:
             if not os.path.isfile(file_path):
                 raise IOError
 
-        pytnyzer.STRICT_MODE = True
-
         itemlist = []
         size_list = len(path_list)
         for num, orig_file_name in enumerate(path_list):
             dest_file_name = "%s.py" % orig_file_name[:-3]
             if dest_file_name in self.pending_conversion_list:
                 LOGGER.warning("The file %s is already being converted. Waiting", dest_file_name)
                 while dest_file_name in self.pending_conversion_list:
@@ -536,15 +531,14 @@
         file_object.close()
 
         del file_object
 
         self.modules["sys"] = module.Module("sys", "sys", "Administración", icono, "1.0")
         for root, dirs, files in os.walk(utils_base.filedir(base_dir, "system_module")):
             for nombre in files:
-
                 if "tests" in root:
                     continue
 
                 if is_library and nombre.endswith("ui"):
                     continue
 
                 if nombre.endswith("__.py") or nombre.endswith(".src"):
@@ -572,15 +566,14 @@
             "flmetadata",
             "flsettings",
             "flupdates",
             "flmetadata",
             "flseqs",
             "flsettings",
         ):
-
             self.conn_manager.manager().createSystemTable(table)
 
         return True
 
     def load_database_modules(self) -> bool:
         """Load database modules."""
 
@@ -613,15 +606,14 @@
         else:
             result_modules = conn.execute_query(
                 """SELECT idarea, idmodulo, descripcion, icono, version FROM flmodules WHERE bloqueo = %s """
                 % conn.driver().formatValue("bool", "True", False)
             )
 
         for idarea, idmodulo, descripcion, icono, version in list(result_modules):
-
             if idmodulo not in self.modules:
                 icon_cached = xpm.cache_xpm(icono)
                 self.modules[idmodulo] = module.Module(
                     idarea, idmodulo, descripcion, icon_cached, version
                 )
 
         result_files: Any = []
@@ -633,15 +625,14 @@
             )
 
         log_file = open(path._dir("project.txt"), "w")
 
         list_files: List[str] = []
         LOGGER.info("RUN: Populating cache.")
         for idmodulo, nombre, sha, contenido_or_bloqueo in list(result_files):
-
             if idmodulo not in self.modules.keys():  # Si el módulo no existe.
                 continue
 
             elif is_library and nombre.endswith("ui"):  # Si es un UI en modo librería.
                 continue
 
             elif nombre in self.files.keys():  # Si se sobreescribe un fichero ya existente.
@@ -661,29 +652,29 @@
             file_name = path._dir("cache", fileobj.filekey)
             if not os.path.isfile(file_name) or not os.path.getsize(
                 file_name
             ):  # Borra si no existe el fichero o está vacio.
                 if os.path.exists(fileobjdir):
                     utils_base.empty_dir(fileobjdir)
                 else:
-                    os.makedirs(fileobjdir)
+                    os.makedirs(fileobjdir, exist_ok=True)
 
                 contenido_content: Optional[str] = None
 
                 if not static_flfiles:
                     qry = conn.execute_query(
                         """SELECT contenido FROM flfiles WHERE sha = %s AND nombre = %s """
                         % (
                             conn.driver().formatValue("string", sha, False),
                             conn.driver().formatValue("string", nombre, False),
                         )
                     )
 
                     result_content: Any = None
-                    if qry is not None:
+                    if qry:
                         result_content = qry.first()
 
                     if result_content is not None:
                         contenido_content = result_content[
                             0
                         ]  # Recogemos verdadero contenido_content. cuando usamos flfiles. más rápido conexiones lentas.
                 else:
```

### Comparing `pineboo-1.0.4.1/pineboolib/application/proxy.py` & `pineboo-1.0.4.2/pineboolib/application/proxy.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/qsadictmodules.py` & `pineboo-1.0.4.2/pineboolib/application/qsadictmodules.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/qsatypes/date.py` & `pineboo-1.0.4.2/pineboolib/application/qsatypes/date.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/qsatypes/sysbasetype.py` & `pineboo-1.0.4.2/pineboolib/application/qsatypes/sysbasetype.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/qsatypes/tests/test_date.py` & `pineboo-1.0.4.2/pineboolib/application/qsatypes/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/qsatypes/tests/test_sysbasetype.py` & `pineboo-1.0.4.2/pineboolib/application/qsatypes/tests/test_sysbasetype.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/safeqsa.py` & `pineboo-1.0.4.2/pineboolib/application/safeqsa.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/signatures/pdf_digest.py` & `pineboo-1.0.4.2/pineboolib/application/signatures/pdf_digest.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/signatures/pdf_qr.py` & `pineboo-1.0.4.2/pineboolib/application/signatures/pdf_qr.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/signatures/tests/test_signatures.py` & `pineboo-1.0.4.2/pineboolib/application/signatures/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/signatures/xml_digest.py` & `pineboo-1.0.4.2/pineboolib/application/signatures/xml_digest.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/staticloader/pnmodulesstaticloader.py` & `pineboo-1.0.4.2/pineboolib/application/staticloader/pnmodulesstaticloader.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/staticloader/tests/test_static_loader.py` & `pineboo-1.0.4.2/pineboolib/application/staticloader/tests/test_static_loader.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/staticloader/ui/static_loader.ui` & `pineboo-1.0.4.2/pineboolib/application/staticloader/ui/static_loader.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/tests/test_application.py` & `pineboo-1.0.4.2/pineboolib/application/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/tests/test_load_script.py` & `pineboo-1.0.4.2/pineboolib/application/tests/test_load_script.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/tests/test_process.py` & `pineboo-1.0.4.2/pineboolib/application/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/tests/test_projectmodule.py` & `pineboo-1.0.4.2/pineboolib/application/tests/test_projectmodule.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/tests/test_proxy.py` & `pineboo-1.0.4.2/pineboolib/application/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/tests/test_types.py` & `pineboo-1.0.4.2/pineboolib/application/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/tests/test_xmlaction.py` & `pineboo-1.0.4.2/pineboolib/application/tests/test_xmlaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/translator/pntranslator.py` & `pineboo-1.0.4.2/pineboolib/application/translator/pntranslator.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/translator/test/test_pntranslator.py` & `pineboo-1.0.4.2/pineboolib/application/translator/test/test_pntranslator.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/types.py` & `pineboo-1.0.4.2/pineboolib/application/types.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/utils/check_dependencies.py` & `pineboo-1.0.4.2/pineboolib/application/utils/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/utils/convert_flaction.py` & `pineboo-1.0.4.2/pineboolib/application/utils/convert_flaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/utils/date_conversion.py` & `pineboo-1.0.4.2/pineboolib/application/utils/date_conversion.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/utils/flfiles_dir.py` & `pineboo-1.0.4.2/pineboolib/application/utils/flfiles_dir.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/utils/geometry.py` & `pineboo-1.0.4.2/pineboolib/application/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/utils/mobilemode.py` & `pineboo-1.0.4.2/pineboolib/application/utils/mobilemode.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/utils/modules.py` & `pineboo-1.0.4.2/pineboolib/application/utils/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,14 @@
     ):  # Si no existe el fichero o está vacio.
         file_dir = os.path.dirname(file_name)
         if not os.path.exists(file_dir):  # Si no existe la carpeta la crea
             os.makedirs(file_dir)
         elif os.path.exists(file_name):  # Si existe la carpeta borra el archivo erroneo
             os.remove(file_name)
 
-        pytnyzer.STRICT_MODE = False
-
         prog = flscriptparse.parse(source)
         if prog is None:
             raise ValueError("Failed to convert to Python")
         tree_data = flscriptparse.calctree(prog, alias_mode=0)
         ast = postparse.post_parse(tree_data)
 
         file_ = open(file_name, "w", encoding="UTF-8")
```

### Comparing `pineboo-1.0.4.1/pineboolib/application/utils/path.py` & `pineboo-1.0.4.2/pineboolib/application/utils/path.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/utils/service.py` & `pineboo-1.0.4.2/pineboolib/application/utils/service.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/utils/sql_tools.py` & `pineboo-1.0.4.2/pineboolib/application/utils/sql_tools.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/utils/xpm.py` & `pineboo-1.0.4.2/pineboolib/application/utils/xpm.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/application/xmlaction.py` & `pineboo-1.0.4.2/pineboolib/application/xmlaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/decorators.py` & `pineboo-1.0.4.2/pineboolib/core/decorators.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/exceptions.py` & `pineboo-1.0.4.2/pineboolib/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/garbage_collector.py` & `pineboo-1.0.4.2/pineboolib/core/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Pi-symbol.svg` & `pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Pi-symbol.svg`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi.psd` & `pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi.psd`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi2.xcf` & `pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi2.xcf`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi2_1024.png` & `pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi2_1024.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi2_256.png` & `pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi2_256.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi2_512.png` & `pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi2_512.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi_1024.png` & `pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi_1024.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi_256.png` & `pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi_256.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icono_pi/Symbol_pi_512.png` & `pineboo-1.0.4.2/pineboolib/core/images/icono_pi/Symbol_pi_512.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/about.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/about.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/aboutqt.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/aboutqt.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/cancel.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/consola.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/consola.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/date.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/date.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/delete.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/delete.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/down.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/down.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/edit.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/edit.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/edit_file.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/edit_file.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/edit_file_xml.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/edit_file_xml.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/estilo.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/estilo.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/exit.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/exit.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/fltable-clean.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/fltable-clean.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/fltable-data.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/fltable-data.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/fltable-odf.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/fltable-odf.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/folder_update.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/folder_update.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/font.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/font.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/go-bottom.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/go-bottom.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/go-down.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/go-down.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/go-first.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/go-first.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/go-home.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/go-home.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/go-jump.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/go-jump.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/go-last.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/go-last.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/go-next.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/go-next.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/go-previous.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/go-previous.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/go-top.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/go-top.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/go-up.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/go-up.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-add.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-add.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-bold.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-bold.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-cancel.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-cancel.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-clear.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-clear.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-copy.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-copy.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-cut.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-cut.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-delete.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-delete.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-find-and-replace.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-find-and-replace.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-find.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-find.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-fullscreen.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-fullscreen.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-go-back-ltr.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-go-back-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-go-back-rtl.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-go-back-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-go-down.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-go-down.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-go-forward-ltr.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-go-forward-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-go-forward-rtl.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-go-forward-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-go-up.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-go-up.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-goto-bottom.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-goto-bottom.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-goto-first-ltr.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-goto-first-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-goto-first-rtl.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-goto-first-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-goto-last-ltr.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-goto-last-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-goto-last-rtl.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-goto-last-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-goto-top.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-goto-top.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-home.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-home.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-indent-ltr.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-indent-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-indent-rtl.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-indent-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-italic.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-italic.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-jump-to-ltr.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-jump-to-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-jump-to-rtl.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-jump-to-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-justify-center.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-justify-center.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-justify-fill.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-justify-fill.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-justify-left.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-justify-left.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-justify-right.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-justify-right.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-forward-ltr.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-forward-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-forward-rtl.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-forward-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-next-ltr.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-next-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-next-rtl.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-next-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-play-ltr.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-play-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-previous-ltr.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-previous-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-previous-rtl.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-previous-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-record.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-record.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-rewind-ltr.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-rewind-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-rewind-rtl.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-rewind-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-media-stop.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-media-stop.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-new.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-new.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-open.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-open.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-paste.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-paste.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-print-preview.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-print-preview.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-print.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-print.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-properties.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-properties.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-redo-ltr.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-redo-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-refresh.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-refresh.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-save-as.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-save-as.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-save.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-save.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-select-all.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-select-all.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-stop.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-stop.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-strikethrough.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-strikethrough.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-underline.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-underline.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-undo-ltr.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-undo-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-unindent-ltr.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-unindent-ltr.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/gtk-unindent-rtl.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/gtk-unindent-rtl.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/help_index.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/help_index.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/insert.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/insert.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/lock.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/lock.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/ok.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/ok.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/paste.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/paste.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-128.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-128.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-16.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-16.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-24.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-24.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-256.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-256.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-32.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-32.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-48.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-48.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-57.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-57.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-64.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-64.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo-72.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo-72.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo-logo.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo-logo.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo-128.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo-128.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo-16.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo-16.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo-24.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo-24.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo-256.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo-256.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo-32.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo-32.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo-48.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo-48.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo-64.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo-64.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/pineboo2-logo.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/pineboo2-logo.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/print.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/print.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/reload.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/reload.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/signed_stamp.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/signed_stamp.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/sys_ebcomportamiento.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/sys_ebcomportamiento.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flareas.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flareas.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/sys_fldumpdb.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/sys_fldumpdb.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flgroups.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flgroups.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flloadmod.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flloadmod.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flloadmodpkg.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flloadmodpkg.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flmodules.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flmodules.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flmrproper.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flmrproper.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flreinit.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flreinit.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flreloadbatch.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flreloadbatch.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flreloadlast.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flreloadlast.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/sys_flusers.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/sys_flusers.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/terminal.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/terminal.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/unlock.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/unlock.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/up.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/up.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/icons/zoom.png` & `pineboo-1.0.4.2/pineboolib/core/images/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/splashscreen/dbadmin240.png` & `pineboo-1.0.4.2/pineboolib/core/images/splashscreen/dbadmin240.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/splashscreen/dbadmin480.png` & `pineboo-1.0.4.2/pineboolib/core/images/splashscreen/dbadmin480.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/splashscreen/quick240.png` & `pineboo-1.0.4.2/pineboolib/core/images/splashscreen/quick240.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/splashscreen/quick480.png` & `pineboo-1.0.4.2/pineboolib/core/images/splashscreen/quick480.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/splashscreen/splash.png` & `pineboo-1.0.4.2/pineboolib/core/images/splashscreen/splash.png`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/images/splashscreen/splash.svg` & `pineboo-1.0.4.2/pineboolib/core/images/splashscreen/splash.svg`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/message_manager.py` & `pineboo-1.0.4.2/pineboolib/core/message_manager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/settings.py` & `pineboo-1.0.4.2/pineboolib/core/settings.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/test/test_settings.py` & `pineboo-1.0.4.2/pineboolib/core/test/test_settings.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/utils/check_dependencies.py` & `pineboo-1.0.4.2/pineboolib/core/utils/check_dependencies.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/utils/logging.py` & `pineboo-1.0.4.2/pineboolib/core/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/utils/singleton.py` & `pineboo-1.0.4.2/pineboolib/core/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/utils/struct.py` & `pineboo-1.0.4.2/pineboolib/core/utils/struct.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/utils/tests/test_utils_base.py` & `pineboo-1.0.4.2/pineboolib/core/utils/tests/test_utils_base.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/utils/tests/test_version.py` & `pineboo-1.0.4.2/pineboolib/core/utils/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/utils/utils_base.py` & `pineboo-1.0.4.2/pineboolib/core/utils/utils_base.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/core/utils/version.py` & `pineboo-1.0.4.2/pineboolib/core/utils/version.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqformdb.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqformdb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqobjectquerylist.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqobjectquerylist.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqods.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqods.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqs.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqs.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqsbuttongroup.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqsbuttongroup.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqsobjectfactory.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqsobjectfactory.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqsql.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqsql.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/aqssproject.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/aqssproject.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/tests/test_aqobjectquerylist.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/tests/test_aqobjectquerylist.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/tests/test_aqods.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/tests/test_aqods.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/tests/test_aqs.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/tests/test_aqs.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/tests/test_aqsbuttongroup.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/tests/test_aqsbuttongroup.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/tests/test_aqsql.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/tests/test_aqsql.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/aqsobjects/tests/test_aqutil.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/aqsobjects/tests/test_aqutil.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flcodbar.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flcodbar.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/fldatatable.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/fldatatable.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/fldateedit.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/fldateedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/fldoublevalidator.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/fldoublevalidator.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flfastcgi.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flfastcgi.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flfielddb.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flfielddb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flformdb.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flformdb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flformrecorddb.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flformrecorddb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flformsearchdb.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flformsearchdb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flintvalidator.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flintvalidator.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/fllineedit.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/fllineedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/fllistviewitem.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/fllistviewitem.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flmanager.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flmanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flmanagermodules.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flmanagermodules.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flnetwork.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flnetwork.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flpixmapview.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flpixmapview.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flposprinter.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flposprinter.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flreportengine.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flreportengine.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flreportviewer.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flreportviewer.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flserialport.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flserialport.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flsettings.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flsettings.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flsmtpclient.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flsmtpclient.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flspinbox.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flspinbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/fltable.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/fltable.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/fltabledb.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/fltabledb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/fltimeedit.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/fltimeedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/fluintvalidator.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/fluintvalidator.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flutil.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flutil.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flvar.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flvar.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/flwidget.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/flwidget.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/forms/FLWidgetReportViewer.ui` & `pineboo-1.0.4.2/pineboolib/fllegacy/forms/FLWidgetReportViewer.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/systype.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/systype.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flcodbar.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flcodbar.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_fldatatable.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_fldatatable.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_fldateedit.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_fldateedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flfielddb.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flfielddb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flform.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flform.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flformrecorddb.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flformrecorddb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flformsearch.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flformsearch.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flmanager.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flmanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flreportengine.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flreportengine.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_fltabledb.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_fltabledb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_flutil.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_flutil.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_settings.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_smtp.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_smtp.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/fllegacy/tests/test_systype.py` & `pineboo-1.0.4.2/pineboolib/fllegacy/tests/test_systype.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/interfaces/iconnection.py` & `pineboo-1.0.4.2/pineboolib/interfaces/iconnection.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/interfaces/ifieldmetadata.py` & `pineboo-1.0.4.2/pineboolib/interfaces/ifieldmetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/interfaces/imainwindow.py` & `pineboo-1.0.4.2/pineboolib/interfaces/imainwindow.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/interfaces/imanager.py` & `pineboo-1.0.4.2/pineboolib/interfaces/imanager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/interfaces/isqlcursor.py` & `pineboo-1.0.4.2/pineboolib/interfaces/isqlcursor.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/interfaces/isqldriver.py` & `pineboo-1.0.4.2/pineboolib/interfaces/isqldriver.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/interfaces/itablemetadata.py` & `pineboo-1.0.4.2/pineboolib/interfaces/itablemetadata.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/loader/connection.py` & `pineboo-1.0.4.2/pineboolib/loader/connection.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/loader/dgi.py` & `pineboo-1.0.4.2/pineboolib/loader/dgi.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/loader/dlgconnect/conn_dialog.py` & `pineboo-1.0.4.2/pineboolib/loader/dlgconnect/conn_dialog.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/loader/dlgconnect/dlgconnect.py` & `pineboo-1.0.4.2/pineboolib/loader/dlgconnect/dlgconnect.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/loader/dlgconnect/dlgconnect.ui` & `pineboo-1.0.4.2/pineboolib/loader/dlgconnect/dlgconnect.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/loader/dlgconnect/tests/test_dlgconnect.py` & `pineboo-1.0.4.2/pineboolib/loader/dlgconnect/tests/test_dlgconnect.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/loader/init_project.py` & `pineboo-1.0.4.2/pineboolib/loader/init_project.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/loader/main.py` & `pineboo-1.0.4.2/pineboolib/loader/main.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/loader/options.py` & `pineboo-1.0.4.2/pineboolib/loader/options.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/loader/preload.py` & `pineboo-1.0.4.2/pineboolib/loader/preload.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/loader/projectconfig.py` & `pineboo-1.0.4.2/pineboolib/loader/projectconfig.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/loader/tests/test_connection.py` & `pineboo-1.0.4.2/pineboolib/loader/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/loader/tests/test_main.py` & `pineboo-1.0.4.2/pineboolib/loader/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/loader/tests/test_projectconfig.py` & `pineboo-1.0.4.2/pineboolib/loader/tests/test_projectconfig.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/loader/utils.py` & `pineboo-1.0.4.2/pineboolib/loader/utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_fcgi/dgi_fcgi.py` & `pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_fcgi/dgi_fcgi.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.py` & `pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui` & `pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/dlg_about/about_pineboo.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py` & `pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/progress_dialog_manager.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_objects/splash_screen.py` & `pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/splash_screen.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_objects/status_help_msg.py` & `pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_objects/status_help_msg.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_qt/dgi_qt.py` & `pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_qt/dgi_qt.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/dgi/dgi_schema.py` & `pineboo-1.0.4.2/pineboolib/plugins/dgi/dgi_schema.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo/eneboo.py` & `pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo/eneboo.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo/mainform.ui` & `pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo/mainform.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo/tests/test_eneboo.py` & `pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo/tests/test_eneboo.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo_mdi/eneboo_mdi.py` & `pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo_mdi/eneboo_mdi.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo_mdi/mainform.ui` & `pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo_mdi/mainform.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/mainform/eneboo_mdi/tests/test_eneboo_mdi.py` & `pineboo-1.0.4.2/pineboolib/plugins/mainform/eneboo_mdi/tests/test_eneboo_mdi.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/sql/flmysql_myisam.py` & `pineboo-1.0.4.2/pineboolib/plugins/sql/flmysql_myisam.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/sql/flpymssql.py` & `pineboo-1.0.4.2/pineboolib/plugins/sql/flpymssql.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/sql/flpyodbc.py` & `pineboo-1.0.4.2/pineboolib/plugins/sql/flpyodbc.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/sql/flqpsql.py` & `pineboo-1.0.4.2/pineboolib/plugins/sql/flqpsql.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/sql/flsqlite.py` & `pineboo-1.0.4.2/pineboolib/plugins/sql/flsqlite.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/sql/tests/test_flmysql_innodb.py` & `pineboo-1.0.4.2/pineboolib/plugins/sql/tests/test_flmysql_innodb.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/sql/tests/test_flmysql_myisam.py` & `pineboo-1.0.4.2/pineboolib/plugins/sql/tests/test_flmysql_myisam.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/sql/tests/test_flpymssql.py` & `pineboo-1.0.4.2/pineboolib/plugins/sql/tests/test_flpymssql.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/sql/tests/test_flpyodbc.py` & `pineboo-1.0.4.2/pineboolib/plugins/sql/tests/test_flpyodbc.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/sql/tests/test_flsqlite.py` & `pineboo-1.0.4.2/pineboolib/plugins/sql/tests/test_flsqlite.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/sql/tests/test_qpsql.py` & `pineboo-1.0.4.2/pineboolib/plugins/sql/tests/test_qpsql.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/plugins/sql/tests/test_stress.py` & `pineboo-1.0.4.2/pineboolib/plugins/sql/tests/test_stress.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/checkbox.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/dateedit.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/dateedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/dialog.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/filedialog.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/filedialog.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/lineedit.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/lineedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/messagebox.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/messagebox.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Messagebox module."""
 
 # -*- coding: utf-8 -*-
 from PyQt6 import QtWidgets  # type: ignore[import]
 
 from pineboolib import application
+from pineboolib.core.utils import utils_base
 from pineboolib.core.utils import logging
 import clipboard  # type: ignore [import] # noqa: F821
 
 from typing import Optional, List
 
 LOGGER = logging.get_logger(__name__)
 
@@ -23,15 +24,15 @@
     Ignore = QtWidgets.QMessageBox.StandardButton.Ignore
 
     @classmethod
     def msgbox(cls, typename, *args) -> Optional["QtWidgets.QMessageBox.StandardButton"]:
         """Return a messageBox."""
 
         if not getattr(application, "TESTING_MODE", None):
-            if QtWidgets.QApplication.platformName() == "offscreen":
+            if utils_base.is_library():
                 LOGGER.warning(
                     "q3widget.MessageBox launch when library mode ON! (%s : %s)",
                     typename,
                     args,
                     stack_info=True,
                 )
                 return None
```

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/numberedit.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/numberedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qaction.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qaction.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qbuttongroup.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qbuttongroup.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qbytearray.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qbytearray.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qcheckbox.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qcheckbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qcombobox.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qcombobox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qdateedit.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qdateedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qdialog.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qdialog.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qframe.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qframe.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qgroupbox.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qgroupbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qhboxlayout.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qhboxlayout.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qhttp.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qhttp.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qlabel.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qlabel.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qline.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qline.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qlineedit.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qlineedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qlistview.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qlistview.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qobject.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qobject.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qpushbutton.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qpushbutton.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qradiobutton.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qradiobutton.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qtable.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qtable.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qtabwidget.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qtabwidget.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qtextedit.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qtextedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qtimeedit.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qtimeedit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qtoolbutton.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qtoolbutton.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qvboxlayout.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qvboxlayout.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/qwidget.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/qwidget.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/spinbox.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/spinbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_messagebox.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_messagebox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_qbytearray.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_qbytearray.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_qhttp.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_qhttp.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_qpushbutton.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_qpushbutton.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_qradiobuttons.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_qradiobuttons.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_qtabwidget.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_qtabwidget.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_qtextstream.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_qtextstream.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/q3widgets/tests/test_spinbox.py` & `pineboo-1.0.4.2/pineboolib/q3widgets/tests/test_spinbox.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/qsa/decorators.py` & `pineboo-1.0.4.2/pineboolib/qsa/decorators.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/qsa/emptyscript.py` & `pineboo-1.0.4.2/pineboolib/qsa/emptyscript.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/qsa/formdbwidget.py` & `pineboo-1.0.4.2/pineboolib/qsa/formdbwidget.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/qsa/input.py` & `pineboo-1.0.4.2/pineboolib/qsa/input.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/qsa/object_class.py` & `pineboo-1.0.4.2/pineboolib/qsa/object_class.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/qsa/pncontrolsfactory.py` & `pineboo-1.0.4.2/pineboolib/qsa/pncontrolsfactory.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/qsa/qsa.py` & `pineboo-1.0.4.2/pineboolib/qsa/qsa.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/qsa/tests/test_class.py` & `pineboo-1.0.4.2/pineboolib/qsa/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/qsa/tests/test_classes.py` & `pineboo-1.0.4.2/pineboolib/qsa/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/qsa/tests/test_knownbugs.py` & `pineboo-1.0.4.2/pineboolib/qsa/tests/test_knownbugs.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/qsa/tests/test_orm.py` & `pineboo-1.0.4.2/pineboolib/qsa/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/qsa/tests/test_query_values.py` & `pineboo-1.0.4.2/pineboolib/qsa/tests/test_query_values.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/qsa/tests/test_require.py` & `pineboo-1.0.4.2/pineboolib/qsa/tests/test_require.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Test require module."""
 
 from pineboolib.application import qsadictmodules
-from pineboolib.application.parsers.parser_qsa import pytnyzer
+from pineboolib.application.parsers import parser_qsa
 from importlib import util
 from pineboolib.qsa.tests import fixture_path
 from pineboolib.loader.main import init_testing, finish_testing
 import os
 
 import unittest
 
@@ -13,15 +13,15 @@
 class TestRequire(unittest.TestCase):
     """Test Require."""
 
     @classmethod
     def setUpClass(cls) -> None:
         """Ensure pineboo is initialized for testing."""
         init_testing()
-        pytnyzer.STRICT_MODE = True
+        parser_qsa.STRICT_MODE = True
         util_path = fixture_path("Import.py")
         spec = util.spec_from_file_location("Import", util_path)
         if spec and spec.loader is not None:
             module_instance = util.module_from_spec(spec)
             spec.loader.exec_module(module_instance)  # type: ignore [attr-defined]
             main_class = module_instance.FormInternalObj()  # type: ignore [attr-defined]
             qsadictmodules.QSADictModules.set_qsa_tree("formImport", main_class)  # type: ignore [arg-type]
```

### Comparing `pineboo-1.0.4.1/pineboolib/qsa/tests/test_utils.py` & `pineboo-1.0.4.2/pineboolib/qsa/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/qsa/utils.py` & `pineboo-1.0.4.2/pineboolib/qsa/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,19 @@
         """Return if regex is global."""
         return self.is_global
 
     def set_global(self, state: bool) -> None:
         """Set regex global flag."""
         self.is_global = state
 
+    def exactMatch(self, value: str) -> Optional[Match[str]]:
+        """Return exactMatch."""
+
+        return self.pattern.fullmatch(value)
+
     global_ = property(get_global, set_global)
 
 
 def reg_exp(str_re: str) -> QsaRegExp:
     """
     Return qsaRegexp object from search.
 
@@ -431,15 +436,15 @@
 def is_nan(value: Any) -> bool:
     """
     Check if value is NaN.
 
     @param x. Valor numérico
     @return True o False
     """
-    if value in [None, ""]:
+    if value in [None, "", True, False]:
         return True
 
     if isinstance(value, str) and value.find(":"):
         value = value.replace(":", "")
     try:
         value = float(value)
         return math.isnan(value)
@@ -474,15 +479,14 @@
             if len(real_args) == 2:  # Delete
                 pos_ini = real_args[0]
                 length_ = real_args[1]
                 for i in reversed(range(pos_ini, pos_ini + length_)):
                     array_.pop(i)
 
             elif len(real_args) > 2 and real_args[1] == 0:  # Insertion
-
                 for value in reversed(real_args[2:]):
                     array_.insert(real_args[0], value)
 
             elif len(real_args) > 2 and real_args[1] > 0:  # Replacement
                 pos_ini = real_args[0]
                 replacement_size = real_args[1]
                 new_values = real_args[2:]
@@ -519,15 +523,14 @@
         """Sort function."""
 
         new_array_: List = []
         if self._function is not None:
             for pos, value in enumerate(array_):
                 found = False
                 for new_pos, new_value in enumerate(list(new_array_)):
-
                     result = self._function(value, new_value)
                     # print("Comparando", value, new_value, result, "-->", new_array_)
                     if result == 0:
                         # print("Es igual (%s == %s)" % (value, new_value))
                         new_array_.append(value)
                         found = True
                         break
```

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/forms/FLWidgetMasterTable.ui` & `pineboo-1.0.4.2/pineboolib/system_module/forms/FLWidgetMasterTable.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/forms/ebcomportamiento.ui` & `pineboo-1.0.4.2/pineboolib/system_module/forms/ebcomportamiento.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/forms/flareas.ui` & `pineboo-1.0.4.2/pineboolib/system_module/forms/flareas.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/forms/flfiles.ui` & `pineboo-1.0.4.2/pineboolib/system_module/forms/flfiles.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/forms/flgroups.ui` & `pineboo-1.0.4.2/pineboolib/system_module/forms/flgroups.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/forms/flmodulos.ui` & `pineboo-1.0.4.2/pineboolib/system_module/forms/flmodulos.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/forms/fltest.ui` & `pineboo-1.0.4.2/pineboolib/system_module/forms/fltest.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/forms/flusers.ui` & `pineboo-1.0.4.2/pineboolib/system_module/forms/flusers.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/forms/master.ui` & `pineboo-1.0.4.2/pineboolib/system_module/forms/master.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/forms/master_copy.ui` & `pineboo-1.0.4.2/pineboolib/system_module/forms/master_copy.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/forms/master_print.ui` & `pineboo-1.0.4.2/pineboolib/system_module/forms/master_print.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/forms/master_print_copy.ui` & `pineboo-1.0.4.2/pineboolib/system_module/forms/master_print_copy.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/forms/sys.ui` & `pineboo-1.0.4.2/pineboolib/system_module/forms/sys.ui`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/flareas_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/flareas_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/flfiles_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/flfiles_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/flgroups_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/flgroups_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/fllarge_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/fllarge_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/flmetadata_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/flmetadata_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/flmodules_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/flmodules_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/flseqs_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/flseqs_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/flserial_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/flserial_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/flsettings_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/flsettings_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/fltest2_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/fltest2_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/fltest3_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/fltest3_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/fltest4_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/fltest4_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/fltest5_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/fltest5_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/fltest_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/fltest_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/flupdates_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/flupdates_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/flusers_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/flusers_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/models/flvar_model.py` & `pineboo-1.0.4.2/pineboolib/system_module/models/flvar_model.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/queries/fltest2.qry` & `pineboo-1.0.4.2/pineboolib/system_module/queries/fltest2.qry`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/scripts/ebcomportamiento.py` & `pineboo-1.0.4.2/pineboolib/system_module/scripts/ebcomportamiento.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/scripts/flfiles.py` & `pineboo-1.0.4.2/pineboolib/system_module/scripts/flfiles.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/scripts/flloadmod.py` & `pineboo-1.0.4.2/pineboolib/system_module/scripts/flloadmod.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/scripts/flmodules.py` & `pineboo-1.0.4.2/pineboolib/system_module/scripts/flmodules.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/scripts/flreloadbatch.py` & `pineboo-1.0.4.2/pineboolib/system_module/scripts/flreloadbatch.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/scripts/flreloadlast.py` & `pineboo-1.0.4.2/pineboolib/system_module/scripts/flreloadlast.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/scripts/sys.py` & `pineboo-1.0.4.2/pineboolib/system_module/scripts/sys.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_ebcomportamiento.py` & `pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_ebcomportamiento.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_flfiles.py` & `pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_flfiles.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_flloadmodpkg.py` & `pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_flloadmodpkg.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_flmodules.py` & `pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_flmodules.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_flmrproper.py` & `pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_flmrproper.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_flreinit.py` & `pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_flreinit.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_reload_last.py` & `pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_reload_last.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/scripts/tests/test_sys.py` & `pineboo-1.0.4.2/pineboolib/system_module/scripts/tests/test_sys.py`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/sys.xml` & `pineboo-1.0.4.2/pineboolib/system_module/sys.xml`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/sys.xpm` & `pineboo-1.0.4.2/pineboolib/system_module/sys.xpm`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/translations/sys.ca.ts` & `pineboo-1.0.4.2/pineboolib/system_module/translations/sys.ca.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/translations/sys.de.ts` & `pineboo-1.0.4.2/pineboolib/system_module/translations/sys.de.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/translations/sys.en.ts` & `pineboo-1.0.4.2/pineboolib/system_module/translations/sys.en.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/translations/sys.es.ts` & `pineboo-1.0.4.2/pineboolib/system_module/translations/sys.es.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/translations/sys.fr.ts` & `pineboo-1.0.4.2/pineboolib/system_module/translations/sys.fr.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/translations/sys.gl.ts` & `pineboo-1.0.4.2/pineboolib/system_module/translations/sys.gl.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/translations/sys.it.ts` & `pineboo-1.0.4.2/pineboolib/system_module/translations/sys.it.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/pineboolib/system_module/translations/sys.pt.ts` & `pineboo-1.0.4.2/pineboolib/system_module/translations/sys.pt.ts`

 * *Files identical despite different names*

### Comparing `pineboo-1.0.4.1/setup.py` & `pineboo-1.0.4.2/setup.py`

 * *Files identical despite different names*

