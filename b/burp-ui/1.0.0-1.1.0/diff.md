# Comparing `tmp/burp-ui-1.0.0.tar.gz` & `tmp/burp-ui-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burp-ui-1.0.0.tar", last modified: Sun Nov  6 20:40:37 2022, max compression
+gzip compressed data, was "burp-ui-1.1.0.tar", last modified: Mon May  1 19:13:30 2023, max compression
```

## Comparing `burp-ui-1.0.0.tar` & `burp-ui-1.1.0.tar`

### file list

```diff
@@ -1,517 +1,517 @@
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.735190 burp-ui-1.0.0/
--rw-r--r--   0 master    (1000) master    (1000)    22556 2022-11-06 20:36:34.000000 burp-ui-1.0.0/CHANGELOG.rst
--rw-r--r--   0 master    (1000) master    (1000)      368 2021-09-17 12:05:44.000000 burp-ui-1.0.0/CONTRIBUTORS
--rw-r--r--   0 master    (1000) master    (1000)     1575 2018-05-14 12:28:48.000000 burp-ui-1.0.0/LICENSE
--rw-r--r--   0 master    (1000) master    (1000)      342 2019-11-04 21:35:27.000000 burp-ui-1.0.0/MANIFEST.in
--rw-r--r--   0 master    (1000) master    (1000)     5873 2022-11-06 20:40:37.735190 burp-ui-1.0.0/PKG-INFO
--rw-r--r--   0 master    (1000) master    (1000)     5025 2021-09-17 12:05:44.000000 burp-ui-1.0.0/README.rst
--rw-r--r--   0 master    (1000) master    (1000)      229 2017-04-28 13:40:18.000000 burp-ui-1.0.0/babel.cfg
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.675189 burp-ui-1.0.0/burp_ui.egg-info/
--rw-r--r--   0 master    (1000) master    (1000)     5873 2022-11-06 20:40:37.000000 burp-ui-1.0.0/burp_ui.egg-info/PKG-INFO
--rw-r--r--   0 master    (1000) master    (1000)    15086 2022-11-06 20:40:37.000000 burp-ui-1.0.0/burp_ui.egg-info/SOURCES.txt
--rw-r--r--   0 master    (1000) master    (1000)        1 2022-11-06 20:40:37.000000 burp-ui-1.0.0/burp_ui.egg-info/dependency_links.txt
--rw-r--r--   0 master    (1000) master    (1000)      243 2022-11-06 20:40:37.000000 burp-ui-1.0.0/burp_ui.egg-info/entry_points.txt
--rw-r--r--   0 master    (1000) master    (1000)      756 2022-11-06 20:40:37.000000 burp-ui-1.0.0/burp_ui.egg-info/requires.txt
--rw-r--r--   0 master    (1000) master    (1000)        7 2022-11-06 20:40:37.000000 burp-ui-1.0.0/burp_ui.egg-info/top_level.txt
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.679189 burp-ui-1.0.0/burpui/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.679189 burp-ui-1.0.0/burpui/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)    12191 2019-10-03 09:41:02.000000 burp-ui-1.0.0/burpui/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2018-06-05 15:54:46.000000 burp-ui-1.0.0/burpui/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)      779 2019-10-03 09:41:02.000000 burp-ui-1.0.0/burpui/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.000000 burp-ui-1.0.0/burpui/RELEASE
--rw-r--r--   0 master    (1000) master    (1000)        6 2022-11-06 20:36:47.000000 burp-ui-1.0.0/burpui/VERSION
--rw-r--r--   0 master    (1000) master    (1000)      382 2021-09-17 12:05:44.000000 burp-ui-1.0.0/burpui/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)     9534 2021-09-17 12:05:44.000000 burp-ui-1.0.0/burpui/__main__.py
--rw-r--r--   0 master    (1000) master    (1000)      249 2021-05-12 15:45:53.000000 burp-ui-1.0.0/burpui/_cli.py
--rw-r--r--   0 master    (1000) master    (1000)     2059 2021-09-17 12:05:44.000000 burp-ui-1.0.0/burpui/_compat.py
--rw-r--r--   0 master    (1000) master    (1000)     1202 2021-09-17 12:05:44.000000 burp-ui-1.0.0/burpui/_json.py
--rw-r--r--   0 master    (1000) master    (1000)      397 2021-09-17 12:05:44.000000 burp-ui-1.0.0/burpui/_rtfd.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.683189 burp-ui-1.0.0/burpui/api/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.683189 burp-ui-1.0.0/burpui/api/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4794 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/api/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)     2643 2018-09-14 14:17:22.000000 burp-ui-1.0.0/burpui/api/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-23 14:42:15.000000 burp-ui-1.0.0/burpui/api/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2018-09-14 14:17:22.000000 burp-ui-1.0.0/burpui/api/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)     8428 2021-09-17 19:21:59.000000 burp-ui-1.0.0/burpui/api/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    60893 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/api/admin.py
--rw-r--r--   0 master    (1000) master    (1000)     4961 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/api/backup.py
--rw-r--r--   0 master    (1000) master    (1000)    36404 2022-11-06 20:18:32.000000 burp-ui-1.0.0/burpui/api/client.py
--rw-r--r--   0 master    (1000) master    (1000)    25729 2021-09-17 19:48:45.000000 burp-ui-1.0.0/burpui/api/clients.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.683189 burp-ui-1.0.0/burpui/api/custom/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.683189 burp-ui-1.0.0/burpui/api/custom/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-01 14:25:10.000000 burp-ui-1.0.0/burpui/api/custom/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)      291 2019-10-01 14:25:10.000000 burp-ui-1.0.0/burpui/api/custom/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-01 14:25:10.000000 burp-ui-1.0.0/burpui/api/custom/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2019-10-01 14:25:10.000000 burp-ui-1.0.0/burpui/api/custom/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)      213 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/api/custom/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)      588 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/api/custom/fields.py
--rw-r--r--   0 master    (1000) master    (1000)     2860 2021-09-17 23:27:12.000000 burp-ui-1.0.0/burpui/api/custom/my_fields.py
--rw-r--r--   0 master    (1000) master    (1000)     1430 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/api/custom/resource.py
--rw-r--r--   0 master    (1000) master    (1000)    35390 2021-09-17 23:27:12.000000 burp-ui-1.0.0/burpui/api/misc.py
--rw-r--r--   0 master    (1000) master    (1000)     8585 2022-11-06 13:46:24.000000 burp-ui-1.0.0/burpui/api/prefs.py
--rw-r--r--   0 master    (1000) master    (1000)    17614 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/api/restore.py
--rw-r--r--   0 master    (1000) master    (1000)     8028 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/api/servers.py
--rw-r--r--   0 master    (1000) master    (1000)    35778 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/api/settings.py
--rw-r--r--   0 master    (1000) master    (1000)    32801 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/api/tasks.py
--rw-r--r--   0 master    (1000) master    (1000)    15681 2021-09-17 23:27:12.000000 burp-ui-1.0.0/burpui/app.py
--rw-r--r--   0 master    (1000) master    (1000)    16384 2017-07-26 14:40:04.000000 burp-ui-1.0.0/burpui/celerybeat-schedule
--rw-r--r--   0 master    (1000) master    (1000)    45220 2021-10-06 15:22:13.000000 burp-ui-1.0.0/burpui/cli.py
--rw-r--r--   0 master    (1000) master    (1000)    10045 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/config.py
--rw-r--r--   0 master    (1000) master    (1000)    23767 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/datastructures.py
--rw-r--r--   0 master    (1000) master    (1000)     2769 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/decorators.py
--rw-r--r--   0 master    (1000) master    (1000)      964 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/desc.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.683189 burp-ui-1.0.0/burpui/engines/
--rw-r--r--   0 master    (1000) master    (1000)        0 2019-11-04 21:35:27.000000 burp-ui-1.0.0/burpui/engines/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    14172 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/engines/agent.py
--rw-r--r--   0 master    (1000) master    (1000)    11303 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/engines/monitor.py
--rw-r--r--   0 master    (1000) master    (1000)    17915 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/engines/server.py
--rw-r--r--   0 master    (1000) master    (1000)      943 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/engines/worker.py
--rw-r--r--   0 master    (1000) master    (1000)      871 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/exceptions.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.687189 burp-ui-1.0.0/burpui/ext/
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/ext/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)      349 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/ext/cache.py
--rw-r--r--   0 master    (1000) master    (1000)      946 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/ext/i18n.py
--rw-r--r--   0 master    (1000) master    (1000)      309 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/ext/limit.py
--rw-r--r--   0 master    (1000) master    (1000)      233 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/ext/session.py
--rw-r--r--   0 master    (1000) master    (1000)      232 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/ext/sql.py
--rw-r--r--   0 master    (1000) master    (1000)      230 2019-04-02 19:43:50.000000 burp-ui-1.0.0/burpui/ext/tasks.py
--rw-r--r--   0 master    (1000) master    (1000)      544 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/ext/ws.py
--rw-r--r--   0 master    (1000) master    (1000)    11896 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/extensions.py
--rw-r--r--   0 master    (1000) master    (1000)     3524 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/filter.py
--rw-r--r--   0 master    (1000) master    (1000)      728 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/forms.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.687189 burp-ui-1.0.0/burpui/misc/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.687189 burp-ui-1.0.0/burpui/misc/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4794 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/misc/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)     2452 2018-07-23 07:59:35.000000 burp-ui-1.0.0/burpui/misc/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-20 15:54:46.000000 burp-ui-1.0.0/burpui/misc/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2018-07-23 07:59:35.000000 burp-ui-1.0.0/burpui/misc/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/misc/__init__.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.687189 burp-ui-1.0.0/burpui/misc/acl/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.687189 burp-ui-1.0.0/burpui/misc/acl/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4794 2019-09-24 13:37:49.000000 burp-ui-1.0.0/burpui/misc/acl/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)      346 2019-09-27 12:40:13.000000 burp-ui-1.0.0/burpui/misc/acl/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2019-09-25 20:15:11.000000 burp-ui-1.0.0/burpui/misc/acl/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2019-09-27 12:40:13.000000 burp-ui-1.0.0/burpui/misc/acl/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/misc/acl/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    14445 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/acl/basic.py
--rw-r--r--   0 master    (1000) master    (1000)     5656 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/acl/handler.py
--rw-r--r--   0 master    (1000) master    (1000)     5390 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/acl/interface.py
--rw-r--r--   0 master    (1000) master    (1000)    28562 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/acl/meta.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.687189 burp-ui-1.0.0/burpui/misc/audit/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.691189 burp-ui-1.0.0/burpui/misc/audit/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/misc/audit/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)      138 2018-08-03 09:24:44.000000 burp-ui-1.0.0/burpui/misc/audit/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2018-06-05 13:59:15.000000 burp-ui-1.0.0/burpui/misc/audit/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)       27 2018-08-03 09:24:44.000000 burp-ui-1.0.0/burpui/misc/audit/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2019-11-04 21:35:27.000000 burp-ui-1.0.0/burpui/misc/audit/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)     2782 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/audit/basic.py
--rw-r--r--   0 master    (1000) master    (1000)     3569 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/audit/handler.py
--rw-r--r--   0 master    (1000) master    (1000)     1855 2019-11-04 21:35:27.000000 burp-ui-1.0.0/burpui/misc/audit/interface.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.691189 burp-ui-1.0.0/burpui/misc/auth/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.691189 burp-ui-1.0.0/burpui/misc/auth/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/misc/auth/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)      763 2019-01-29 14:01:08.000000 burp-ui-1.0.0/burpui/misc/auth/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2018-06-07 15:21:13.000000 burp-ui-1.0.0/burpui/misc/auth/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)     2077 2019-01-29 14:01:08.000000 burp-ui-1.0.0/burpui/misc/auth/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/misc/auth/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)     9655 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/auth/basic.py
--rw-r--r--   0 master    (1000) master    (1000)    10821 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/auth/handler.py
--rw-r--r--   0 master    (1000) master    (1000)     3488 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/auth/interface.py
--rw-r--r--   0 master    (1000) master    (1000)    11183 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/auth/ldap.py
--rw-r--r--   0 master    (1000) master    (1000)     4674 2021-09-17 23:27:12.000000 burp-ui-1.0.0/burpui/misc/auth/local.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.691189 burp-ui-1.0.0/burpui/misc/backend/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.691189 burp-ui-1.0.0/burpui/misc/backend/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/misc/backend/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)     1168 2020-05-08 22:06:12.000000 burp-ui-1.0.0/burpui/misc/backend/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-18 09:19:37.000000 burp-ui-1.0.0/burpui/misc/backend/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2020-05-08 22:06:12.000000 burp-ui-1.0.0/burpui/misc/backend/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/misc/backend/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    47313 2021-10-06 15:22:17.000000 burp-ui-1.0.0/burpui/misc/backend/burp1.py
--rw-r--r--   0 master    (1000) master    (1000)    30603 2021-10-06 15:22:17.000000 burp-ui-1.0.0/burpui/misc/backend/burp2.py
--rw-r--r--   0 master    (1000) master    (1000)    41268 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/backend/interface.py
--rw-r--r--   0 master    (1000) master    (1000)    23473 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/backend/multi.py
--rw-r--r--   0 master    (1000) master    (1000)    38355 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/backend/parallel.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.695190 burp-ui-1.0.0/burpui/misc/backend/utils/
--rw-r--r--   0 master    (1000) master    (1000)        0 2019-11-04 21:35:27.000000 burp-ui-1.0.0/burpui/misc/backend/utils/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    12736 2021-10-06 15:22:17.000000 burp-ui-1.0.0/burpui/misc/backend/utils/burp2.py
--rw-r--r--   0 master    (1000) master    (1000)      398 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/backend/utils/constant.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.695190 burp-ui-1.0.0/burpui/misc/parser/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.695190 burp-ui-1.0.0/burpui/misc/parser/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-01 12:38:25.000000 burp-ui-1.0.0/burpui/misc/parser/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)      431 2021-10-04 08:39:12.000000 burp-ui-1.0.0/burpui/misc/parser/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-03 09:34:38.000000 burp-ui-1.0.0/burpui/misc/parser/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2021-10-04 08:39:12.000000 burp-ui-1.0.0/burpui/misc/parser/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/misc/parser/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)    37465 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/parser/burp1.py
--rw-r--r--   0 master    (1000) master    (1000)    13883 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/parser/burp2.py
--rw-r--r--   0 master    (1000) master    (1000)    43592 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/parser/doc.py
--rw-r--r--   0 master    (1000) master    (1000)    17679 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/parser/interface.py
--rw-r--r--   0 master    (1000) master    (1000)     8075 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/parser/openssl.py
--rw-r--r--   0 master    (1000) master    (1000)    57168 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/misc/parser/utils.py
--rw-r--r--   0 master    (1000) master    (1000)     3398 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/models.py
--rw-r--r--   0 master    (1000) master    (1000)     2642 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/plugins.py
--rw-r--r--   0 master    (1000) master    (1000)    17405 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/routes.py
--rw-r--r--   0 master    (1000) master    (1000)     2912 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/security.py
--rw-r--r--   0 master    (1000) master    (1000)    11088 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/sessions.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.695190 burp-ui-1.0.0/burpui/static/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.655189 burp-ui-1.0.0/burpui/static/3rdparty/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.695190 burp-ui-1.0.0/burpui/static/3rdparty/highlightjs/
--rw-r--r--   0 master    (1000) master    (1000)     8711 2018-05-14 12:28:49.000000 burp-ui-1.0.0/burpui/static/3rdparty/highlightjs/highlight.pack.js
--rw-r--r--   0 master    (1000) master    (1000)     1211 2018-05-14 12:28:49.000000 burp-ui-1.0.0/burpui/static/3rdparty/highlightjs/style.css
--rw-r--r--   0 master    (1000) master    (1000)     7298 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/static/dashboard.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.655189 burp-ui-1.0.0/burpui/static/extra/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.695190 burp-ui-1.0.0/burpui/static/extra/i18n/
--rw-r--r--   0 master    (1000) master    (1000)      885 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/static/extra/i18n/datatable-es.json
--rw-r--r--   0 master    (1000) master    (1000)      990 2017-04-28 13:40:18.000000 burp-ui-1.0.0/burpui/static/extra/i18n/datatable-fr.json
--rw-r--r--   0 master    (1000) master    (1000)      818 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/static/extra/i18n/datatable-it.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.695190 burp-ui-1.0.0/burpui/static/images/
--rw-r--r--   0 master    (1000) master    (1000)     1150 2017-04-28 13:40:18.000000 burp-ui-1.0.0/burpui/static/images/favicon.ico
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.695190 burp-ui-1.0.0/burpui/static/vendor/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.695190 burp-ui-1.0.0/burpui/static/vendor/ace-builds/
--rw-r--r--   0 master    (1000) master    (1000)      517 2021-09-17 08:35:27.000000 burp-ui-1.0.0/burpui/static/vendor/ace-builds/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      545 2021-09-17 08:35:27.000000 burp-ui-1.0.0/burpui/static/vendor/ace-builds/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.699190 burp-ui-1.0.0/burpui/static/vendor/ace-builds/src-min-noconflict/
--rw-r--r--   0 master    (1000) master    (1000)   358296 2021-09-17 08:35:27.000000 burp-ui-1.0.0/burpui/static/vendor/ace-builds/src-min-noconflict/ace.js
--rw-r--r--   0 master    (1000) master    (1000)     5505 2021-09-17 08:35:27.000000 burp-ui-1.0.0/burpui/static/vendor/ace-builds/src-min-noconflict/mode-json.js
--rw-r--r--   0 master    (1000) master    (1000)    27789 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/ace-builds/src-min-noconflict/theme-ambiance.js
--rw-r--r--   0 master    (1000) master    (1000)    32966 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/ace-builds/src-min-noconflict/worker-json.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.699190 burp-ui-1.0.0/burpui/static/vendor/angular/
--rw-r--r--   0 master    (1000) master    (1000)   169920 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular/angular.min.js
--rw-r--r--   0 master    (1000) master    (1000)      133 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      572 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.699190 burp-ui-1.0.0/burpui/static/vendor/angular-animate/
--rw-r--r--   0 master    (1000) master    (1000)    25733 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-animate/angular-animate.min.js
--rw-r--r--   0 master    (1000) master    (1000)      172 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-animate/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      702 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-animate/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.699190 burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap/
--rw-r--r--   0 master    (1000) master    (1000)      460 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      569 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap/package.json
--rw-r--r--   0 master    (1000) master    (1000)   125728 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap/ui-bootstrap-tpls.min.js
--rw-r--r--   0 master    (1000) master    (1000)   103577 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap/ui-bootstrap.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.699190 burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap-switch/
--rw-r--r--   0 master    (1000) master    (1000)      799 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap-switch/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.699190 burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap-switch/dist/
--rw-r--r--   0 master    (1000) master    (1000)     3139 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap-switch/dist/angular-bootstrap-switch.min.js
--rw-r--r--   0 master    (1000) master    (1000)     1228 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap-switch/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.699190 burp-ui-1.0.0/burpui/static/vendor/angular-datatables-0.6.2/
--rw-r--r--   0 master    (1000) master    (1000)     1720 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-datatables-0.6.2/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.699190 burp-ui-1.0.0/burpui/static/vendor/angular-datatables-0.6.2/dist/
--rw-r--r--   0 master    (1000) master    (1000)    14421 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-datatables-0.6.2/dist/angular-datatables.min.js
--rw-r--r--   0 master    (1000) master    (1000)     1846 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-datatables-0.6.2/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.699190 burp-ui-1.0.0/burpui/static/vendor/angular-highlightjs/
--rw-r--r--   0 master    (1000) master    (1000)      457 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-highlightjs/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/angular-highlightjs/build/
--rw-r--r--   0 master    (1000) master    (1000)     4707 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-highlightjs/build/angular-highlightjs.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/angular-onbeforeunload/
--rw-r--r--   0 master    (1000) master    (1000)      678 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-onbeforeunload/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/angular-onbeforeunload/build/
--rw-r--r--   0 master    (1000) master    (1000)      906 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-onbeforeunload/build/angular-onbeforeunload.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/angular-resource/
--rw-r--r--   0 master    (1000) master    (1000)     4508 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-resource/angular-resource.min.js
--rw-r--r--   0 master    (1000) master    (1000)      174 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-resource/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      738 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-resource/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/angular-route/
--rw-r--r--   0 master    (1000) master    (1000)     5611 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-route/angular-route.min.js
--rw-r--r--   0 master    (1000) master    (1000)      168 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-route/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      687 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-route/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/angular-sanitize/
--rw-r--r--   0 master    (1000) master    (1000)     6612 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-sanitize/angular-sanitize.min.js
--rw-r--r--   0 master    (1000) master    (1000)      174 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-sanitize/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      704 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-sanitize/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/angular-strap/
--rw-r--r--   0 master    (1000) master    (1000)     1268 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-strap/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/angular-strap/dist/
--rw-r--r--   0 master    (1000) master    (1000)    83061 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-strap/dist/angular-strap.min.js
--rw-r--r--   0 master    (1000) master    (1000)     9858 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-strap/dist/angular-strap.tpl.min.js
--rw-r--r--   0 master    (1000) master    (1000)     1756 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-strap/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/angular-ui-calendar/
--rw-r--r--   0 master    (1000) master    (1000)      739 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-ui-calendar/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/angular-ui-calendar/src/
--rw-r--r--   0 master    (1000) master    (1000)    16233 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-ui-calendar/src/calendar.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/angular-ui-select/
--rw-r--r--   0 master    (1000) master    (1000)      574 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-ui-select/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/angular-ui-select/dist/
--rw-r--r--   0 master    (1000) master    (1000)     6092 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-ui-select/dist/select.min.css
--rw-r--r--   0 master    (1000) master    (1000)    45235 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-ui-select/dist/select.min.js
--rw-r--r--   0 master    (1000) master    (1000)     1738 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-ui-select/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/angular-ui-select3/
--rw-r--r--   0 master    (1000) master    (1000)      374 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-ui-select3/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      640 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/angular-ui-select3/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/bootstrap/
--rw-r--r--   0 master    (1000) master    (1000)      641 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/bootstrap/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.659189 burp-ui-1.0.0/burpui/static/vendor/bootstrap/dist/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.707190 burp-ui-1.0.0/burpui/static/vendor/bootstrap/dist/js/
--rw-r--r--   0 master    (1000) master    (1000)    37045 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/bootstrap/dist/js/bootstrap.min.js
--rw-r--r--   0 master    (1000) master    (1000)     2200 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/bootstrap/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/bootstrap-switch/
--rw-r--r--   0 master    (1000) master    (1000)      452 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/bootstrap-switch/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.659189 burp-ui-1.0.0/burpui/static/vendor/bootstrap-switch/dist/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.659189 burp-ui-1.0.0/burpui/static/vendor/bootstrap-switch/dist/css/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.703190 burp-ui-1.0.0/burpui/static/vendor/bootstrap-switch/dist/css/bootstrap3/
--rw-r--r--   0 master    (1000) master    (1000)     5612 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/bootstrap-switch/dist/css/bootstrap3/bootstrap-switch.min.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.707190 burp-ui-1.0.0/burpui/static/vendor/bootstrap-switch/dist/js/
--rw-r--r--   0 master    (1000) master    (1000)    14920 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/bootstrap-switch/dist/js/bootstrap-switch.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.707190 burp-ui-1.0.0/burpui/static/vendor/bootswatch/
--rw-r--r--   0 master    (1000) master    (1000)      830 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/bootswatch/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.707190 burp-ui-1.0.0/burpui/static/vendor/bootswatch/fonts/
--rw-r--r--   0 master    (1000) master    (1000)    20127 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 master    (1000) master    (1000)   108738 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 master    (1000) master    (1000)    45404 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 master    (1000) master    (1000)    23424 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 master    (1000) master    (1000)    18028 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.707190 burp-ui-1.0.0/burpui/static/vendor/bootswatch/slate/
--rw-r--r--   0 master    (1000) master    (1000)   142322 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/bootswatch/slate/bootstrap.min.css
--rw-r--r--   0 master    (1000) master    (1000)     1686 2021-09-17 08:36:04.000000 burp-ui-1.0.0/burpui/static/vendor/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.707190 burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/
--rw-r--r--   0 master    (1000) master    (1000)      399 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.707190 burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/css/
--rw-r--r--   0 master    (1000) master    (1000)    31000 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/fonts/
--rw-r--r--   0 master    (1000) master    (1000)   134808 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 master    (1000) master    (1000)   165742 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 master    (1000) master    (1000)   444379 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 master    (1000) master    (1000)   165548 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 master    (1000) master    (1000)    98024 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 master    (1000) master    (1000)    77160 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 master    (1000) master    (1000)      332 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/d3/
--rw-r--r--   0 master    (1000) master    (1000)      156 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/d3/bower.json
--rw-r--r--   0 master    (1000) master    (1000)   151725 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/d3/d3.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net/
--rw-r--r--   0 master    (1000) master    (1000)      692 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.715190 burp-ui-1.0.0/burpui/static/vendor/datatables.net/js/
--rw-r--r--   0 master    (1000) master    (1000)    81906 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net/js/jquery.dataTables.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-bs/
--rw-r--r--   0 master    (1000) master    (1000)      829 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-bs/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-bs/css/
--rw-r--r--   0 master    (1000) master    (1000)     4188 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-bs/css/dataTables.bootstrap.min.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-bs/js/
--rw-r--r--   0 master    (1000) master    (1000)     1966 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-bs/js/dataTables.bootstrap.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-buttons/
--rw-r--r--   0 master    (1000) master    (1000)      943 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-buttons/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-buttons/js/
--rw-r--r--   0 master    (1000) master    (1000)    17553 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-buttons/js/dataTables.buttons.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-buttons-bs/
--rw-r--r--   0 master    (1000) master    (1000)      960 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-buttons-bs/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-buttons-bs/css/
--rw-r--r--   0 master    (1000) master    (1000)     2867 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-buttons-bs/css/buttons.bootstrap.min.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-buttons-bs/js/
--rw-r--r--   0 master    (1000) master    (1000)      975 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-buttons-bs/js/buttons.bootstrap.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-fixedheader/
--rw-r--r--   0 master    (1000) master    (1000)      761 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-fixedheader/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-fixedheader/js/
--rw-r--r--   0 master    (1000) master    (1000)     6730 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-fixedheader/js/dataTables.fixedHeader.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-fixedheader-bs/
--rw-r--r--   0 master    (1000) master    (1000)      872 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-fixedheader-bs/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-fixedheader-bs/css/
--rw-r--r--   0 master    (1000) master    (1000)      328 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-fixedheader-bs/css/fixedHeader.bootstrap.min.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-responsive/
--rw-r--r--   0 master    (1000) master    (1000)      737 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-responsive/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-responsive/js/
--rw-r--r--   0 master    (1000) master    (1000)    12400 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-responsive/js/dataTables.responsive.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-responsive-bs/
--rw-r--r--   0 master    (1000) master    (1000)      885 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-responsive-bs/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-responsive-bs/css/
--rw-r--r--   0 master    (1000) master    (1000)     3992 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-responsive-bs/css/responsive.bootstrap.min.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-responsive-bs/js/
--rw-r--r--   0 master    (1000) master    (1000)     1246 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-responsive-bs/js/responsive.bootstrap.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.711190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-select/
--rw-r--r--   0 master    (1000) master    (1000)      742 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-select/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.715190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-select/js/
--rw-r--r--   0 master    (1000) master    (1000)    11472 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-select/js/dataTables.select.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.715190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-select-bs/
--rw-r--r--   0 master    (1000) master    (1000)      848 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-select-bs/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.715190 burp-ui-1.0.0/burpui/static/vendor/datatables.net-select-bs/css/
--rw-r--r--   0 master    (1000) master    (1000)     4154 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/datatables.net-select-bs/css/select.bootstrap.min.css
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.715190 burp-ui-1.0.0/burpui/static/vendor/fullcalendar/
--rw-r--r--   0 master    (1000) master    (1000)      853 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/fullcalendar/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.715190 burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/
--rw-r--r--   0 master    (1000) master    (1000)    16066 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.css
--rw-r--r--   0 master    (1000) master    (1000)   213774 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.js
--rw-r--r--   0 master    (1000) master    (1000)     1997 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.print.min.css
--rw-r--r--   0 master    (1000) master    (1000)     4626 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/gcal.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.715190 burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/locale/
--rw-r--r--   0 master    (1000) master    (1000)     3816 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/locale/es.js
--rw-r--r--   0 master    (1000) master    (1000)     3073 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/locale/fr.js
--rw-r--r--   0 master    (1000) master    (1000)     2987 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/locale/it.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.715190 burp-ui-1.0.0/burpui/static/vendor/jquery/
--rw-r--r--   0 master    (1000) master    (1000)      190 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/jquery/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/jquery/dist/
--rw-r--r--   0 master    (1000) master    (1000)    86927 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/jquery/dist/jquery.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.715190 burp-ui-1.0.0/burpui/static/vendor/jquery-file-download/
--rw-r--r--   0 master    (1000) master    (1000)      694 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/jquery-file-download/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      264 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/jquery-file-download/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.663189 burp-ui-1.0.0/burpui/static/vendor/jquery-file-download/src/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.715190 burp-ui-1.0.0/burpui/static/vendor/jquery-file-download/src/Scripts/
--rw-r--r--   0 master    (1000) master    (1000)    19606 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/jquery-file-download/src/Scripts/jquery.fileDownload.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.715190 burp-ui-1.0.0/burpui/static/vendor/jquery-ui/
--rw-r--r--   0 master    (1000) master    (1000)      171 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/jquery-ui/bower.json
--rw-r--r--   0 master    (1000) master    (1000)   253669 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/jquery-ui/jquery-ui.min.js
--rw-r--r--   0 master    (1000) master    (1000)      564 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/jquery-ui/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.715190 burp-ui-1.0.0/burpui/static/vendor/jquery.fancytree/
--rw-r--r--   0 master    (1000) master    (1000)     1009 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/jquery.fancytree/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.715190 burp-ui-1.0.0/burpui/static/vendor/jquery.fancytree/dist/
--rw-r--r--   0 master    (1000) master    (1000)   114799 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/jquery.fancytree/dist/jquery.fancytree-all.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.715190 burp-ui-1.0.0/burpui/static/vendor/jquery.fancytree/dist/skin-bootstrap/
--rw-r--r--   0 master    (1000) master    (1000)    13769 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/jquery.fancytree/dist/skin-bootstrap/ui.fancytree.min.css
--rw-r--r--   0 master    (1000) master    (1000)     1881 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/jquery.fancytree/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/jquery.floatThead/
--rw-r--r--   0 master    (1000) master    (1000)      698 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/jquery.floatThead/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/jquery.floatThead/dist/
--rw-r--r--   0 master    (1000) master    (1000)    13515 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/jquery.floatThead/dist/jquery.floatThead.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/js-cookie/
--rw-r--r--   0 master    (1000) master    (1000)      270 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/js-cookie/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/js-cookie/src/
--rw-r--r--   0 master    (1000) master    (1000)     3886 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/js-cookie/src/js.cookie.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/lodash/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/lodash/dist/
--rw-r--r--   0 master    (1000) master    (1000)    73121 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/lodash/dist/lodash.min.js
--rw-r--r--   0 master    (1000) master    (1000)     2044 2021-09-17 08:35:28.000000 burp-ui-1.0.0/burpui/static/vendor/lodash/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/moment/
--rw-r--r--   0 master    (1000) master    (1000)      442 2021-09-17 08:35:29.000000 burp-ui-1.0.0/burpui/static/vendor/moment/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/moment/locale/
--rw-r--r--   0 master    (1000) master    (1000)     3449 2021-09-17 08:35:29.000000 burp-ui-1.0.0/burpui/static/vendor/moment/locale/es.js
--rw-r--r--   0 master    (1000) master    (1000)     2703 2021-09-17 08:35:29.000000 burp-ui-1.0.0/burpui/static/vendor/moment/locale/fr.js
--rw-r--r--   0 master    (1000) master    (1000)     2157 2021-09-17 08:35:29.000000 burp-ui-1.0.0/burpui/static/vendor/moment/locale/it.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/moment/min/
--rw-r--r--   0 master    (1000) master    (1000)    51654 2021-09-17 08:35:29.000000 burp-ui-1.0.0/burpui/static/vendor/moment/min/moment.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/moment-timezone/
--rw-r--r--   0 master    (1000) master    (1000)      395 2021-09-17 08:35:29.000000 burp-ui-1.0.0/burpui/static/vendor/moment-timezone/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/moment-timezone/builds/
--rw-r--r--   0 master    (1000) master    (1000)    42530 2021-09-17 08:35:29.000000 burp-ui-1.0.0/burpui/static/vendor/moment-timezone/builds/moment-timezone-with-data-10-year-range.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/nvd3/
--rw-r--r--   0 master    (1000) master    (1000)      643 2021-09-17 08:35:29.000000 burp-ui-1.0.0/burpui/static/vendor/nvd3/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/nvd3/build/
--rw-r--r--   0 master    (1000) master    (1000)     8419 2021-09-17 08:35:29.000000 burp-ui-1.0.0/burpui/static/vendor/nvd3/build/nv.d3.min.css
--rw-r--r--   0 master    (1000) master    (1000)   253352 2021-09-17 08:35:29.000000 burp-ui-1.0.0/burpui/static/vendor/nvd3/build/nv.d3.min.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/select2/
--rw-r--r--   0 master    (1000) master    (1000)      206 2021-09-17 08:35:29.000000 burp-ui-1.0.0/burpui/static/vendor/select2/bower.json
--rw-r--r--   0 master    (1000) master    (1000)      678 2021-09-17 08:35:29.000000 burp-ui-1.0.0/burpui/static/vendor/select2/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/socket.io-client/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/socket.io-client/dist/
--rw-r--r--   0 master    (1000) master    (1000)    61701 2021-09-17 08:36:04.000000 burp-ui-1.0.0/burpui/static/vendor/socket.io-client/dist/socket.io.min.js
--rw-r--r--   0 master    (1000) master    (1000)     3098 2021-09-17 08:36:04.000000 burp-ui-1.0.0/burpui/static/vendor/socket.io-client/package.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.719190 burp-ui-1.0.0/burpui/static/vendor/typeahead.js/
--rw-r--r--   0 master    (1000) master    (1000)      247 2021-09-17 08:35:29.000000 burp-ui-1.0.0/burpui/static/vendor/typeahead.js/bower.json
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.723190 burp-ui-1.0.0/burpui/static/vendor/typeahead.js/dist/
--rw-r--r--   0 master    (1000) master    (1000)    26900 2021-09-17 08:35:29.000000 burp-ui-1.0.0/burpui/static/vendor/typeahead.js/dist/typeahead.jquery.min.js
--rw-r--r--   0 master    (1000) master    (1000)     1801 2021-09-17 08:35:29.000000 burp-ui-1.0.0/burpui/static/vendor/typeahead.js/package.json
--rw-r--r--   0 master    (1000) master    (1000)    12285 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/tasks.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.723190 burp-ui-1.0.0/burpui/templates/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.727190 burp-ui-1.0.0/burpui/templates/.ropeproject/
--rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-02 15:12:13.000000 burp-ui-1.0.0/burpui/templates/.ropeproject/config.py
--rw-r--r--   0 master    (1000) master    (1000)        6 2019-10-02 15:12:13.000000 burp-ui-1.0.0/burpui/templates/.ropeproject/globalnames
--rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-02 15:12:13.000000 burp-ui-1.0.0/burpui/templates/.ropeproject/history
--rw-r--r--   0 master    (1000) master    (1000)        6 2019-10-02 15:12:13.000000 burp-ui-1.0.0/burpui/templates/.ropeproject/objectdb
--rw-r--r--   0 master    (1000) master    (1000)     1162 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/about.html
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.727190 burp-ui-1.0.0/burpui/templates/admin/
--rw-r--r--   0 master    (1000) master    (1000)     1780 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/admin/authentication.html
--rw-r--r--   0 master    (1000) master    (1000)     3045 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/admin/grant-authorization.html
--rw-r--r--   0 master    (1000) master    (1000)     3989 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/admin/group-authorization.html
--rw-r--r--   0 master    (1000) master    (1000)     2722 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/admin/sessions.html
--rw-r--r--   0 master    (1000) master    (1000)     7776 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/admin-authentications.html
--rw-r--r--   0 master    (1000) master    (1000)    13642 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/admin-authorizations.html
--rw-r--r--   0 master    (1000) master    (1000)     1846 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/admin-backends.html
--rw-r--r--   0 master    (1000) master    (1000)     4195 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/backup-report.html
--rw-r--r--   0 master    (1000) master    (1000)     1158 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/calendar.html
--rw-r--r--   0 master    (1000) master    (1000)    11932 2019-11-04 21:35:27.000000 burp-ui-1.0.0/burpui/templates/client-browse.html
--rw-r--r--   0 master    (1000) master    (1000)     3121 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/client-report.html
--rw-r--r--   0 master    (1000) master    (1000)     4686 2019-11-04 21:35:27.000000 burp-ui-1.0.0/burpui/templates/client.html
--rw-r--r--   0 master    (1000) master    (1000)     3588 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/clients-report.html
--rw-r--r--   0 master    (1000) master    (1000)     1402 2020-10-16 20:22:41.000000 burp-ui-1.0.0/burpui/templates/clients.html
--rw-r--r--   0 master    (1000) master    (1000)    14377 2020-10-16 20:22:41.000000 burp-ui-1.0.0/burpui/templates/gerard.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.731190 burp-ui-1.0.0/burpui/templates/js/
--rw-r--r--   0 master    (1000) master    (1000)      743 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/js/about.js
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.731190 burp-ui-1.0.0/burpui/templates/js/admin/
--rw-r--r--   0 master    (1000) master    (1000)     1116 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/js/admin/authentication.js
--rw-r--r--   0 master    (1000) master    (1000)     3860 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/js/admin/grant-authorization.js
--rw-r--r--   0 master    (1000) master    (1000)     7738 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/js/admin/group-authorization.js
--rw-r--r--   0 master    (1000) master    (1000)     8347 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/templates/js/admin/sessions.js
--rw-r--r--   0 master    (1000) master    (1000)     9009 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/js/admin-authentications.js
--rw-r--r--   0 master    (1000) master    (1000)    30828 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/js/admin-authorizations.js
--rw-r--r--   0 master    (1000) master    (1000)     3896 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/js/admin-backends.js
--rw-r--r--   0 master    (1000) master    (1000)     2926 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/js/backup-report.js
--rw-r--r--   0 master    (1000) master    (1000)     1680 2020-10-16 20:22:41.000000 burp-ui-1.0.0/burpui/templates/js/calendar.js
--rw-r--r--   0 master    (1000) master    (1000)    13073 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/templates/js/client-browse.js
--rw-r--r--   0 master    (1000) master    (1000)     5127 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/templates/js/client-report.js
--rw-r--r--   0 master    (1000) master    (1000)    10240 2020-10-16 20:22:41.000000 burp-ui-1.0.0/burpui/templates/js/client.js
--rw-r--r--   0 master    (1000) master    (1000)     2643 2019-11-04 21:35:27.000000 burp-ui-1.0.0/burpui/templates/js/clients-report.js
--rw-r--r--   0 master    (1000) master    (1000)     7921 2020-10-16 20:22:41.000000 burp-ui-1.0.0/burpui/templates/js/clients.js
--rw-r--r--   0 master    (1000) master    (1000)     2470 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/js/live-monitor.js
--rw-r--r--   0 master    (1000) master    (1000)     2084 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/js/servers-report.js
--rw-r--r--   0 master    (1000) master    (1000)     1782 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/js/servers.js
--rw-r--r--   0 master    (1000) master    (1000)    27017 2019-11-04 21:35:27.000000 burp-ui-1.0.0/burpui/templates/js/settings.js
--rw-r--r--   0 master    (1000) master    (1000)    20380 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/templates/js/user.js
--rw-r--r--   0 master    (1000) master    (1000)      347 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/js/websocket.js
--rw-r--r--   0 master    (1000) master    (1000)     9972 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/templates/layout.html
--rw-r--r--   0 master    (1000) master    (1000)     4937 2019-11-04 21:35:27.000000 burp-ui-1.0.0/burpui/templates/live-monitor.html
--rw-r--r--   0 master    (1000) master    (1000)      735 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/login.html
--rw-r--r--   0 master    (1000) master    (1000)    16144 2020-10-16 20:22:41.000000 burp-ui-1.0.0/burpui/templates/macros.html
--rw-r--r--   0 master    (1000) master    (1000)     1346 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/notifications.html
--rw-r--r--   0 master    (1000) master    (1000)     1776 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/servers-report.html
--rw-r--r--   0 master    (1000) master    (1000)      923 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/templates/servers.html
--rw-r--r--   0 master    (1000) master    (1000)    40891 2019-11-04 21:35:27.000000 burp-ui-1.0.0/burpui/templates/settings.html
--rw-r--r--   0 master    (1000) master    (1000)      861 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/sideadmin.html
--rw-r--r--   0 master    (1000) master    (1000)     2870 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/sidebar.html
--rw-r--r--   0 master    (1000) master    (1000)     1490 2019-11-04 21:35:27.000000 burp-ui-1.0.0/burpui/templates/sideconfig.html
--rw-r--r--   0 master    (1000) master    (1000)      830 2019-11-04 21:35:27.000000 burp-ui-1.0.0/burpui/templates/sideuser.html
--rw-r--r--   0 master    (1000) master    (1000)     3767 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/small_topbar.html
--rw-r--r--   0 master    (1000) master    (1000)     4572 2018-08-18 00:27:08.000000 burp-ui-1.0.0/burpui/templates/topbar.html
--rw-r--r--   0 master    (1000) master    (1000)    10122 2020-10-16 20:22:41.000000 burp-ui-1.0.0/burpui/templates/user.html
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.731190 burp-ui-1.0.0/burpui/thirdparty/
--rw-r--r--   0 master    (1000) master    (1000)    24832 2021-09-17 23:27:12.000000 burp-ui-1.0.0/burpui/thirdparty/flask_bower.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.731190 burp-ui-1.0.0/burpui/tools/
--rw-r--r--   0 master    (1000) master    (1000)     3289 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/tools/logging.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.667189 burp-ui-1.0.0/burpui/translations/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.667189 burp-ui-1.0.0/burpui/translations/es/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.731190 burp-ui-1.0.0/burpui/translations/es/LC_MESSAGES/
--rw-r--r--   0 master    (1000) master    (1000)    60903 2022-11-06 20:40:36.000000 burp-ui-1.0.0/burpui/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 master    (1000) master    (1000)   102166 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.667189 burp-ui-1.0.0/burpui/translations/fr/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.731190 burp-ui-1.0.0/burpui/translations/fr/LC_MESSAGES/
--rw-r--r--   0 master    (1000) master    (1000)    24327 2022-11-06 20:40:37.000000 burp-ui-1.0.0/burpui/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 master    (1000) master    (1000)    80323 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.667189 burp-ui-1.0.0/burpui/translations/it/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.731190 burp-ui-1.0.0/burpui/translations/it/LC_MESSAGES/
--rw-r--r--   0 master    (1000) master    (1000)    56806 2022-11-06 20:40:36.000000 burp-ui-1.0.0/burpui/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 master    (1000) master    (1000)    97706 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/translations/it/LC_MESSAGES/messages.po
--rw-r--r--   0 master    (1000) master    (1000)     8183 2021-09-17 23:27:12.000000 burp-ui-1.0.0/burpui/utils.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.731190 burp-ui-1.0.0/burpui/ws/
--rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.0.0/burpui/ws/__init__.py
--rw-r--r--   0 master    (1000) master    (1000)      927 2021-09-17 12:05:45.000000 burp-ui-1.0.0/burpui/ws/namespace.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.667189 burp-ui-1.0.0/contrib/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.731190 burp-ui-1.0.0/contrib/centos/
--rwxr-xr-x   0 master    (1000) master    (1000)     1595 2017-04-28 13:40:18.000000 burp-ui-1.0.0/contrib/centos/init.sh
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.731190 burp-ui-1.0.0/contrib/freebsd/
--rw-r--r--   0 master    (1000) master    (1000)      602 2018-05-14 12:28:49.000000 burp-ui-1.0.0/contrib/freebsd/gunicorn.rc
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.731190 burp-ui-1.0.0/contrib/gunicorn/
--rw-r--r--   0 master    (1000) master    (1000)     6080 2021-09-17 12:05:45.000000 burp-ui-1.0.0/contrib/gunicorn/burpui_gunicorn.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.731190 burp-ui-1.0.0/contrib/systemd/
--rw-r--r--   0 master    (1000) master    (1000)      171 2017-05-09 16:54:39.000000 burp-ui-1.0.0/contrib/systemd/bui-agent.service
--rw-r--r--   0 master    (1000) master    (1000)      337 2019-11-04 21:35:27.000000 burp-ui-1.0.0/contrib/systemd/bui-celery-beat.service
--rw-r--r--   0 master    (1000) master    (1000)      191 2019-11-04 21:35:27.000000 burp-ui-1.0.0/contrib/systemd/bui-celery.service
--rw-r--r--   0 master    (1000) master    (1000)      299 2017-05-09 16:54:39.000000 burp-ui-1.0.0/contrib/systemd/bui-gunicorn.service
--rw-r--r--   0 master    (1000) master    (1000)      253 2019-11-04 21:35:27.000000 burp-ui-1.0.0/contrib/systemd/bui-monitor.service
--rw-r--r--   0 master    (1000) master    (1000)      188 2018-05-14 12:28:49.000000 burp-ui-1.0.0/contrib/systemd/bui-websocket.service
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.735190 burp-ui-1.0.0/migrations/
--rwxr-xr-x   0 master    (1000) master    (1000)       39 2021-09-17 12:05:45.000000 burp-ui-1.0.0/migrations/README
--rw-r--r--   0 master    (1000) master    (1000)      770 2017-04-28 13:40:18.000000 burp-ui-1.0.0/migrations/alembic.ini
--rwxr-xr-x   0 master    (1000) master    (1000)     2917 2021-09-17 12:05:45.000000 burp-ui-1.0.0/migrations/env.py
--rwxr-xr-x   0 master    (1000) master    (1000)      412 2017-04-28 13:40:18.000000 burp-ui-1.0.0/migrations/script.py.mako
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.735190 burp-ui-1.0.0/migrations/versions/
--rw-r--r--   0 master    (1000) master    (1000)      980 2021-09-17 12:05:45.000000 burp-ui-1.0.0/migrations/versions/225d9b2f0fb1_initial.py
--rw-r--r--   0 master    (1000) master    (1000)      875 2021-09-17 12:05:45.000000 burp-ui-1.0.0/migrations/versions/4445080944ee_hidden_hosts_management.py
--rw-r--r--   0 master    (1000) master    (1000)      844 2021-09-17 12:05:45.000000 burp-ui-1.0.0/migrations/versions/56de018f4d88_user_prefs.py
--rw-r--r--   0 master    (1000) master    (1000)      983 2021-09-17 12:05:45.000000 burp-ui-1.0.0/migrations/versions/695dcbd29d4f_increase_pref_value_size.py
--rw-r--r--   0 master    (1000) master    (1000)     1190 2021-09-17 12:05:45.000000 burp-ui-1.0.0/migrations/versions/7f317474332d_handle_sessions.py
--rw-r--r--   0 master    (1000) master    (1000)     3244 2021-09-17 12:05:45.000000 burp-ui-1.0.0/migrations/versions/fc07e3fa0086_sql_compatibility.py
--rw-r--r--   0 master    (1000) master    (1000)      224 2021-09-17 12:05:45.000000 burp-ui-1.0.0/pyproject.toml
--rw-r--r--   0 master    (1000) master    (1000)      291 2022-11-06 13:19:11.000000 burp-ui-1.0.0/requirements.txt
--rw-r--r--   0 master    (1000) master    (1000)      503 2022-11-06 20:40:37.735190 burp-ui-1.0.0/setup.cfg
--rwxr-xr-x   0 master    (1000) master    (1000)    14196 2022-11-06 19:38:06.000000 burp-ui-1.0.0/setup.py
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.671189 burp-ui-1.0.0/share/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.671189 burp-ui-1.0.0/share/burpui/
-drwxr-xr-x   0 master    (1000) master    (1000)        0 2022-11-06 20:40:37.735190 burp-ui-1.0.0/share/burpui/etc/
--rw-r--r--   0 master    (1000) master    (1000)      772 2019-11-04 21:35:27.000000 burp-ui-1.0.0/share/burpui/etc/buimonitor.sample.cfg
--rw-r--r--   0 master    (1000) master    (1000)    15828 2021-10-06 15:22:17.000000 burp-ui-1.0.0/share/burpui/etc/burpui.sample.cfg
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.148662 burp-ui-1.1.0/
+-rw-r--r--   0 master    (1000) master    (1000)    22785 2023-05-01 19:11:44.000000 burp-ui-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 master    (1000) master    (1000)      368 2022-11-06 21:20:42.000000 burp-ui-1.1.0/CONTRIBUTORS
+-rw-r--r--   0 master    (1000) master    (1000)     1575 2018-05-14 12:28:48.000000 burp-ui-1.1.0/LICENSE
+-rw-r--r--   0 master    (1000) master    (1000)      342 2022-11-06 21:20:42.000000 burp-ui-1.1.0/MANIFEST.in
+-rw-r--r--   0 master    (1000) master    (1000)     5873 2023-05-01 19:13:30.148662 burp-ui-1.1.0/PKG-INFO
+-rw-r--r--   0 master    (1000) master    (1000)     5025 2022-11-06 21:20:42.000000 burp-ui-1.1.0/README.rst
+-rw-r--r--   0 master    (1000) master    (1000)      229 2017-04-28 13:40:18.000000 burp-ui-1.1.0/babel.cfg
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/burp_ui.egg-info/
+-rw-r--r--   0 master    (1000) master    (1000)     5873 2023-05-01 19:13:30.000000 burp-ui-1.1.0/burp_ui.egg-info/PKG-INFO
+-rw-r--r--   0 master    (1000) master    (1000)    15086 2023-05-01 19:13:30.000000 burp-ui-1.1.0/burp_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 master    (1000) master    (1000)        1 2023-05-01 19:13:30.000000 burp-ui-1.1.0/burp_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 master    (1000) master    (1000)      243 2023-05-01 19:13:30.000000 burp-ui-1.1.0/burp_ui.egg-info/entry_points.txt
+-rw-r--r--   0 master    (1000) master    (1000)      755 2023-05-01 19:13:30.000000 burp-ui-1.1.0/burp_ui.egg-info/requires.txt
+-rw-r--r--   0 master    (1000) master    (1000)        7 2023-05-01 19:13:30.000000 burp-ui-1.1.0/burp_ui.egg-info/top_level.txt
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.100661 burp-ui-1.1.0/burpui/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.100661 burp-ui-1.1.0/burpui/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)    12191 2019-10-03 09:41:02.000000 burp-ui-1.1.0/burpui/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2018-06-05 15:54:46.000000 burp-ui-1.1.0/burpui/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)      779 2019-10-03 09:41:02.000000 burp-ui-1.1.0/burpui/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.000000 burp-ui-1.1.0/burpui/RELEASE
+-rw-r--r--   0 master    (1000) master    (1000)        6 2023-05-01 19:11:44.000000 burp-ui-1.1.0/burpui/VERSION
+-rw-r--r--   0 master    (1000) master    (1000)      382 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)     9535 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/__main__.py
+-rw-r--r--   0 master    (1000) master    (1000)      249 2021-05-12 15:45:53.000000 burp-ui-1.1.0/burpui/_cli.py
+-rw-r--r--   0 master    (1000) master    (1000)     2058 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/_compat.py
+-rw-r--r--   0 master    (1000) master    (1000)     1202 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/_json.py
+-rw-r--r--   0 master    (1000) master    (1000)      397 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/_rtfd.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.104661 burp-ui-1.1.0/burpui/api/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.104661 burp-ui-1.1.0/burpui/api/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4794 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/api/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)     2643 2018-09-14 14:17:22.000000 burp-ui-1.1.0/burpui/api/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-23 14:42:15.000000 burp-ui-1.1.0/burpui/api/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2018-09-14 14:17:22.000000 burp-ui-1.1.0/burpui/api/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)     8428 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    60894 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/admin.py
+-rw-r--r--   0 master    (1000) master    (1000)     4961 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/backup.py
+-rw-r--r--   0 master    (1000) master    (1000)    36404 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/client.py
+-rw-r--r--   0 master    (1000) master    (1000)    25725 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/clients.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.104661 burp-ui-1.1.0/burpui/api/custom/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.104661 burp-ui-1.1.0/burpui/api/custom/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-01 14:25:10.000000 burp-ui-1.1.0/burpui/api/custom/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)      291 2019-10-01 14:25:10.000000 burp-ui-1.1.0/burpui/api/custom/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-01 14:25:10.000000 burp-ui-1.1.0/burpui/api/custom/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2019-10-01 14:25:10.000000 burp-ui-1.1.0/burpui/api/custom/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)      213 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/api/custom/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)      585 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/custom/fields.py
+-rw-r--r--   0 master    (1000) master    (1000)     2860 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/custom/my_fields.py
+-rw-r--r--   0 master    (1000) master    (1000)     1430 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/api/custom/resource.py
+-rw-r--r--   0 master    (1000) master    (1000)    35378 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/misc.py
+-rw-r--r--   0 master    (1000) master    (1000)     8585 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/prefs.py
+-rw-r--r--   0 master    (1000) master    (1000)    17608 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/restore.py
+-rw-r--r--   0 master    (1000) master    (1000)     8028 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/servers.py
+-rw-r--r--   0 master    (1000) master    (1000)    35800 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/settings.py
+-rw-r--r--   0 master    (1000) master    (1000)    32795 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/api/tasks.py
+-rw-r--r--   0 master    (1000) master    (1000)    15706 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/app.py
+-rw-r--r--   0 master    (1000) master    (1000)    16384 2017-07-26 14:40:04.000000 burp-ui-1.1.0/burpui/celerybeat-schedule
+-rw-r--r--   0 master    (1000) master    (1000)    45118 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/cli.py
+-rw-r--r--   0 master    (1000) master    (1000)    10045 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/config.py
+-rw-r--r--   0 master    (1000) master    (1000)    23767 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/datastructures.py
+-rw-r--r--   0 master    (1000) master    (1000)     2768 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/decorators.py
+-rw-r--r--   0 master    (1000) master    (1000)      964 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/desc.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.104661 burp-ui-1.1.0/burpui/engines/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/engines/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    14171 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/engines/agent.py
+-rw-r--r--   0 master    (1000) master    (1000)    11302 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/engines/monitor.py
+-rw-r--r--   0 master    (1000) master    (1000)    17914 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/engines/server.py
+-rw-r--r--   0 master    (1000) master    (1000)      943 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/engines/worker.py
+-rw-r--r--   0 master    (1000) master    (1000)      871 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/exceptions.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.104661 burp-ui-1.1.0/burpui/ext/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/ext/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)      371 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/ext/cache.py
+-rw-r--r--   0 master    (1000) master    (1000)      926 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/ext/i18n.py
+-rw-r--r--   0 master    (1000) master    (1000)      309 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/ext/limit.py
+-rw-r--r--   0 master    (1000) master    (1000)      233 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/ext/session.py
+-rw-r--r--   0 master    (1000) master    (1000)      232 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/ext/sql.py
+-rw-r--r--   0 master    (1000) master    (1000)      230 2019-04-02 19:43:50.000000 burp-ui-1.1.0/burpui/ext/tasks.py
+-rw-r--r--   0 master    (1000) master    (1000)      545 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/ext/ws.py
+-rw-r--r--   0 master    (1000) master    (1000)    11897 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/extensions.py
+-rw-r--r--   0 master    (1000) master    (1000)     3524 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/filter.py
+-rw-r--r--   0 master    (1000) master    (1000)      728 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/forms.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.104661 burp-ui-1.1.0/burpui/misc/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.108661 burp-ui-1.1.0/burpui/misc/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4794 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)     2452 2018-07-23 07:59:35.000000 burp-ui-1.1.0/burpui/misc/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-20 15:54:46.000000 burp-ui-1.1.0/burpui/misc/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2018-07-23 07:59:35.000000 burp-ui-1.1.0/burpui/misc/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/__init__.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.108661 burp-ui-1.1.0/burpui/misc/acl/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.108661 burp-ui-1.1.0/burpui/misc/acl/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4794 2019-09-24 13:37:49.000000 burp-ui-1.1.0/burpui/misc/acl/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)      346 2019-09-27 12:40:13.000000 burp-ui-1.1.0/burpui/misc/acl/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2019-09-25 20:15:11.000000 burp-ui-1.1.0/burpui/misc/acl/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2019-09-27 12:40:13.000000 burp-ui-1.1.0/burpui/misc/acl/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/acl/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    14445 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/acl/basic.py
+-rw-r--r--   0 master    (1000) master    (1000)     5655 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/acl/handler.py
+-rw-r--r--   0 master    (1000) master    (1000)     5389 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/acl/interface.py
+-rw-r--r--   0 master    (1000) master    (1000)    28562 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/acl/meta.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.108661 burp-ui-1.1.0/burpui/misc/audit/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.108661 burp-ui-1.1.0/burpui/misc/audit/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/audit/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)      138 2018-08-03 09:24:44.000000 burp-ui-1.1.0/burpui/misc/audit/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2018-06-05 13:59:15.000000 burp-ui-1.1.0/burpui/misc/audit/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)       27 2018-08-03 09:24:44.000000 burp-ui-1.1.0/burpui/misc/audit/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/misc/audit/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)     2804 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/audit/basic.py
+-rw-r--r--   0 master    (1000) master    (1000)     3591 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/audit/handler.py
+-rw-r--r--   0 master    (1000) master    (1000)     1854 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/audit/interface.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.108661 burp-ui-1.1.0/burpui/misc/auth/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.108661 burp-ui-1.1.0/burpui/misc/auth/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/auth/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)      763 2019-01-29 14:01:08.000000 burp-ui-1.1.0/burpui/misc/auth/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2018-06-07 15:21:13.000000 burp-ui-1.1.0/burpui/misc/auth/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)     2077 2019-01-29 14:01:08.000000 burp-ui-1.1.0/burpui/misc/auth/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/auth/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)     9656 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/auth/basic.py
+-rw-r--r--   0 master    (1000) master    (1000)    10821 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/auth/handler.py
+-rw-r--r--   0 master    (1000) master    (1000)     3489 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/auth/interface.py
+-rw-r--r--   0 master    (1000) master    (1000)    11181 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/auth/ldap.py
+-rw-r--r--   0 master    (1000) master    (1000)     4675 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/auth/local.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/misc/backend/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/misc/backend/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4829 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/backend/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)     1168 2020-05-08 22:06:12.000000 burp-ui-1.1.0/burpui/misc/backend/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2018-07-18 09:19:37.000000 burp-ui-1.1.0/burpui/misc/backend/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2020-05-08 22:06:12.000000 burp-ui-1.1.0/burpui/misc/backend/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/backend/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    47346 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/backend/burp1.py
+-rw-r--r--   0 master    (1000) master    (1000)    30620 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/backend/burp2.py
+-rw-r--r--   0 master    (1000) master    (1000)    41267 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/backend/interface.py
+-rw-r--r--   0 master    (1000) master    (1000)    23472 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/backend/multi.py
+-rw-r--r--   0 master    (1000) master    (1000)    38354 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/backend/parallel.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/misc/backend/utils/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/misc/backend/utils/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    12735 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/backend/utils/burp2.py
+-rw-r--r--   0 master    (1000) master    (1000)      398 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/misc/backend/utils/constant.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/misc/parser/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/misc/parser/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-01 12:38:25.000000 burp-ui-1.1.0/burpui/misc/parser/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)      431 2021-10-04 08:39:12.000000 burp-ui-1.1.0/burpui/misc/parser/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-03 09:34:38.000000 burp-ui-1.1.0/burpui/misc/parser/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2021-10-04 08:39:12.000000 burp-ui-1.1.0/burpui/misc/parser/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/misc/parser/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)    37464 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/parser/burp1.py
+-rw-r--r--   0 master    (1000) master    (1000)    13883 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/parser/burp2.py
+-rw-r--r--   0 master    (1000) master    (1000)    43592 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/misc/parser/doc.py
+-rw-r--r--   0 master    (1000) master    (1000)    17679 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/misc/parser/interface.py
+-rw-r--r--   0 master    (1000) master    (1000)     8075 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/parser/openssl.py
+-rw-r--r--   0 master    (1000) master    (1000)    57165 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/misc/parser/utils.py
+-rw-r--r--   0 master    (1000) master    (1000)     3399 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/models.py
+-rw-r--r--   0 master    (1000) master    (1000)     2642 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/plugins.py
+-rw-r--r--   0 master    (1000) master    (1000)    17427 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/routes.py
+-rw-r--r--   0 master    (1000) master    (1000)     2913 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/security.py
+-rw-r--r--   0 master    (1000) master    (1000)    11088 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/sessions.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/static/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.088661 burp-ui-1.1.0/burpui/static/3rdparty/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/static/3rdparty/highlightjs/
+-rw-r--r--   0 master    (1000) master    (1000)     8711 2018-05-14 12:28:49.000000 burp-ui-1.1.0/burpui/static/3rdparty/highlightjs/highlight.pack.js
+-rw-r--r--   0 master    (1000) master    (1000)     1211 2018-05-14 12:28:49.000000 burp-ui-1.1.0/burpui/static/3rdparty/highlightjs/style.css
+-rw-r--r--   0 master    (1000) master    (1000)     7298 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/static/dashboard.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.088661 burp-ui-1.1.0/burpui/static/extra/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.112661 burp-ui-1.1.0/burpui/static/extra/i18n/
+-rw-r--r--   0 master    (1000) master    (1000)      885 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/static/extra/i18n/datatable-es.json
+-rw-r--r--   0 master    (1000) master    (1000)      990 2017-04-28 13:40:18.000000 burp-ui-1.1.0/burpui/static/extra/i18n/datatable-fr.json
+-rw-r--r--   0 master    (1000) master    (1000)      818 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/static/extra/i18n/datatable-it.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/images/
+-rw-r--r--   0 master    (1000) master    (1000)     1150 2017-04-28 13:40:18.000000 burp-ui-1.1.0/burpui/static/images/favicon.ico
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/ace-builds/
+-rw-r--r--   0 master    (1000) master    (1000)      517 2021-09-17 08:35:27.000000 burp-ui-1.1.0/burpui/static/vendor/ace-builds/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      545 2021-09-17 08:35:27.000000 burp-ui-1.1.0/burpui/static/vendor/ace-builds/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/
+-rw-r--r--   0 master    (1000) master    (1000)   358296 2021-09-17 08:35:27.000000 burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/ace.js
+-rw-r--r--   0 master    (1000) master    (1000)     5505 2021-09-17 08:35:27.000000 burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/mode-json.js
+-rw-r--r--   0 master    (1000) master    (1000)    27789 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/theme-ambiance.js
+-rw-r--r--   0 master    (1000) master    (1000)    32966 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/worker-json.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular/
+-rw-r--r--   0 master    (1000) master    (1000)   169920 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular/angular.min.js
+-rw-r--r--   0 master    (1000) master    (1000)      133 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      572 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular-animate/
+-rw-r--r--   0 master    (1000) master    (1000)    25733 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-animate/angular-animate.min.js
+-rw-r--r--   0 master    (1000) master    (1000)      172 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-animate/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      702 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-animate/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/
+-rw-r--r--   0 master    (1000) master    (1000)      460 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      569 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/package.json
+-rw-r--r--   0 master    (1000) master    (1000)   125728 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/ui-bootstrap-tpls.min.js
+-rw-r--r--   0 master    (1000) master    (1000)   103577 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/ui-bootstrap.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/
+-rw-r--r--   0 master    (1000) master    (1000)      799 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/dist/
+-rw-r--r--   0 master    (1000) master    (1000)     3139 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/dist/angular-bootstrap-switch.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     1228 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/
+-rw-r--r--   0 master    (1000) master    (1000)     1720 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    14421 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/dist/angular-datatables.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     1846 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.116661 burp-ui-1.1.0/burpui/static/vendor/angular-highlightjs/
+-rw-r--r--   0 master    (1000) master    (1000)      457 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-highlightjs/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-highlightjs/build/
+-rw-r--r--   0 master    (1000) master    (1000)     4707 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-highlightjs/build/angular-highlightjs.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-onbeforeunload/
+-rw-r--r--   0 master    (1000) master    (1000)      678 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-onbeforeunload/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-onbeforeunload/build/
+-rw-r--r--   0 master    (1000) master    (1000)      906 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-onbeforeunload/build/angular-onbeforeunload.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-resource/
+-rw-r--r--   0 master    (1000) master    (1000)     4508 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-resource/angular-resource.min.js
+-rw-r--r--   0 master    (1000) master    (1000)      174 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-resource/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      738 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-resource/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-route/
+-rw-r--r--   0 master    (1000) master    (1000)     5611 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-route/angular-route.min.js
+-rw-r--r--   0 master    (1000) master    (1000)      168 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-route/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      687 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-route/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-sanitize/
+-rw-r--r--   0 master    (1000) master    (1000)     6612 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-sanitize/angular-sanitize.min.js
+-rw-r--r--   0 master    (1000) master    (1000)      174 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-sanitize/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      704 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-sanitize/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-strap/
+-rw-r--r--   0 master    (1000) master    (1000)     1268 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-strap/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-strap/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    83061 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-strap/dist/angular-strap.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     9858 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-strap/dist/angular-strap.tpl.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     1756 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-strap/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-ui-calendar/
+-rw-r--r--   0 master    (1000) master    (1000)      739 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-calendar/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-ui-calendar/src/
+-rw-r--r--   0 master    (1000) master    (1000)    16233 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-calendar/src/calendar.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/
+-rw-r--r--   0 master    (1000) master    (1000)      574 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/dist/
+-rw-r--r--   0 master    (1000) master    (1000)     6092 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/dist/select.min.css
+-rw-r--r--   0 master    (1000) master    (1000)    45235 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/dist/select.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     1738 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select3/
+-rw-r--r--   0 master    (1000) master    (1000)      374 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select3/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      640 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/angular-ui-select3/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/bootstrap/
+-rw-r--r--   0 master    (1000) master    (1000)      641 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootstrap/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.088661 burp-ui-1.1.0/burpui/static/vendor/bootstrap/dist/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/bootstrap/dist/js/
+-rw-r--r--   0 master    (1000) master    (1000)    37045 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootstrap/dist/js/bootstrap.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     2200 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootstrap/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/
+-rw-r--r--   0 master    (1000) master    (1000)      452 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.088661 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.088661 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/css/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/css/bootstrap3/
+-rw-r--r--   0 master    (1000) master    (1000)     5612 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/css/bootstrap3/bootstrap-switch.min.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/js/
+-rw-r--r--   0 master    (1000) master    (1000)    14920 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/js/bootstrap-switch.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.120661 burp-ui-1.1.0/burpui/static/vendor/bootswatch/
+-rw-r--r--   0 master    (1000) master    (1000)      830 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootswatch/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.124662 burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/
+-rw-r--r--   0 master    (1000) master    (1000)    20127 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 master    (1000) master    (1000)   108738 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 master    (1000) master    (1000)    45404 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 master    (1000) master    (1000)    23424 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 master    (1000) master    (1000)    18028 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.124662 burp-ui-1.1.0/burpui/static/vendor/bootswatch/slate/
+-rw-r--r--   0 master    (1000) master    (1000)   142322 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/bootswatch/slate/bootstrap.min.css
+-rw-r--r--   0 master    (1000) master    (1000)     1686 2021-09-17 08:36:04.000000 burp-ui-1.1.0/burpui/static/vendor/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.124662 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/
+-rw-r--r--   0 master    (1000) master    (1000)      399 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.124662 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/css/
+-rw-r--r--   0 master    (1000) master    (1000)    31000 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.124662 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/
+-rw-r--r--   0 master    (1000) master    (1000)   134808 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 master    (1000) master    (1000)   165742 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 master    (1000) master    (1000)   444379 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 master    (1000) master    (1000)   165548 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 master    (1000) master    (1000)    98024 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 master    (1000) master    (1000)    77160 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 master    (1000) master    (1000)      332 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.124662 burp-ui-1.1.0/burpui/static/vendor/d3/
+-rw-r--r--   0 master    (1000) master    (1000)      156 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/d3/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)   151725 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/d3/d3.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.124662 burp-ui-1.1.0/burpui/static/vendor/datatables.net/
+-rw-r--r--   0 master    (1000) master    (1000)      692 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net/js/
+-rw-r--r--   0 master    (1000) master    (1000)    81906 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net/js/jquery.dataTables.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/
+-rw-r--r--   0 master    (1000) master    (1000)      829 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/css/
+-rw-r--r--   0 master    (1000) master    (1000)     4188 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/css/dataTables.bootstrap.min.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/js/
+-rw-r--r--   0 master    (1000) master    (1000)     1966 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/js/dataTables.bootstrap.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons/
+-rw-r--r--   0 master    (1000) master    (1000)      943 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons/js/
+-rw-r--r--   0 master    (1000) master    (1000)    17553 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons/js/dataTables.buttons.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/
+-rw-r--r--   0 master    (1000) master    (1000)      960 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/css/
+-rw-r--r--   0 master    (1000) master    (1000)     2867 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/css/buttons.bootstrap.min.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/js/
+-rw-r--r--   0 master    (1000) master    (1000)      975 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/js/buttons.bootstrap.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader/
+-rw-r--r--   0 master    (1000) master    (1000)      761 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader/js/
+-rw-r--r--   0 master    (1000) master    (1000)     6730 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader/js/dataTables.fixedHeader.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader-bs/
+-rw-r--r--   0 master    (1000) master    (1000)      872 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader-bs/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader-bs/css/
+-rw-r--r--   0 master    (1000) master    (1000)      328 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader-bs/css/fixedHeader.bootstrap.min.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive/
+-rw-r--r--   0 master    (1000) master    (1000)      737 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive/js/
+-rw-r--r--   0 master    (1000) master    (1000)    12400 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive/js/dataTables.responsive.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/
+-rw-r--r--   0 master    (1000) master    (1000)      885 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/css/
+-rw-r--r--   0 master    (1000) master    (1000)     3992 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/css/responsive.bootstrap.min.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/js/
+-rw-r--r--   0 master    (1000) master    (1000)     1246 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/js/responsive.bootstrap.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select/
+-rw-r--r--   0 master    (1000) master    (1000)      742 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select/js/
+-rw-r--r--   0 master    (1000) master    (1000)    11472 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select/js/dataTables.select.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select-bs/
+-rw-r--r--   0 master    (1000) master    (1000)      848 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select-bs/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select-bs/css/
+-rw-r--r--   0 master    (1000) master    (1000)     4154 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/datatables.net-select-bs/css/select.bootstrap.min.css
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/
+-rw-r--r--   0 master    (1000) master    (1000)      853 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.128661 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    16066 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.css
+-rw-r--r--   0 master    (1000) master    (1000)   213774 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     1997 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.print.min.css
+-rw-r--r--   0 master    (1000) master    (1000)     4626 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/gcal.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/locale/
+-rw-r--r--   0 master    (1000) master    (1000)     3816 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/locale/es.js
+-rw-r--r--   0 master    (1000) master    (1000)     3073 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/locale/fr.js
+-rw-r--r--   0 master    (1000) master    (1000)     2987 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/locale/it.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery/
+-rw-r--r--   0 master    (1000) master    (1000)      190 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    86927 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery/dist/jquery.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/
+-rw-r--r--   0 master    (1000) master    (1000)      694 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      264 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.092661 burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/src/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/src/Scripts/
+-rw-r--r--   0 master    (1000) master    (1000)    19606 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/src/Scripts/jquery.fileDownload.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery-ui/
+-rw-r--r--   0 master    (1000) master    (1000)      171 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery-ui/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)   253669 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery-ui/jquery-ui.min.js
+-rw-r--r--   0 master    (1000) master    (1000)      564 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery-ui/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/
+-rw-r--r--   0 master    (1000) master    (1000)     1009 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/dist/
+-rw-r--r--   0 master    (1000) master    (1000)   114799 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/dist/jquery.fancytree-all.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/dist/skin-bootstrap/
+-rw-r--r--   0 master    (1000) master    (1000)    13769 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/dist/skin-bootstrap/ui.fancytree.min.css
+-rw-r--r--   0 master    (1000) master    (1000)     1881 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery.floatThead/
+-rw-r--r--   0 master    (1000) master    (1000)      698 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery.floatThead/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/jquery.floatThead/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    13515 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/jquery.floatThead/dist/jquery.floatThead.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/js-cookie/
+-rw-r--r--   0 master    (1000) master    (1000)      270 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/js-cookie/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/js-cookie/src/
+-rw-r--r--   0 master    (1000) master    (1000)     3886 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/js-cookie/src/js.cookie.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/lodash/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/lodash/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    73121 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/lodash/dist/lodash.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     2044 2021-09-17 08:35:28.000000 burp-ui-1.1.0/burpui/static/vendor/lodash/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/moment/
+-rw-r--r--   0 master    (1000) master    (1000)      442 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/moment/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/moment/locale/
+-rw-r--r--   0 master    (1000) master    (1000)     3449 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/moment/locale/es.js
+-rw-r--r--   0 master    (1000) master    (1000)     2703 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/moment/locale/fr.js
+-rw-r--r--   0 master    (1000) master    (1000)     2157 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/moment/locale/it.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/moment/min/
+-rw-r--r--   0 master    (1000) master    (1000)    51654 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/moment/min/moment.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/moment-timezone/
+-rw-r--r--   0 master    (1000) master    (1000)      395 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/moment-timezone/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.132662 burp-ui-1.1.0/burpui/static/vendor/moment-timezone/builds/
+-rw-r--r--   0 master    (1000) master    (1000)    42530 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/moment-timezone/builds/moment-timezone-with-data-10-year-range.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.136662 burp-ui-1.1.0/burpui/static/vendor/nvd3/
+-rw-r--r--   0 master    (1000) master    (1000)      643 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/nvd3/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.136662 burp-ui-1.1.0/burpui/static/vendor/nvd3/build/
+-rw-r--r--   0 master    (1000) master    (1000)     8419 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/nvd3/build/nv.d3.min.css
+-rw-r--r--   0 master    (1000) master    (1000)   253352 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/nvd3/build/nv.d3.min.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.136662 burp-ui-1.1.0/burpui/static/vendor/select2/
+-rw-r--r--   0 master    (1000) master    (1000)      206 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/select2/bower.json
+-rw-r--r--   0 master    (1000) master    (1000)      678 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/select2/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.136662 burp-ui-1.1.0/burpui/static/vendor/socket.io-client/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.136662 burp-ui-1.1.0/burpui/static/vendor/socket.io-client/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    61701 2021-09-17 08:36:04.000000 burp-ui-1.1.0/burpui/static/vendor/socket.io-client/dist/socket.io.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     3098 2021-09-17 08:36:04.000000 burp-ui-1.1.0/burpui/static/vendor/socket.io-client/package.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.136662 burp-ui-1.1.0/burpui/static/vendor/typeahead.js/
+-rw-r--r--   0 master    (1000) master    (1000)      247 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/typeahead.js/bower.json
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.136662 burp-ui-1.1.0/burpui/static/vendor/typeahead.js/dist/
+-rw-r--r--   0 master    (1000) master    (1000)    26900 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/typeahead.js/dist/typeahead.jquery.min.js
+-rw-r--r--   0 master    (1000) master    (1000)     1801 2021-09-17 08:35:29.000000 burp-ui-1.1.0/burpui/static/vendor/typeahead.js/package.json
+-rw-r--r--   0 master    (1000) master    (1000)    12285 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/tasks.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.140662 burp-ui-1.1.0/burpui/templates/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.140662 burp-ui-1.1.0/burpui/templates/.ropeproject/
+-rw-r--r--   0 master    (1000) master    (1000)     4794 2019-10-02 15:12:13.000000 burp-ui-1.1.0/burpui/templates/.ropeproject/config.py
+-rw-r--r--   0 master    (1000) master    (1000)        6 2019-10-02 15:12:13.000000 burp-ui-1.1.0/burpui/templates/.ropeproject/globalnames
+-rw-r--r--   0 master    (1000) master    (1000)       14 2019-10-02 15:12:13.000000 burp-ui-1.1.0/burpui/templates/.ropeproject/history
+-rw-r--r--   0 master    (1000) master    (1000)        6 2019-10-02 15:12:13.000000 burp-ui-1.1.0/burpui/templates/.ropeproject/objectdb
+-rw-r--r--   0 master    (1000) master    (1000)     1162 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/about.html
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.140662 burp-ui-1.1.0/burpui/templates/admin/
+-rw-r--r--   0 master    (1000) master    (1000)     1780 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/admin/authentication.html
+-rw-r--r--   0 master    (1000) master    (1000)     3045 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/admin/grant-authorization.html
+-rw-r--r--   0 master    (1000) master    (1000)     3989 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/admin/group-authorization.html
+-rw-r--r--   0 master    (1000) master    (1000)     2722 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/admin/sessions.html
+-rw-r--r--   0 master    (1000) master    (1000)     7776 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/admin-authentications.html
+-rw-r--r--   0 master    (1000) master    (1000)    13642 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/admin-authorizations.html
+-rw-r--r--   0 master    (1000) master    (1000)     1846 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/admin-backends.html
+-rw-r--r--   0 master    (1000) master    (1000)     4195 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/backup-report.html
+-rw-r--r--   0 master    (1000) master    (1000)     1158 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/calendar.html
+-rw-r--r--   0 master    (1000) master    (1000)    11932 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/client-browse.html
+-rw-r--r--   0 master    (1000) master    (1000)     3121 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/client-report.html
+-rw-r--r--   0 master    (1000) master    (1000)     4686 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/client.html
+-rw-r--r--   0 master    (1000) master    (1000)     3588 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/clients-report.html
+-rw-r--r--   0 master    (1000) master    (1000)     1402 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/clients.html
+-rw-r--r--   0 master    (1000) master    (1000)    14377 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/gerard.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.140662 burp-ui-1.1.0/burpui/templates/js/
+-rw-r--r--   0 master    (1000) master    (1000)      743 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/about.js
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.140662 burp-ui-1.1.0/burpui/templates/js/admin/
+-rw-r--r--   0 master    (1000) master    (1000)     1116 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/admin/authentication.js
+-rw-r--r--   0 master    (1000) master    (1000)     3860 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/admin/grant-authorization.js
+-rw-r--r--   0 master    (1000) master    (1000)     7738 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/admin/group-authorization.js
+-rw-r--r--   0 master    (1000) master    (1000)     8347 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/admin/sessions.js
+-rw-r--r--   0 master    (1000) master    (1000)     9009 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/admin-authentications.js
+-rw-r--r--   0 master    (1000) master    (1000)    30828 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/admin-authorizations.js
+-rw-r--r--   0 master    (1000) master    (1000)     3896 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/admin-backends.js
+-rw-r--r--   0 master    (1000) master    (1000)     2926 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/backup-report.js
+-rw-r--r--   0 master    (1000) master    (1000)     1680 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/calendar.js
+-rw-r--r--   0 master    (1000) master    (1000)    13073 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/client-browse.js
+-rw-r--r--   0 master    (1000) master    (1000)     5127 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/client-report.js
+-rw-r--r--   0 master    (1000) master    (1000)    10240 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/client.js
+-rw-r--r--   0 master    (1000) master    (1000)     2643 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/clients-report.js
+-rw-r--r--   0 master    (1000) master    (1000)     7921 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/clients.js
+-rw-r--r--   0 master    (1000) master    (1000)     2470 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/live-monitor.js
+-rw-r--r--   0 master    (1000) master    (1000)     2084 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/servers-report.js
+-rw-r--r--   0 master    (1000) master    (1000)     1782 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/servers.js
+-rw-r--r--   0 master    (1000) master    (1000)    27017 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/settings.js
+-rw-r--r--   0 master    (1000) master    (1000)    20380 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/js/user.js
+-rw-r--r--   0 master    (1000) master    (1000)      347 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/js/websocket.js
+-rw-r--r--   0 master    (1000) master    (1000)     9972 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/layout.html
+-rw-r--r--   0 master    (1000) master    (1000)     4937 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/live-monitor.html
+-rw-r--r--   0 master    (1000) master    (1000)      735 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/login.html
+-rw-r--r--   0 master    (1000) master    (1000)    16144 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/macros.html
+-rw-r--r--   0 master    (1000) master    (1000)     1346 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/notifications.html
+-rw-r--r--   0 master    (1000) master    (1000)     1776 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/servers-report.html
+-rw-r--r--   0 master    (1000) master    (1000)      923 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/servers.html
+-rw-r--r--   0 master    (1000) master    (1000)    40891 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/settings.html
+-rw-r--r--   0 master    (1000) master    (1000)      861 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/sideadmin.html
+-rw-r--r--   0 master    (1000) master    (1000)     2870 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/sidebar.html
+-rw-r--r--   0 master    (1000) master    (1000)     1490 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/sideconfig.html
+-rw-r--r--   0 master    (1000) master    (1000)      830 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/sideuser.html
+-rw-r--r--   0 master    (1000) master    (1000)     3767 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/small_topbar.html
+-rw-r--r--   0 master    (1000) master    (1000)     4572 2018-08-18 00:27:08.000000 burp-ui-1.1.0/burpui/templates/topbar.html
+-rw-r--r--   0 master    (1000) master    (1000)    10122 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/templates/user.html
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/burpui/thirdparty/
+-rw-r--r--   0 master    (1000) master    (1000)    24832 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/thirdparty/flask_bower.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/burpui/tools/
+-rw-r--r--   0 master    (1000) master    (1000)     3289 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/tools/logging.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/burpui/translations/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/burpui/translations/es/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/burpui/translations/es/LC_MESSAGES/
+-rw-r--r--   0 master    (1000) master    (1000)    60903 2023-05-01 19:13:29.000000 burp-ui-1.1.0/burpui/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 master    (1000) master    (1000)   102166 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/burpui/translations/fr/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/burpui/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 master    (1000) master    (1000)    24327 2023-05-01 19:13:29.000000 burp-ui-1.1.0/burpui/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 master    (1000) master    (1000)    80323 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/burpui/translations/it/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/burpui/translations/it/LC_MESSAGES/
+-rw-r--r--   0 master    (1000) master    (1000)    56806 2023-05-01 19:13:29.000000 burp-ui-1.1.0/burpui/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 master    (1000) master    (1000)    97706 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/translations/it/LC_MESSAGES/messages.po
+-rw-r--r--   0 master    (1000) master    (1000)     8182 2023-05-01 18:42:40.000000 burp-ui-1.1.0/burpui/utils.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/burpui/ws/
+-rw-r--r--   0 master    (1000) master    (1000)        0 2018-07-24 09:36:18.000000 burp-ui-1.1.0/burpui/ws/__init__.py
+-rw-r--r--   0 master    (1000) master    (1000)      927 2022-11-06 21:20:42.000000 burp-ui-1.1.0/burpui/ws/namespace.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/contrib/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/contrib/centos/
+-rwxr-xr-x   0 master    (1000) master    (1000)     1595 2017-04-28 13:40:18.000000 burp-ui-1.1.0/contrib/centos/init.sh
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/contrib/freebsd/
+-rw-r--r--   0 master    (1000) master    (1000)      602 2018-05-14 12:28:49.000000 burp-ui-1.1.0/contrib/freebsd/gunicorn.rc
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/contrib/gunicorn/
+-rw-r--r--   0 master    (1000) master    (1000)     6080 2022-11-06 21:20:42.000000 burp-ui-1.1.0/contrib/gunicorn/burpui_gunicorn.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/contrib/systemd/
+-rw-r--r--   0 master    (1000) master    (1000)      171 2017-05-09 16:54:39.000000 burp-ui-1.1.0/contrib/systemd/bui-agent.service
+-rw-r--r--   0 master    (1000) master    (1000)      337 2022-11-06 21:20:42.000000 burp-ui-1.1.0/contrib/systemd/bui-celery-beat.service
+-rw-r--r--   0 master    (1000) master    (1000)      191 2022-11-06 21:20:42.000000 burp-ui-1.1.0/contrib/systemd/bui-celery.service
+-rw-r--r--   0 master    (1000) master    (1000)      299 2017-05-09 16:54:39.000000 burp-ui-1.1.0/contrib/systemd/bui-gunicorn.service
+-rw-r--r--   0 master    (1000) master    (1000)      253 2022-11-06 21:20:42.000000 burp-ui-1.1.0/contrib/systemd/bui-monitor.service
+-rw-r--r--   0 master    (1000) master    (1000)      188 2018-05-14 12:28:49.000000 burp-ui-1.1.0/contrib/systemd/bui-websocket.service
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/migrations/
+-rwxr-xr-x   0 master    (1000) master    (1000)       39 2022-11-06 21:20:42.000000 burp-ui-1.1.0/migrations/README
+-rw-r--r--   0 master    (1000) master    (1000)      770 2017-04-28 13:40:18.000000 burp-ui-1.1.0/migrations/alembic.ini
+-rwxr-xr-x   0 master    (1000) master    (1000)     2919 2023-05-01 18:42:40.000000 burp-ui-1.1.0/migrations/env.py
+-rwxr-xr-x   0 master    (1000) master    (1000)      412 2017-04-28 13:40:18.000000 burp-ui-1.1.0/migrations/script.py.mako
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/migrations/versions/
+-rw-r--r--   0 master    (1000) master    (1000)      980 2023-05-01 18:42:40.000000 burp-ui-1.1.0/migrations/versions/225d9b2f0fb1_initial.py
+-rw-r--r--   0 master    (1000) master    (1000)      875 2023-05-01 18:42:40.000000 burp-ui-1.1.0/migrations/versions/4445080944ee_hidden_hosts_management.py
+-rw-r--r--   0 master    (1000) master    (1000)      844 2023-05-01 18:42:40.000000 burp-ui-1.1.0/migrations/versions/56de018f4d88_user_prefs.py
+-rw-r--r--   0 master    (1000) master    (1000)      983 2023-05-01 18:42:40.000000 burp-ui-1.1.0/migrations/versions/695dcbd29d4f_increase_pref_value_size.py
+-rw-r--r--   0 master    (1000) master    (1000)     1190 2023-05-01 18:42:40.000000 burp-ui-1.1.0/migrations/versions/7f317474332d_handle_sessions.py
+-rw-r--r--   0 master    (1000) master    (1000)     3244 2023-05-01 18:42:40.000000 burp-ui-1.1.0/migrations/versions/fc07e3fa0086_sql_compatibility.py
+-rw-r--r--   0 master    (1000) master    (1000)      224 2022-11-06 21:20:42.000000 burp-ui-1.1.0/pyproject.toml
+-rw-r--r--   0 master    (1000) master    (1000)      290 2023-05-01 18:42:40.000000 burp-ui-1.1.0/requirements.txt
+-rw-r--r--   0 master    (1000) master    (1000)      503 2023-05-01 19:13:30.148662 burp-ui-1.1.0/setup.cfg
+-rwxr-xr-x   0 master    (1000) master    (1000)    14194 2023-05-01 18:42:40.000000 burp-ui-1.1.0/setup.py
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/share/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.096661 burp-ui-1.1.0/share/burpui/
+drwxr-xr-x   0 master    (1000) master    (1000)        0 2023-05-01 19:13:30.144662 burp-ui-1.1.0/share/burpui/etc/
+-rw-r--r--   0 master    (1000) master    (1000)      772 2022-11-06 21:20:42.000000 burp-ui-1.1.0/share/burpui/etc/buimonitor.sample.cfg
+-rw-r--r--   0 master    (1000) master    (1000)    15828 2022-11-06 21:20:42.000000 burp-ui-1.1.0/share/burpui/etc/burpui.sample.cfg
```

### Comparing `burp-ui-1.0.0/CHANGELOG.rst` & `burp-ui-1.1.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+1.1.0 (05/01/2023)
+------------------
+
+- fix: update dependencies and fix unit tests `#352 <https://git.ziirish.me/ziirish/burp-ui/issues/352>`_
+- fix: platform.dist is no longer part of the std lib
+- fix: adapt send_file usage
+
 1.0.0 (11/06/2022)
 ------------------
 
 - **BREAKING**: the *single* and *version* options within the ``[Global]`` section have been removed in favor of a new unified *backend* option
 - **BREAKING**: a change introduced by `#284 <https://git.ziirish.me/ziirish/burp-ui/issues/284>`_ may return wrong timestamps for backups made with burp-server <= 2.1.10 if your current burp-server is >= 2.1.10
 - **BREAKING**: the authentication backends section have been renamed with the ``:AUTH`` suffix
 - **BREAKING**: the ``prefix`` option has been moved from the ``[Global]`` configuration section to the ``[Production]`` one
```

### Comparing `burp-ui-1.0.0/LICENSE` & `burp-ui-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/PKG-INFO` & `burp-ui-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burp-ui
-Version: 1.0.0
+Version: 1.1.0
 Summary: Burp-UI is a web-ui for burp backup written in python with Flask and jQuery/Bootstrap
 Home-page: https://git.ziirish.me/ziirish/burp-ui
 Author: Benjamin SANS (Ziirish)
 Author-email: hi+burpui@ziirish.me
 License: BSD 3-clause License
 Keywords: burp web ui backup monitoring
 Platform: UNKNOWN
```

### Comparing `burp-ui-1.0.0/README.rst` & `burp-ui-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burp_ui.egg-info/PKG-INFO` & `burp-ui-1.1.0/burp_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burp-ui
-Version: 1.0.0
+Version: 1.1.0
 Summary: Burp-UI is a web-ui for burp backup written in python with Flask and jQuery/Bootstrap
 Home-page: https://git.ziirish.me/ziirish/burp-ui
 Author: Benjamin SANS (Ziirish)
 Author-email: hi+burpui@ziirish.me
 License: BSD 3-clause License
 Keywords: burp web ui backup monitoring
 Platform: UNKNOWN
```

### Comparing `burp-ui-1.0.0/burp_ui.egg-info/SOURCES.txt` & `burp-ui-1.1.0/burp_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burp_ui.egg-info/requires.txt` & `burp-ui-1.1.0/burp_ui.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-trio==0.19.0
-Flask==2.0.3
+trio==0.22.0
+Flask==2.2.3
 Flask-Login==0.6.2
-Flask-Babel==2.0.0
+Flask-Babel==3.0.1
 Flask-WTF==0.15.1
-flask-restx==1.0.3
-Flask-Caching==1.10.1
+flask-restx==1.1.0
+Flask-Caching==2.0.2
 Flask-Session==0.4.0
-WTForms==2.3.3
-arrow==1.1.1
+WTForms==3.0.0
+arrow==1.2.3
 pluginbase==1.0.1
-tzlocal==3.0
-pyOpenSSL==22.1.0
-configobj==5.0.6
+tzlocal==4.3
+pyOpenSSL==23.0.0
+configobj==5.0.8
 async_generator==1.10
-Click==7.1.2
-python-pam==1.8.4
+Click==8.1.3
+python-pam==2.0.2
 
 [celery]
 Celery>=4.3
 redis
 
 [ci]
 pytest
```

### Comparing `burp-ui-1.0.0/burpui/.ropeproject/config.py` & `burp-ui-1.1.0/burpui/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/.ropeproject/globalnames` & `burp-ui-1.1.0/burpui/.ropeproject/globalnames`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/.ropeproject/objectdb` & `burp-ui-1.1.0/burpui/.ropeproject/objectdb`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/__main__.py` & `burp-ui-1.1.0/burpui/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,15 @@
     :platform: Unix
     :synopsis: Burp-UI main module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 """
 import os
 import sys
-
-from argparse import ArgumentParser, REMAINDER
+from argparse import REMAINDER, ArgumentParser
 
 ROOT = os.path.dirname(os.path.realpath(__file__))
 # Try to load modules from our current env first
 sys.path.insert(0, os.path.join(ROOT, ".."))
 
 
 def parse_args(mode=True, name=None):
@@ -75,15 +74,15 @@
 
     options, unknown = parser.parse_known_args()
     if mode and options.mode and options.mode not in ["celery", "manage", "server"]:
         options = parser.parse_args()
         unknown = []
 
     if options.version:
-        from burpui.desc import __title__, __version__, __release__
+        from burpui.desc import __release__, __title__, __version__
 
         ver = "{}: v{}".format(mname or __title__, __version__)
         if options.log:
             ver = "{} ({})".format(ver, __release__)
         print(ver)
         sys.exit(0)
 
@@ -149,14 +148,15 @@
     args += [x for x in options.remaining if x != "--"]
 
     os.execvpe(args[0], args, env)
 
 
 def agent(options=None):
     import trio
+
     from burpui.engines.agent import BUIAgent as Agent
     from burpui.utils import lookup_file
 
     if not options:
         options, _ = parse_args(mode=False, name="bui-agent")
 
     conf = ["buiagent.cfg", "buiagent.sample.cfg"]
@@ -168,14 +168,15 @@
 
     agent = Agent(conf, options.log, options.logfile)
     trio.run(agent.run)
 
 
 def monitor(options=None):
     import trio
+
     from burpui.engines.monitor import MonitorPool
     from burpui.utils import lookup_file
 
     if not options:
         options, _ = parse_args(mode=False, name="bui-agent")
 
     conf = ["buimonitor.cfg", "buimonitor.sample.cfg"]
```

### Comparing `burp-ui-1.0.0/burpui/_compat.py` & `burp-ui-1.1.0/burpui/_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
     :platform: Unix
     :synopsis: Burp-UI compatibility module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
 import pickle  # noqa
-
-from urllib.parse import unquote, quote, urlparse, urljoin  # noqa
+from urllib.parse import quote, unquote, urljoin, urlparse  # noqa
 
 text_type = str
 string_types = (str,)
 
 
 def to_bytes(text):
     """Transform string to bytes."""
```

### Comparing `burp-ui-1.0.0/burpui/_json.py` & `burp-ui-1.1.0/burpui/_json.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/api/.ropeproject/config.py` & `burp-ui-1.1.0/burpui/api/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/api/.ropeproject/globalnames` & `burp-ui-1.1.0/burpui/api/.ropeproject/globalnames`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/api/__init__.py` & `burp-ui-1.1.0/burpui/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,30 +4,30 @@
     :platform: Unix
     :synopsis: Burp-UI api module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 
 """
+import hashlib
 import os
 import sys
 import uuid
-import hashlib
+from functools import wraps
+from importlib import import_module
 
-from flask import Blueprint, Response, request, current_app, session, abort, g
-from flask_restx import Api as ApiPlus
+from flask import Blueprint, Response, abort, current_app, g, request, session
 from flask_login import current_user
-from importlib import import_module
-from functools import wraps
+from flask_restx import Api as ApiPlus
 
 from .._compat import to_bytes
-from ..desc import __version__, __release__, __url__, __doc__
+from ..config import config
+from ..desc import __doc__, __release__, __url__, __version__
 from ..engines.server import BUIServer  # noqa
 from ..exceptions import BUIserverException
-from ..config import config
 from ..tools.logging import logger
 
 bui = current_app  # type: BUIServer
 EXEMPT_METHODS = set(["OPTIONS"])
 
 
 def force_refresh():
```

### Comparing `burp-ui-1.0.0/burpui/api/admin.py` & `burp-ui-1.1.0/burpui/api/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 .. module:: burpui.api.admin
     :platform: Unix
     :synopsis: Burp-UI admin api module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-from . import api
+import json
+
+from flask import current_app
+from flask_babel import gettext
+from flask_login import current_user
+
 from ..engines.server import BUIServer  # noqa
-from ..sessions import session_manager
 from ..misc.acl.meta import meta_grants
+from ..sessions import session_manager
 from ..utils import NOTIF_OK
-from .custom import fields, Resource
+from . import api
+from .custom import Resource, fields
 
 #  from ..exceptions import BUIserverException
 
-from flask import current_app
-from flask_login import current_user
-from flask_babel import gettext
-
-import json
 
 bui = current_app  # type: BUIServer
 ns = api.namespace("admin", "Admin methods")
 
 user_fields = ns.model(
     "Users",
     {
```

### Comparing `burp-ui-1.0.0/burpui/api/backup.py` & `burp-ui-1.1.0/burpui/api/backup.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 .. module:: burpui.api.backup
     :platform: Unix
     :synopsis: Burp-UI backup api module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-from . import api
-from ..engines.server import BUIServer  # noqa
-from .custom import Resource
-from ..exceptions import BUIserverException
-
 from flask import current_app
 from flask_login import current_user
 
+from ..engines.server import BUIServer  # noqa
+from ..exceptions import BUIserverException
+from . import api
+from .custom import Resource
+
 bui = current_app  # type: BUIServer
 ns = api.namespace("backup", "Backup methods")
 
 
 @ns.route(
     "/server-backup/<name>",
     "/<server>/server-backup/<name>",
```

### Comparing `burp-ui-1.0.0/burpui/api/client.py` & `burp-ui-1.1.0/burpui/api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
 import os
 import re
 
-from . import api, cache_key, force_refresh
-from ..engines.server import BUIServer  # noqa
-from .custom import fields, Resource
-from ..decorators import browser_cache
-from ..ext.cache import cache
-from ..exceptions import BUIserverException
-
-from flask_restx.marshalling import marshal
-from flask_restx import inputs
 from flask import current_app, request
 from flask_login import current_user
+from flask_restx import inputs
+from flask_restx.marshalling import marshal
+
+from ..decorators import browser_cache
+from ..engines.server import BUIServer  # noqa
+from ..exceptions import BUIserverException
+from ..ext.cache import cache
+from . import api, cache_key, force_refresh
+from .custom import Resource, fields
 
 bui = current_app  # type: BUIServer
 ns = api.namespace("client", "Client methods")
 
 node_fields = ns.model(
     "ClientTree",
     {
```

### Comparing `burp-ui-1.0.0/burpui/api/clients.py` & `burp-ui-1.1.0/burpui/api/clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 .. module:: burpui.api.clients
     :platform: Unix
     :synopsis: Burp-UI clients api module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-from . import api, cache_key, force_refresh
+from flask import current_app, g
+from flask_login import current_user
+
+from ..decorators import browser_cache
 from ..engines.server import BUIServer  # noqa
-from .custom import fields, Resource
-from .client import ClientLabels
-from ..ext.cache import cache
 from ..exceptions import BUIserverException
-from ..decorators import browser_cache
+from ..ext.cache import cache
 from ..filter import mask
-
-from flask import current_app, g
-from flask_login import current_user
+from . import api, cache_key, force_refresh
+from .client import ClientLabels
+from .custom import Resource, fields
 
 bui = current_app  # type: BUIServer
 ns = api.namespace("clients", "Clients methods")
 
 
 @ns.route(
     "/running",
@@ -225,15 +225,15 @@
                     x
                     for x in clients
                     if mask.is_client_allowed(current_user, x, server)
                 ]
                 res = [x for x in res if x in allowed]
         running = False
         if isinstance(res, dict):
-            for (_, run) in res.items():
+            for _, run in res.items():
                 running = running or (len(run) > 0)
                 if running:
                     break
         else:
             running = len(res) > 0
 
         return running
@@ -772,13 +772,13 @@
                         x
                         for x in clients_cache.get(serv, [])
                         if bui.acl.is_client_allowed(user, x, serv)
                     ]
             else:
                 for serv in bui.client.servers:
                     grants[serv] = "all"
-            for (serv, clients) in grants.items():
+            for serv, clients in grants.items():
                 if not isinstance(clients, list):
                     clients = clients_cache.get(serv, [])
                 ret += [{"name": x, "agent": serv} for x in clients]
 
         return ret
```

### Comparing `burp-ui-1.0.0/burpui/api/custom/.ropeproject/config.py` & `burp-ui-1.1.0/burpui/api/custom/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/api/custom/fields.py` & `burp-ui-1.1.0/burpui/api/custom/fields.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,23 +5,18 @@
     :synopsis: Burp-UI api custom fields module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 
 """
 import flask_restx.fields
-
 from flask_restx.fields import *  # noqa # pylint: disable=locally-disabled, wildcard-import, unused-wildcard-import
-from .my_fields import (
-    DateTime,
-    DateTimeHuman,
-    BackupNumber,
-    SafeString,
-    LocalizedString,
-)  # noqa
+
+from .my_fields import DateTimeHuman  # noqa
+from .my_fields import BackupNumber, DateTime, LocalizedString, SafeString
 
 __all__ = flask_restx.fields.__all__ + (
     DateTime,
     DateTimeHuman,
     BackupNumber,
     SafeString,
     LocalizedString,
```

### Comparing `burp-ui-1.0.0/burpui/api/custom/my_fields.py` & `burp-ui-1.1.0/burpui/api/custom/my_fields.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     :synopsis: Burp-UI api custom fields module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 
 """
 import datetime
-import arrow
-
-from ...ext.i18n import get_locale
 
-from flask_restx import fields
-from flask_babel import gettext as _
+import arrow
 from flask import escape
+from flask_babel import gettext as _
+from flask_restx import fields
 from tzlocal import get_localzone
 
+from ...ext.i18n import get_locale
+
 TZ = str(get_localzone())
 
 
 class DateTime(fields.DateTime):
     """Custom DateTime parser on top of :mod:`arrow` to provide lossless dates"""
 
     def parse(self, value):
```

### Comparing `burp-ui-1.0.0/burpui/api/custom/resource.py` & `burp-ui-1.1.0/burpui/api/custom/resource.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/api/misc.py` & `burp-ui-1.1.0/burpui/api/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 .. module:: burpui.api.misc
     :platform: Unix
     :synopsis: Burp-UI misc api module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-from . import api, cache_key, force_refresh
+import random
+import re
+
+from flask import current_app, flash, get_flashed_messages, session, url_for
+from flask_login import current_user
+
+from ..decorators import browser_cache
 from ..engines.server import BUIServer  # noqa
-from .custom import fields, Resource
-from .client import ClientLabels
-from ..filter import mask
 from ..exceptions import BUIserverException
-from ..decorators import browser_cache
 from ..ext.cache import cache
 from ..ext.i18n import LANGUAGES
-
-from flask import flash, get_flashed_messages, url_for, current_app, session
-from flask_login import current_user
-
-import random
-import re
+from ..filter import mask
+from . import api, cache_key, force_refresh
+from .client import ClientLabels
+from .custom import Resource, fields
 
 bui = current_app  # type: BUIServer
 ns = api.namespace("misc", "Misc methods")
 
 
 def clear_cache(pattern=None):
     """Clear the cache, you can also provide a pattern to only clean matching keys"""
@@ -209,15 +209,15 @@
                     404,
                     "'{}' not found in the list of running clients for '{}'".format(
                         client, server
                     ),
                 )
             else:
                 found = False
-                for (_, cls) in running.items():
+                for _, cls in running.items():
                     if client in cls:
                         found = True
                         break
                 if not found:
                     api.bort(404, "'{}' not found in running clients".format(client))
         else:
             if client not in running:
@@ -342,15 +342,15 @@
                     x
                     for x in running
                     if mask.is_client_allowed(current_user, x, server)
                 ]
         else:
             running = bui.client.is_one_backup_running()
         if isinstance(running, dict):
-            for (serv, clients) in running.items():
+            for serv, clients in running.items():
                 for client in clients:
                     # ACL
                     if mask.has_filters(current_user) and not mask.is_client_allowed(
                         current_user, client, serv
                     ):
                         continue
                     data = {}
@@ -529,23 +529,23 @@
         res["release"] = api.release
         res["api"] = url_for("api.doc")
         res["burp"] = []
         cli = bui.client.get_client_version(server)
         srv = bui.client.get_server_version(server)
         multi = {}
         if isinstance(cli, dict):
-            for (name, val) in cli.items():
+            for name, val in cli.items():
                 multi[name] = {"client": val}
         if isinstance(srv, dict):
-            for (name, val) in srv.items():
+            for name, val in srv.items():
                 multi[name]["server"] = val
         if not multi:
             res["burp"].append({"client": cli, "server": srv})
         else:
-            for (name, val) in multi.items():
+            for name, val in multi.items():
                 tmp = val
                 tmp.update({"name": name})
                 res["burp"].append(tmp)
         return res
 
 
 @ns.route("/ping", endpoint="ping")
@@ -837,15 +837,15 @@
                     grants[serv] = [
                         x
                         for x in all_clients
                         if mask.is_client_allowed(current_user, x, serv)
                     ]
                 else:
                     grants[serv] = "all"
-            for (serv, clients) in grants.items():
+            for serv, clients in grants.items():
                 if not isinstance(clients, list):
                     if data and serv in data:
                         clients = data[serv].keys()
                     else:
                         clients = [
                             x["name"]
                             for x in bui.client.get_all_clients(
```

### Comparing `burp-ui-1.0.0/burpui/api/prefs.py` & `burp-ui-1.1.0/burpui/api/prefs.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 .. module:: burpui.api.prefs
     :platform: Unix
     :synopsis: Burp-UI prefs api module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-from flask import session, current_app, request
+from flask import current_app, request, session
 from flask_login import current_user
 from werkzeug.datastructures import MultiDict
 
-from . import api
 from ..engines.server import BUIServer  # noqa
 from ..ext.i18n import LANGUAGES
-from .custom import fields, Resource
+from . import api
+from .custom import Resource, fields
 
 bui = current_app  # type: BUIServer
 ns = api.namespace("preferences", "Preferences methods")
 
 
 @ns.route("/ui/hide", endpoint="prefs_ui_hide")
 class PrefsUIHide(Resource):
```

### Comparing `burp-ui-1.0.0/burpui/api/restore.py` & `burp-ui-1.1.0/burpui/api/restore.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,28 +5,28 @@
     :synopsis: Burp-UI restore api module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
 import select
 import struct
-
-from . import api
-from ..engines.server import BUIServer  # noqa
-from .custom import fields, Resource
-from ..exceptions import BUIserverException
-
-from zlib import adler32
 from time import gmtime, strftime, time
-from flask import Response, send_file, make_response, after_this_request, current_app
+from zlib import adler32
+
+from flask import Response, after_this_request, current_app, make_response, send_file
 from flask_login import current_user
 from flask_restx import inputs
 from werkzeug.datastructures import Headers
 from werkzeug.exceptions import HTTPException
 
+from ..engines.server import BUIServer  # noqa
+from ..exceptions import BUIserverException
+from . import api
+from .custom import Resource, fields
+
 bui = current_app  # type: BUIServer
 ns = api.namespace("restore", "Restore methods")
 
 
 @ns.route(
     "/archive/<name>/<int:backup>",
     "/<server>/archive/<name>/<int:backup>",
@@ -185,15 +185,15 @@
 
                     os.remove(archive)
                     return response
 
                 resp = send_file(
                     fh,
                     as_attachment=True,
-                    attachment_filename=filename,
+                    download_name=filename,
                     mimetype="application/zip",
                 )
                 resp.set_cookie("fileDownload", "true")
             except Exception as exp:
                 bui.client.logger.error(str(exp))
                 self.abort(500, str(exp))
         else:
```

### Comparing `burp-ui-1.0.0/burpui/api/servers.py` & `burp-ui-1.1.0/burpui/api/servers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf8 -*-
 
 # This is a submodule we can also use "from ..api import api"
-from . import api, cache_key, force_refresh
-from ..engines.server import BUIServer  # noqa
-from .custom import fields, Resource
-from ..filter import mask
-from ..ext.cache import cache
-from ..decorators import browser_cache
-from ..exceptions import BUIserverException
-
 from flask import current_app, g
 from flask_login import current_user
 
+from ..decorators import browser_cache
+from ..engines.server import BUIServer  # noqa
+from ..exceptions import BUIserverException
+from ..ext.cache import cache
+from ..filter import mask
+from . import api, cache_key, force_refresh
+from .custom import Resource, fields
+
 bui = current_app  # type: BUIServer
 ns = api.namespace("servers", "Servers methods")
 
 
 @ns.route("/stats", endpoint="servers_stats")
 class ServersStats(Resource):
     """The :class:`burpui.api.servers.ServersStats` resource allows you to
```

### Comparing `burp-ui-1.0.0/burpui/api/settings.py` & `burp-ui-1.1.0/burpui/api/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,35 +5,36 @@
     :synopsis: Burp-UI settings api module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
 import json
 
-from . import api
-from ..engines.server import BUIServer  # noqa
-from ..ext.cache import cache
-from .custom import Resource
-from .._compat import unquote
-from ..utils import NOTIF_INFO
-
-from flask_babel import gettext as _, refresh
 from flask import (
-    jsonify,
-    request,
-    url_for,
     current_app,
     g,
-    session,
+    jsonify,
     render_template_string,
+    request,
+    session,
+    url_for,
 )
+from flask_babel import gettext as _
+from flask_babel import refresh
 from flask_login import current_user
 from flask_restx import inputs
 from jinja2 import Environment, meta
+
+from .._compat import unquote
 from ..datastructures import ImmutableMultiDict, MultiDict
+from ..engines.server import BUIServer  # noqa
+from ..ext.cache import cache
+from ..utils import NOTIF_INFO
+from . import api
+from .custom import Resource
 
 TEMPLATE_EXCLUDES = ["client", "agent"]
 
 bui = current_app  # type: BUIServer
 ns = api.namespace("settings", "Settings methods")
 
 
@@ -1022,15 +1023,14 @@
 @ns.doc(
     params={
         "server": "Which server to collect data from when in multi-agent mode",
         "client": "Client name",
     },
 )
 class PathExpander(Resource):
-
     parser = ns.parser()
     parser.add_argument("path", required=True, help="No 'path' provided")
     parser.add_argument("source", required=False, help="Which file is it included in")
 
     @api.acl_admin_or_moderator_required(
         message=_("Sorry, you don't have rights to access the setting panel")
     )
```

### Comparing `burp-ui-1.0.0/burpui/api/tasks.py` & `burp-ui-1.1.0/burpui/api/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,44 +6,44 @@
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
 import os
 import select
 import struct
-
-from . import api, cache_key, force_refresh
-from .misc import History
-from .custom import Resource
-from .client import node_fields
-from .clients import RunningBackup, ClientsReport, RunningClients
-from ..engines.server import BUIServer  # noqa
-from ..ext.cache import cache
-from ..config import config
-from ..decorators import browser_cache
-from ..tasks import perform_restore, load_all_tree, delete_client, force_scheduling_now
-
+from datetime import timedelta
 from time import time
 from zlib import adler32
+
 from flask import (
-    url_for,
     Response,
-    current_app,
     after_this_request,
-    send_file,
-    request,
+    current_app,
     g,
+    request,
+    send_file,
     session,
+    url_for,
 )
 from flask_babel import gettext as _
-from flask_restx import inputs
 from flask_login import current_user
-from datetime import timedelta
+from flask_restx import inputs
 from werkzeug.datastructures import Headers
 
+from ..config import config
+from ..decorators import browser_cache
+from ..engines.server import BUIServer  # noqa
+from ..ext.cache import cache
+from ..tasks import delete_client, force_scheduling_now, load_all_tree, perform_restore
+from . import api, cache_key, force_refresh
+from .client import node_fields
+from .clients import ClientsReport, RunningBackup, RunningClients
+from .custom import Resource
+from .misc import History
+
 try:
     from .ext.ws import socketio  # noqa
 
     WS_AVAILABLE = True
 except ImportError:
     WS_AVAILABLE = False
 
@@ -236,15 +236,15 @@
                 """
                 os.remove(path)
                 return response
 
             resp = send_file(
                 fh,
                 as_attachment=True,
-                attachment_filename=filename,
+                download_name=filename,
                 mimetype="application/zip",
             )
             resp.set_cookie("fileDownload", "true")
         except Exception as e:
             bui.client.logger.error(str(e))
             self.abort(500, str(e))
```

### Comparing `burp-ui-1.0.0/burpui/app.py` & `burp-ui-1.1.0/burpui/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 .. module:: burpui.app
     :platform: Unix
     :synopsis: Burp-UI app module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 """
+import json
+import logging
 import os
 import sys
-import json
 import time
-import logging
 
-from .desc import __version__, __release__
+from .desc import __release__, __version__
 from .extensions import (
     create_celery,
     create_db,
     create_websocket,
-    parse_db_setting,
     get_redis_server,
+    parse_db_setting,
 )
 
 
 def create_app(conf=None, verbose=0, logfile=None, **kwargs):
     """Initialize the whole application.
 
     :param conf: Configuration file to use
@@ -49,26 +49,27 @@
                    - websocket_server (bool): Are we running the websocket
                    server. Default is False
     :type kwargs: dict
 
     :returns: A :class:`burpui.engines.server.BUIServer` object
     """
     from flask import g, request, session
-    from flask_login import LoginManager
     from flask_babel import gettext
-    from .thirdparty.flask_bower import Bower
-    from .utils import ReverseProxied, lookup_file, is_uuid
-    from .tools.logging import logger
-    from .security import basic_login_from_request
+    from flask_login import LoginManager
+
     from .engines.server import BUIServer as BurpUI
-    from .sessions import session_manager
-    from .filter import mask
     from .ext.cache import cache
     from .ext.i18n import babel, get_locale
+    from .filter import mask
     from .misc.auth.handler import BUIanon
+    from .security import basic_login_from_request
+    from .sessions import session_manager
+    from .thirdparty.flask_bower import Bower
+    from .tools.logging import logger
+    from .utils import ReverseProxied, is_uuid, lookup_file
 
     gunicorn = kwargs.get("gunicorn", True)
     unittest = kwargs.get("unittest", False)
     debug = kwargs.get("debug", False)
     cli = kwargs.get("cli", False)
     reverse_proxy = kwargs.get("reverse_proxy", gunicorn)
     celery_worker = kwargs.get("celery_worker", False)
@@ -175,14 +176,15 @@
         try:
             # Session setup
             if not app.session_db or str(app.session_db).lower() not in [
                 "none",
                 "false",
             ]:
                 from redis import Redis
+
                 from .ext.session import sess
 
                 host, port, pwd = get_redis_server(app)
                 db = 0
                 if app.session_db and str(app.session_db).lower() not in [
                     "redis",
                     "default",
@@ -230,15 +232,15 @@
                     db = 1
                 logger.debug(
                     "CACHE: Using redis://guest:****@{}:{}/{}".format(host, port, db)
                 )
                 cache.init_app(
                     app,
                     config={
-                        "CACHE_TYPE": "redis",
+                        "CACHE_TYPE": "flask_caching.backends.redis",
                         "CACHE_REDIS_HOST": host,
                         "CACHE_REDIS_PORT": port,
                         "CACHE_REDIS_PASSWORD": pwd,
                         "CACHE_REDIS_DB": db,
                     },
                 )
                 # clear cache at startup in case we removed or added servers
@@ -295,15 +297,15 @@
     babel.init_app(app)
 
     # Create SQLAlchemy if enabled
     create_db(app, cli, unittest, celery_worker=celery_worker)
 
     if not celery_worker:
         from .api import api, apibp
-        from .routes import view, mypad
+        from .routes import mypad, view
 
         app.jinja_env.globals.update(
             isinstance=isinstance,
             list=list,
             mypad=mypad,
             version_id="{}-{}".format(__version__, __release__),
         )
```

### Comparing `burp-ui-1.0.0/burpui/celerybeat-schedule` & `burp-ui-1.1.0/burpui/celerybeat-schedule`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/cli.py` & `burp-ui-1.1.0/burpui/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     :synopsis: Burp-UI CLI module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 """
 import os
 import sys
 import time
+
 import click
 
 if os.getenv("BUI_MODE") in ["server", "ws"] or "websocket" in sys.argv:
     try:
         from gevent import monkey
 
         monkey.patch_socket()
@@ -55,18 +56,19 @@
     gunicorn=False,
     unittest=UNITTEST,
     cli=CLI,
     websocket_server=(os.getenv("BUI_MODE") == "ws" or "websocket" in sys.argv),
 )
 
 try:
-    from .extensions import create_db
-    from .ext.sql import db
     from flask_migrate import Migrate
 
+    from .ext.sql import db
+    from .extensions import create_db
+
     # This may have been reseted by create_app
     if isinstance(app.database, bool):
         app.config["WITH_SQL"] = app.database
     else:
         app.config["WITH_SQL"] = app.database and app.database.lower() != "none"
 
     if app.config["WITH_SQL"]:
@@ -466,21 +468,22 @@
         msg = app.load_modules()
     except Exception as e:
         msg = str(e)
 
     if msg:
         _die(msg, "setup-burp")
 
-    from .misc.parser.utils import Config
-    from .misc.backend.utils.constant import BURP_LISTEN_OPTION, BURP_BIND_MULTIPLE
-    from .app import get_redis_server
-    from .config import BUIConfig
     import difflib
     import tempfile
 
+    from .app import get_redis_server
+    from .config import BUIConfig
+    from .misc.backend.utils.constant import BURP_BIND_MULTIPLE, BURP_LISTEN_OPTION
+    from .misc.parser.utils import Config
+
     if monitor:
         monconf = BUIConfig(monitor)
         monconf_orig = []
         mon_orig = mon_source = monitor
 
         if dry:
             try:
@@ -591,18 +594,19 @@
                     "Backend password does not match monitor password", fg="yellow"
                 )
             )
 
     if redis:
         try:
             # detect missing modules
-            import redis as redis_client  # noqa
-            import celery  # noqa
             import socket
 
+            import celery  # noqa
+            import redis as redis_client  # noqa
+
             if (
                 "redis" not in app.conf.options["Production"]
                 or "redis" in app.conf.options["Production"]
                 and app.conf.options["Production"]["redis"] != redis
             ) and app.redis != redis:
                 app.conf.options["Production"]["redis"] = redis
                 app.redis = redis
@@ -970,15 +974,14 @@
         warn(
             'Unable to find "clientconfdir" option, you will have to '
             "setup the agent by your own"
         )
         bconfagent = os.devnull
 
     if not os.path.exists(bconfagent):
-
         agenttpl = """
 password = abcdefgh
 """
 
         if not dry:
             with open(bconfagent, "w") as confagent:
                 confagent.write(agenttpl)
@@ -1035,17 +1038,17 @@
         msg = app.load_modules()
     except Exception as e:
         msg = str(e)
 
     if msg:
         _die(msg, "diag")
 
+    from .app import get_redis_server
     from .misc.backend.utils.constant import BURP_LISTEN_OPTION
     from .misc.parser.utils import Config
-    from .app import get_redis_server
 
     def _value_in_option(value, option, section="Production"):
         if section not in app.conf.options:
             return False
         if option not in app.conf.options[section]:
             return False
         return value in app.conf.options[section][option]
@@ -1053,18 +1056,19 @@
     if (
         "Production" in app.conf.options
         and "redis" in app.conf.options["Production"]
         and any(_value_in_option("redis", x) for x in ["storage", "session", "cache"])
     ):
         try:
             # detect missing modules
-            import redis as redis_client  # noqa
-            import celery  # noqa
             import socket
 
+            import celery  # noqa
+            import redis as redis_client  # noqa
+
             rhost, rport, _ = get_redis_server(app)
             ret = -1
             for res in socket.getaddrinfo(
                 rhost, rport, socket.AF_UNSPEC, socket.SOCK_STREAM
             ):
                 if ret == 0:
                     break
@@ -1341,17 +1345,18 @@
     help="Dump parts of the config (Please double check no sensitive" " data leaked)",
 )
 @click.option(
     "-l", "--load", is_flag=True, help="Load all configured modules for full summary"
 )
 def sysinfo(verbose, load):
     """Returns a couple of system informations to help debugging."""
-    from .desc import __release__, __version__
     import platform
 
+    from .desc import __release__, __version__
+
     msg = None
     if load:
         try:
             msg = app.load_modules()
         except Exception as e:
             msg = str(e)
 
@@ -1371,16 +1376,14 @@
     )
     log("Burp-UI version:     {} ({})".format(__version__, __release__))
     log(
         "OS:                  {}:{} ({})".format(
             platform.system(), platform.release(), os.name
         )
     )
-    if platform.system() == "Linux":
-        log("Distribution:        {} {} {}".format(*platform.dist()))
     log("Single mode:         {}".format(app.config["STANDALONE"]))
     log("Backend:             {}".format(backend))
     log(
         "WebSocket embedded:  {}".format(
             click.style(embedded_ws, fg=colors[embedded_ws])
         )
     )
```

### Comparing `burp-ui-1.0.0/burpui/config.py` & `burp-ui-1.1.0/burpui/config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 .. module:: burpui.config
     :platform: Unix
     :synopsis: Burp-UI config module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
+import codecs
 import os
 import re
-import codecs
+
 import configobj
 import validate
 
 from .tools.logging import logger
 
 
 class BUIConfig(dict):
@@ -110,15 +111,14 @@
             with codecs.open(source, "r", "utf-8", errors="ignore") as config:
                 ori = [x.rstrip("\n") for x in config.readlines()]
             if ori:
                 with codecs.open(conffile, "w", "utf-8", errors="ignore") as config:
                     found = False
                     for line in ori:
                         if re.match(r"^\s*(#|;)+\s*\[{}\]".format(section), line):
-
                             config.write("[{}]\n".format(section))
                             found = True
                         else:
                             config.write("{}\n".format(line))
 
                     if not found:
                         config.write("[{}]\n".format(section))
```

### Comparing `burp-ui-1.0.0/burpui/datastructures.py` & `burp-ui-1.1.0/burpui/datastructures.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/decorators.py` & `burp-ui-1.1.0/burpui/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 .. module:: burpui.decorators
     :platform: Unix
     :synopsis: Burp-UI decorators module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-import time
 import datetime
-
+import time
 from functools import wraps
 
 
 def browser_cache(expires=None):
     """Add Flask cache response headers based on expires in seconds.
 
     If expires is None, caching will be disabled.
@@ -26,21 +25,21 @@
         @app.route('/map')
         @browser_cache(expires=60)
         def index():
             return render_template('index.html')
 
     """
     from wsgiref.handlers import format_date_time
+
     from flask import g
     from flask_restx.utils import unpack
 
     def cache_decorator(view):
         @wraps(view)
         def cache_func(*args, **kwargs):
-
             resp, code, headers = unpack(view(*args, **kwargs))
             now = datetime.datetime.now()
 
             headers["Last-Modified"] = format_date_time(time.mktime(now.timetuple()))
 
             failure = code - 200 >= 100  # this is not a successful answer
             do_not_cache = getattr(g, "DONOTCACHE", False)
```

### Comparing `burp-ui-1.0.0/burpui/desc.py` & `burp-ui-1.1.0/burpui/desc.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/engines/agent.py` & `burp-ui-1.1.0/burpui/engines/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,31 +3,30 @@
 .. module:: burpui.engines.agent
     :platform: Unix
     :synopsis: Burp-UI agent module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
+import json
+import logging
 import os
+import ssl
 import struct
 import sys
-import ssl
-import json
-import logging
 import time
+from functools import partial
 
 import trio
 
-from functools import partial
-
-from ..exceptions import BUIserverException
-from ..misc.backend.interface import BUIbackend
 from .._compat import pickle, to_bytes, to_unicode
 from ..config import config
 from ..desc import __version__
+from ..exceptions import BUIserverException
+from ..misc.backend.interface import BUIbackend
 
 # TODO: sendfile is not yet supported by trio
 # try:
 #     from sendfile import sendfile
 #     USE_SENDFILE = True
 # except ImportError:
 #     USE_SENDFILE = False
@@ -265,16 +264,16 @@
                         os.unlink(path)
                         res = json.dumps(True)
                 else:
                     callback = getattr(self.client, j["func"])
                     if j["args"]:
                         if "pickled" in j and j["pickled"]:
                             # de-serialize arguments if needed
-                            import hmac
                             import hashlib
+                            import hmac
                             from base64 import b64decode
 
                             pickles = to_bytes(j["args"])
                             key = "{}{}".format(self.password, j["func"])
                             key = to_bytes(key)
                             bytes_pickles = pickles
                             digest = hmac.new(
```

### Comparing `burp-ui-1.0.0/burpui/engines/monitor.py` & `burp-ui-1.1.0/burpui/engines/monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,33 +3,32 @@
 .. module:: burpui.engines.monitor
     :platform: Unix
     :synopsis: Burp-UI monitor pool module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-import ssl
-import trio
+import datetime
 import json
+import logging
 import math
+import ssl
 import struct
-import logging
-import datetime
-
 from functools import partial
 from itertools import count
+
+import trio
 from async_generator import asynccontextmanager
 
+from .._compat import to_bytes, to_unicode
+from ..config import config
+from ..desc import __version__
 from ..exceptions import BUIserverException
 from ..misc.backend.utils.burp2 import Monitor
-from ..config import config
-from .._compat import to_bytes, to_unicode
 from ..tools.logging import logger
-from ..desc import __version__
-
 
 CONNECTION_COUNTER = count()
 
 
 BUI_DEFAULTS = {
     "Global": {
         "port": 11111,
```

### Comparing `burp-ui-1.0.0/burpui/engines/server.py` & `burp-ui-1.1.0/burpui/engines/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 .. module:: burpui.server
     :platform: Unix
     :synopsis: Burp-UI server module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
+import logging  # noqa
 import os
 import re
 import sys
-import logging  # noqa
 import warnings
+from datetime import timedelta
 
-from ..tools.logging import logger
-from ..misc.auth.handler import UserAuthHandler
+from flask import Flask
+
+from ..config import config
 from ..misc.acl.handler import ACLloader
 from ..misc.audit.handler import BUIauditLoader
-from ..config import config
+from ..misc.auth.handler import UserAuthHandler
 from ..plugins import PluginManager
-
-from datetime import timedelta
-from flask import Flask
-
+from ..tools.logging import logger
 
 BUI_DEFAULTS = {
     "Global": {
         "port": 0,
         "bind": "",
         "ssl": False,
         "sslcert": "",
```

### Comparing `burp-ui-1.0.0/burpui/engines/worker.py` & `burp-ui-1.1.0/burpui/engines/worker.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/exceptions.py` & `burp-ui-1.1.0/burpui/exceptions.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/ext/i18n.py` & `burp-ui-1.1.0/burpui/ext/i18n.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,31 +6,32 @@
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
 from flask import request, session
 from flask_babel import Babel
 from flask_login import current_user
-from ..config import config
-from .._compat import to_unicode
 
-babel = Babel()
+from .._compat import to_unicode
+from ..config import config
 
 LANGUAGES = {
     "en": to_unicode("English"),
     "fr": to_unicode("Français"),
     "es": to_unicode("Español"),
     "it": to_unicode("Italiano"),
 }
 config["LANGUAGES"] = LANGUAGES
 
 
-@babel.localeselector
 def get_locale():
     locale = None
     if current_user and not current_user.is_anonymous:
         locale = getattr(current_user, "language", None)
     elif "language" in session:
         locale = session.get("language", None)
     if locale not in LANGUAGES:
         locale = None
     return locale or request.accept_languages.best_match(config["LANGUAGES"].keys())
+
+
+babel = Babel()
```

### Comparing `burp-ui-1.0.0/burpui/ext/ws.py` & `burp-ui-1.1.0/burpui/ext/ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 .. module:: burpui.ext.ws
     :platform: Unix
     :synopsis: Burp-UI external WebSocket module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-from ..config import config
 from flask_socketio import SocketIO
 
+from ..config import config
+
 options = {}
 options["async_mode"] = config.get("WS_ASYNC_MODE", "gevent")
 
 #    engineio_logger=config.get('WS_DEBUG', False),
 socketio = SocketIO(
     message_queue=config.get("WS_MESSAGE_QUEUE"),
     manage_session=config.get("WS_MANAGE_SESSION", False),
```

### Comparing `burp-ui-1.0.0/burpui/extensions.py` & `burp-ui-1.1.0/burpui/extensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,17 +53,18 @@
     """Create the SQLAlchemy instance if possible
 
     :param myapp: Application context
     :type myapp: :class:`burpui.engines.server.BUIServer`
     """
     if myapp.config["WITH_SQL"]:
         try:
-            from .ext.sql import db
             from sqlalchemy.exc import OperationalError
             from sqlalchemy_utils.functions import database_exists
+
+            from .ext.sql import db
             from .models import lazy_loading
 
             lazy_loading()
             myapp.config["SQLALCHEMY_TRACK_MODIFICATIONS"] = False
             if (
                 not database_exists(myapp.config["SQLALCHEMY_DATABASE_URI"])
                 and not cli
```

### Comparing `burp-ui-1.0.0/burpui/filter.py` & `burp-ui-1.1.0/burpui/filter.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/misc/.ropeproject/config.py` & `burp-ui-1.1.0/burpui/misc/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/misc/.ropeproject/globalnames` & `burp-ui-1.1.0/burpui/misc/.ropeproject/globalnames`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/misc/acl/.ropeproject/config.py` & `burp-ui-1.1.0/burpui/misc/acl/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/misc/acl/basic.py` & `burp-ui-1.1.0/burpui/misc/acl/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf8 -*-
-from .meta import meta_grants, BUIaclGrant
+from ...utils import NOTIF_ERROR, NOTIF_OK, NOTIF_WARN, __
 from .interface import BUIaclLoader
-from ...utils import NOTIF_OK, NOTIF_WARN, NOTIF_ERROR, __
+from .meta import BUIaclGrant, meta_grants
 
 
 class ACLloader(BUIaclLoader):
     __doc__ = __("Uses the Burp-UI configuration file to load its rules.")
     section = name = "BASIC:ACL"
     priority = 100
```

### Comparing `burp-ui-1.0.0/burpui/misc/acl/handler.py` & `burp-ui-1.1.0/burpui/misc/acl/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf8 -*-
 import os
+from collections import OrderedDict
+from importlib import import_module
 
 from .interface import BUIacl, BUIaclLoader
 from .meta import meta_grants
 
-from importlib import import_module
-from collections import OrderedDict
-
 
 class ACLloader(BUIaclLoader):
     section = name = "ACL"
 
     def __init__(self, app=None):
         """See :func:`burpui.misc.acl.interface.BUIaclLoader.__init__`
```

### Comparing `burp-ui-1.0.0/burpui/misc/acl/interface.py` & `burp-ui-1.1.0/burpui/misc/acl/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 .. module:: burpui.misc.acl.interface
     :platform: Unix
     :synopsis: Burp-UI ACL interface.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-from abc import ABCMeta, abstractmethod, abstractproperty
-
 import logging
+from abc import ABCMeta, abstractmethod, abstractproperty
 
 
 class BUIaclLoader(object, metaclass=ABCMeta):
     """The :class:`burpui.misc.acl.interface.BUIaclLoader` class is used to
     load the actual ACL backend"""
 
     logger = logging.getLogger("burp-ui")
```

### Comparing `burp-ui-1.0.0/burpui/misc/acl/meta.py` & `burp-ui-1.1.0/burpui/misc/acl/meta.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 .. module:: burpui.misc.acl.meta
     :platform: Unix
     :synopsis: Burp-UI ACL meta definitions.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-from .interface import BUIacl
-from ...utils import make_list
+import fnmatch
+import json
+import re
+
 from ...config import config
 from ...ext.cache import cache
-
-import re
-import json
-import fnmatch
+from ...utils import make_list
+from .interface import BUIacl
 
 PARSE_EXCLUDE_KEYS = ["agents", "clients", "ro", "rw", "order", "exclude"]
 PARSE_RESERVED_KEYS = ["ro", "rw", "order", "exclude"]
 DEFAULT_EVAL_ORDER = ["exclude", "rw", "ro"]
 MODE_RETURN = {
     "ro": False,
     "rw": True,
```

### Comparing `burp-ui-1.0.0/burpui/misc/audit/.ropeproject/config.py` & `burp-ui-1.1.0/burpui/misc/audit/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/misc/audit/basic.py` & `burp-ui-1.1.0/burpui/misc/audit/basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf8 -*-
-import re
 import logging
+import re
 
-from .interface import BUIaudit, BUIauditLogger as BUIauditLoggerInterface
 from ...tools.logging import logger as parent_logger
+from .interface import BUIaudit
+from .interface import BUIauditLogger as BUIauditLoggerInterface
 
 
 class BUIauditLoader(BUIaudit):
     section = name = "BASIC:AUDIT"
 
     logfile = None
     max_bytes = None
```

### Comparing `burp-ui-1.0.0/burpui/misc/audit/handler.py` & `burp-ui-1.1.0/burpui/misc/audit/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf8 -*-
-import os
 import inspect
-
-from .interface import BUIaudit, BUIauditLogger as BUIauditLoggerInterface
-
-from importlib import import_module
+import os
 from collections import OrderedDict
+from importlib import import_module
+
 from flask_login import current_user
 
+from .interface import BUIaudit
+from .interface import BUIauditLogger as BUIauditLoggerInterface
+
 
 class BUIauditLoader(BUIaudit):
     """See :class:`burpui.misc.audit.interface.BUIaudit`"""
 
     def __init__(self, app=None):
         """See :func:`burpui.misc.audit.interface.BUIaudit.__init__`
```

### Comparing `burp-ui-1.0.0/burpui/misc/audit/interface.py` & `burp-ui-1.1.0/burpui/misc/audit/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
     :platform: Unix
     :synopsis: Burp-UI audit interface.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
 import logging
-
 from abc import ABCMeta, abstractmethod
 
 
 class BUIauditLogger(object, metaclass=ABCMeta):
     """The :class:`burpui.misc.audit.interface.BUIauditLogger` class defines the audit
     Logger interface.
     """
```

### Comparing `burp-ui-1.0.0/burpui/misc/auth/.ropeproject/config.py` & `burp-ui-1.1.0/burpui/misc/auth/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/misc/auth/.ropeproject/globalnames` & `burp-ui-1.1.0/burpui/misc/auth/.ropeproject/globalnames`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/misc/auth/.ropeproject/objectdb` & `burp-ui-1.1.0/burpui/misc/auth/.ropeproject/objectdb`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/misc/auth/basic.py` & `burp-ui-1.1.0/burpui/misc/auth/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf8 -*-
 import re
 
 from flask_login import AnonymousUserMixin
-from .interface import BUIhandler, BUIuser, BUIloader
-from ...utils import NOTIF_ERROR, NOTIF_OK, NOTIF_WARN, __
 from werkzeug.security import check_password_hash, generate_password_hash
 
+from ...utils import NOTIF_ERROR, NOTIF_OK, NOTIF_WARN, __
+from .interface import BUIhandler, BUIloader, BUIuser
+
 
 class BasicLoader(BUIloader):
     """The :class:`burpui.misc.auth.basic.BasicLoader` class loads the *Basic*
     users.
     """
 
     section = name = "BASIC:AUTH"
```

### Comparing `burp-ui-1.0.0/burpui/misc/auth/handler.py` & `burp-ui-1.1.0/burpui/misc/auth/handler.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf8 -*-
 import os
+from collections import OrderedDict
+from importlib import import_module
+
+from flask import session
+from flask_login import AnonymousUserMixin
 
 from ...sessions import session_manager
 from ...utils import is_uuid
-from .interface import BUIhandler, BUIuser
 from ..acl.interface import BUIacl
-
-from importlib import import_module
-from flask import session
-from collections import OrderedDict
-from flask_login import AnonymousUserMixin
+from .interface import BUIhandler, BUIuser
 
 ACL_METHODS = BUIacl.__abstractmethods__
 
 
 class UserAuthHandler(BUIhandler):
     """See :class:`burpui.misc.auth.interface.BUIhandler`"""
```

### Comparing `burp-ui-1.0.0/burpui/misc/auth/interface.py` & `burp-ui-1.1.0/burpui/misc/auth/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 .. module:: burpui.misc.auth.interface
     :platform: Unix
     :synopsis: Burp-UI authentication interface.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-from flask_login import UserMixin, AnonymousUserMixin
 from abc import ABCMeta, abstractmethod, abstractproperty
 
+from flask_login import AnonymousUserMixin, UserMixin
+
 from ...tools.logging import logger
 
 
 class BUIloader:
     logger = logger
```

### Comparing `burp-ui-1.0.0/burpui/misc/auth/ldap.py` & `burp-ui-1.1.0/burpui/misc/auth/ldap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf8 -*-
+import ssl
+
 from flask_login import AnonymousUserMixin
 
-from .interface import BUIhandler, BUIuser, BUIloader
 from ...utils import __
-
-import ssl
+from .interface import BUIhandler, BUIloader, BUIuser
 
 try:
     from ldap3 import (
-        Server,
-        Connection,
-        Tls,
         ALL,
-        RESTARTABLE,
-        AUTO_BIND_TLS_BEFORE_BIND,
         AUTO_BIND_NONE,
+        AUTO_BIND_TLS_BEFORE_BIND,
+        RESTARTABLE,
         SIMPLE,
+        Connection,
+        Server,
+        Tls,
     )
 except ImportError:
     raise ImportError("Unable to load 'ldap3' module")
 
 
 class LdapLoader(BUIloader):
     """The :class:`burpui.misc.auth.ldap.LdapLoader` handles searching for and
@@ -70,15 +70,15 @@
         try:
             handler.priority = (
                 conf.safe_get("priority", "integer", section=self.section)
                 or handler.priority
             )
         except:
             pass
-        for (opt, key) in mapping.items():
+        for opt, key in mapping.items():
             setattr(self, opt, conf.safe_get(key, "force_string", section=self.section))
 
         if self.validate and self.validate.lower() in ["none", "optional", "required"]:
             self.validate = getattr(ssl, "CERT_{}".format(self.validate.upper()))
         else:
             self.validate = None
         self.version = ssl.OP_NO_SSLv3
```

### Comparing `burp-ui-1.0.0/burpui/misc/auth/local.py` & `burp-ui-1.1.0/burpui/misc/auth/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf8 -*-
 import pwd
-import pam
 
+import pam
 from flask_login import AnonymousUserMixin
-from .interface import BUIhandler, BUIuser, BUIloader
+
 from ...utils import __
+from .interface import BUIhandler, BUIloader, BUIuser
 
 
 class LocalLoader(BUIloader):
     """The :class:`burpui.misc.auth.local.LocalLoader` class loads the *Local*
     users.
     """
```

### Comparing `burp-ui-1.0.0/burpui/misc/backend/.ropeproject/config.py` & `burp-ui-1.1.0/burpui/misc/backend/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/misc/backend/.ropeproject/globalnames` & `burp-ui-1.1.0/burpui/misc/backend/.ropeproject/globalnames`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/misc/backend/burp1.py` & `burp-ui-1.1.0/burpui/misc/backend/burp1.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 .. module:: burpui.misc.backend.burp1
     :platform: Unix
     :synopsis: Burp-UI burp1 backend module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-import re
-import os
-import socket
-import time
 import datetime
 import json
+import os
+import re
 import shutil
+import socket
 import subprocess
 import tempfile
+import time
+from shlex import quote
 
-from .interface import BUIbackend
-from ..parser.burp1 import Parser
-from ...utils import human_readable as _hr, BUIcompress, utc_to_local
-from ...security import sanitize_string
+from ..._compat import to_bytes, to_unicode, unquote
 from ...exceptions import BUIserverException
-from ..._compat import unquote, to_unicode, to_bytes
-
-from shlex import quote
+from ...security import sanitize_string
+from ...utils import BUIcompress
+from ...utils import human_readable as _hr
+from ...utils import utc_to_local
+from ..parser.burp1 import Parser
+from .interface import BUIbackend
 
 
 class Burp(BUIbackend):
     """The :class:`burpui.misc.backend.burp1.Burp` class provides a consistent
     backend for ``burp-1`` servers.
 
     It implements the :class:`burpui.misc.backend.interface.BUIbackend` class
@@ -506,15 +507,15 @@
                 continue
             elif re.match(r"^-+$", line):
                 useful = True
                 continue
 
             found = False
             # this method is not optimal, but it is easy to read and to maintain
-            for (key, regex) in lookup_easy.items():
+            for key, regex in lookup_easy.items():
                 reg = re.search(regex, line)
                 if reg:
                     found = True
                     if key in ["start", "end"]:
                         backup[key] = int(
                             time.mktime(
                                 datetime.datetime.strptime(
@@ -522,15 +523,15 @@
                                 ).timetuple()
                             )
                         )
                     elif key == "duration":
                         tmp = reg.group(1).split(":")
                         tmp.reverse()
                         fields = [0] * 4
-                        for (i, val) in enumerate(tmp):
+                        for i, val in enumerate(tmp):
                             fields[i] = int(val)
                         seconds = 0
                         seconds += fields[0]
                         seconds += fields[1] * 60
                         seconds += fields[2] * (60 * 60)
                         seconds += fields[3] * (60 * 60 * 24)
                         backup[key] = seconds
@@ -539,15 +540,15 @@
                     # break the loop as soon as we find a match
                     break
 
             # if found is True, we already parsed the line so we can jump to the next one
             if found:
                 continue
 
-            for (key, regex) in lookup_complex.items():
+            for key, regex in lookup_complex.items():
                 reg = re.search(regex, line)
                 if reg:
                     # self.logger.debug("match[1]: '{0}'".format(reg.group(1)))
                     spl = re.split(r"\s+", reg.group(1))
                     if len(spl) < 5:
                         return {}
                     backup[key] = {
```

### Comparing `burp-ui-1.0.0/burpui/misc/backend/burp2.py` & `burp-ui-1.1.0/burpui/misc/backend/burp2.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 .. module:: burpui.misc.backend.burp2
     :platform: Unix
     :synopsis: Burp-UI burp2 backend module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-import re
+import json
 import os
+import re
 import time
-import json
-
 from collections import OrderedDict
 
+from ..._compat import to_unicode
+from ...exceptions import BUIserverException
+from ...utils import human_readable as _hr
+from ...utils import utc_to_local
+from ..parser.burp2 import Parser
 from .burp1 import Burp as Burp1
 from .interface import BUIbackend
 from .utils.burp2 import Monitor
 from .utils.constant import BURP_REVERSE_COUNTERS, BURP_STATUS_FORMAT_V2
-from ..parser.burp2 import Parser
-from ...utils import human_readable as _hr, utc_to_local
-from ...exceptions import BUIserverException
-from ..._compat import to_unicode
 
 
 # Some functions are the same as in Burp1 backend
 class Burp(Burp1):
     """The :class:`burpui.misc.backend.burp2.Burp` class provides a consistent
     backend for ``burp-2`` servers.
 
@@ -297,15 +297,15 @@
             name = counter["name"]
             if name in translate:
                 name = translate[name]
             if counter["name"] in single:
                 result[name] = counter["count"]
             else:
                 result[name] = {}
-                for (key, val) in counts.items():
+                for key, val in counts.items():
                     if val in counter:
                         result[name][key] = counter[val]
                     else:
                         result[name][key] = 0
         if "start" in result and "end" in result:
             result["duration"] = result["end"] - result["start"]
             # convert utc timestamp to local
```

### Comparing `burp-ui-1.0.0/burpui/misc/backend/interface.py` & `burp-ui-1.1.0/burpui/misc/backend/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     :synopsis: Burp-UI backend interface.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
 import os
 import re
-
 from abc import ABCMeta, abstractmethod
 
 from ...tools.logging import logger
 
 G_BURPPORT = 4972
 G_BURPHOST = "::1"
 G_BURPBIN = "/usr/sbin/burp"
```

### Comparing `burp-ui-1.0.0/burpui/misc/backend/multi.py` & `burp-ui-1.1.0/burpui/misc/backend/multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf8 -*-
-import re
-import socket
 import errno
 import json
+import re
+import socket
 import struct
 
 from werkzeug.datastructures import ImmutableMultiDict as _ImmutableMultiDict
 
-from .interface import BUIbackend
-from ..parser.interface import BUIparser
-from ...exceptions import BUIserverException
-from ..._compat import pickle, to_unicode, to_bytes
-from ...decorators import implement
+from ..._compat import pickle, to_bytes, to_unicode
 from ...datastructures import ImmutableMultiDict
-
+from ...decorators import implement
+from ...exceptions import BUIserverException
+from ..parser.interface import BUIparser
+from .interface import BUIbackend
 
 INTERFACE_METHODS = BUIbackend.__abstractmethods__
 PARSER_INTERFACE_METHODS = BUIparser.__abstractmethods__
 AGENT_VERSION_CAST = "0.4.9999"
 
 
 class ProxyCall(object):
@@ -552,16 +551,16 @@
         template=False,
         statictemplate=False,
         content="",
         agent=None,
     ):
         """See :func:`burpui.misc.backend.interface.BUIbackend.store_conf_cli`"""
         # serialize data as it is a nested dict
-        import hmac
         import hashlib
+        import hmac
         from base64 import b64encode
 
         if not isinstance(data, (_ImmutableMultiDict, ImmutableMultiDict)):
             msg = "Wrong data type"
             self.logger.warning(msg)
             raise BUIserverException(msg)
         vers = self._get_agent_version()
@@ -595,16 +594,16 @@
         }
         return json.loads(self.do_command(data))
 
     @implement
     def store_conf_srv(self, data, conf=None, agent=None):
         """See :func:`burpui.misc.backend.interface.BUIbackend.store_conf_srv`"""
         # serialize data as it is a nested dict
-        import hmac
         import hashlib
+        import hmac
         from base64 import b64encode
 
         if not isinstance(data, (_ImmutableMultiDict, ImmutableMultiDict)):
             msg = "Wrong data type"
             self.logger.warning(msg)
             raise BUIserverException(msg)
         vers = self._get_agent_version()
```

### Comparing `burp-ui-1.0.0/burpui/misc/backend/parallel.py` & `burp-ui-1.1.0/burpui/misc/backend/parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 .. module:: burpui.misc.backend.parallel
     :platform: Unix
     :synopsis: Burp-UI parallel backend module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
+import json
 import os
 import re
-import json
 import ssl
-import time
-import trio
 import struct
-
+import time
 from asyncio import iscoroutinefunction
 from functools import partial
 
-from .burp2 import Burp as Burp2
-from .interface import BUIbackend, BUIBACKEND_INTERFACE_METHODS
-from .utils.constant import BURP_STATUS_FORMAT_V2
-from ..parser.burp2 import Parser
-from ...exceptions import BUIserverException
+import trio
+
+from ..._compat import to_bytes, to_unicode
 from ...decorators import implement, usetriorun
-from ...utils import utc_to_local
-from ..._compat import to_unicode, to_bytes
+from ...exceptions import BUIserverException
 from ...tools.logging import logger
+from ...utils import utc_to_local
+from ..parser.burp2 import Parser
+from .burp2 import Burp as Burp2
+from .interface import BUIBACKEND_INTERFACE_METHODS, BUIbackend
+from .utils.constant import BURP_STATUS_FORMAT_V2
 
 BUI_DEFAULTS = {
     "Parallel": {
         "host": "::1",
         "port": 11111,
         "ssl": True,
         "password": "password123456",
@@ -132,15 +132,14 @@
                 result = await self._do_process(data)
             self.connected = False
         else:
             result = await self._do_process(data)
         return result
 
     async def status(self, query, timeout=None, cache=True):
-
         request = {
             "query": query,
             "timeout": timeout,
             "cache": cache,
             "password": self.password,
         }
         request = json.dumps(request)
```

### Comparing `burp-ui-1.0.0/burpui/misc/backend/utils/burp2.py` & `burp-ui-1.1.0/burpui/misc/backend/utils/burp2.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 .. module:: burpui.misc.backend.utils.burp2
     :platform: Unix
     :synopsis: Burp-UI burp utils module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
+import datetime
+import json
 import re
 import subprocess
-import json
-import datetime
-
 from select import select
 
 from ...._compat import to_bytes, to_unicode
 from ....exceptions import BUIserverException
 from ....security import sanitize_string
 from ....tools.logging import logger
 from .constant import (
     BURP_LIST_BATCH,
     BURP_MINIMAL_VERSION,
-    BURP_STATUS_FORMAT_V2,
     BURP_STATUS_DELIMITER,
+    BURP_STATUS_FORMAT_V2,
 )
 
 
 class Monitor(object):
     """The :class:`burpui.misc.backend.utils.burp2.Monitor` class provides a ``burp-2``
     Monitor object to interact with the server.
```

### Comparing `burp-ui-1.0.0/burpui/misc/parser/.ropeproject/config.py` & `burp-ui-1.1.0/burpui/misc/parser/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/misc/parser/burp1.py` & `burp-ui-1.1.0/burpui/misc/parser/burp1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # -*- coding: utf8 -*-
 """
 .. module:: burpui.misc.parser.burp1
     :platform: Unix
     :synopsis: Burp-UI configuration file parser for Burp1.
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 """
-import re
-import os
-import json
 import codecs
+import json
+import os
+import re
 import shutil
-
 from glob import glob
 
-from .doc import Doc
-from .utils import Config
-from .openssl import OSSLConf, OSSLAuth
 from ...exceptions import BUIserverException
 from ...utils import NOTIF_ERROR, NOTIF_OK, NOTIF_WARN
+from .doc import Doc
+from .openssl import OSSLAuth, OSSLConf
+from .utils import Config
 
 
 class Parser(Doc):
     """:class:`burpui.misc.parser.burp1.Parser` provides a consistent interface
     to parse burp configuration files.
 
     It implements :class:`burpui.misc.parser.interface.BUIparser`.
```

### Comparing `burp-ui-1.0.0/burpui/misc/parser/burp2.py` & `burp-ui-1.1.0/burpui/misc/parser/burp2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf8 -*-
 """
 .. module:: burpui.misc.parser.burp2
     :platform: Unix
     :synopsis: Burp-UI configuration file parser for Burp2.
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 """
+from ..backend.utils.constant import BURP_BIND_MULTIPLE, BURP_LISTEN_OPTION
 from .burp1 import Parser as Burp1
-from ..backend.utils.constant import BURP_LISTEN_OPTION, BURP_BIND_MULTIPLE
 
 
 def __(string):
     """dummy function to fake the translation"""
     return string
```

### Comparing `burp-ui-1.0.0/burpui/misc/parser/doc.py` & `burp-ui-1.1.0/burpui/misc/parser/doc.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/misc/parser/interface.py` & `burp-ui-1.1.0/burpui/misc/parser/interface.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/misc/parser/openssl.py` & `burp-ui-1.1.0/burpui/misc/parser/openssl.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf8 -*-
 """
 .. module:: burpui.misc.parser.openssl
     :platform: Unix
     :synopsis: Burp-UI configuration file parser OpenSSL configuration.
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 """
+import codecs
 import os
 import re
-import codecs
 import subprocess
-
 from hashlib import md5
+
 from OpenSSL import crypto
 
 from ...tools.logging import logger
 
 
 class OSSLAuth(object):
     """OpenSSL wrapper"""
```

### Comparing `burp-ui-1.0.0/burpui/misc/parser/utils.py` & `burp-ui-1.1.0/burpui/misc/parser/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,26 @@
 """
 .. module:: burpui.misc.parser.utils
     :platform: Unix
     :synopsis: Burp-UI configuration file parser utilities.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 """
+import codecs
 import os
 import re
-import codecs
 import shutil
-
-from copy import copy
-from hashlib import md5
 from collections import OrderedDict
+from copy import copy
 from glob import glob
+from hashlib import md5
 
-from ...utils import NOTIF_ERROR, NOTIF_OK, NOTIF_WARN
-from ...security import sanitize_string
 from ...datastructures import MultiDict
-
+from ...security import sanitize_string
+from ...utils import NOTIF_ERROR, NOTIF_OK, NOTIF_WARN
 
 RESET_IDENTIFIER = "_reset_bui_CUSTOM"
 BEGIN_TEMPLATES = "BURP-UI TEMPLATES"
 END_TEMPLATES = "END TEMPLATES"
 
 
 class Option(object):
@@ -1510,15 +1508,14 @@
     def changed(self):
         for path, conf in self.files.items():
             if conf.changed:
                 return True
         return False
 
     def _parse(self):
-
         orig = self.files.copy()
         for root, conf in orig.items():
             conf.parse()
             for key, val in conf.flatten("include", False).items():
                 for path in val:
                     if not os.path.isabs(path):
                         path = os.path.join(os.path.dirname(root), path)
```

### Comparing `burp-ui-1.0.0/burpui/models.py` & `burp-ui-1.1.0/burpui/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,18 @@
     :synopsis: Burp-UI DB models module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
 import datetime
 
-from .ext.sql import db
 from flask import current_app, session
+
 from .engines.server import BUIServer  # noqa
+from .ext.sql import db
 
 app = current_app  # type: BUIServer
 
 
 class Task(db.Model):
     id = db.Column(db.Integer, primary_key=True)
     uuid = db.Column(db.String(256), unique=True)
```

### Comparing `burp-ui-1.0.0/burpui/plugins.py` & `burp-ui-1.1.0/burpui/plugins.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/routes.py` & `burp-ui-1.1.0/burpui/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,42 +3,42 @@
 .. module:: burpui.routes
     :platform: Unix
     :synopsis: Burp-UI routes module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-import re
 import math
+import re
 import uuid
 
 from flask import (
-    request,
-    render_template,
-    redirect,
-    url_for,
-    abort,
-    flash,
     Blueprint,
-    session,
+    abort,
     current_app,
+    flash,
     g,
+    redirect,
+    render_template,
+    request,
+    session,
+    url_for,
 )
-from flask_login import login_user, login_required, logout_user, current_user
-from flask_babel import gettext as _, refresh as refresh_babel
+from flask_babel import gettext as _
+from flask_babel import refresh as refresh_babel
+from flask_login import current_user, login_required, login_user, logout_user
 
-from .desc import __url__, __doc__
-from .engines.server import BUIServer  # noqa
-from .sessions import session_manager
 from ._compat import quote
-from .forms import LoginForm
+from .desc import __doc__, __url__
+from .engines.server import BUIServer  # noqa
 from .exceptions import BUIserverException
+from .forms import LoginForm
+from .security import is_safe_url, sanitize_string
+from .sessions import session_manager
 from .utils import human_readable as _hr
-from .security import sanitize_string, is_safe_url
-
 
 bui = current_app  # type: BUIServer
 view = Blueprint("view", "burpui", template_folder="templates")
 
 
 """
 Here are some custom filters
```

### Comparing `burp-ui-1.0.0/burpui/security.py` & `burp-ui-1.1.0/burpui/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 .. module:: burpui.security
     :platform: Unix
     :synopsis: Burp-UI security module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-from ._compat import to_unicode, urlparse, urljoin
+from ._compat import to_unicode, urljoin, urlparse
 
 
 def sanitize_string(string, strict=True, paranoid=False):
     """Return a 'safe' version of the string (ie. remove malicious chars like
     '\n')
 
     :param string: String to escape
@@ -41,24 +41,25 @@
     :type app: :class:`burpui.engines.server.BUIServer`
     """
     if app.auth != "none":
         if request.headers.get("X-From-UI", False):
             return None
         auth = request.authorization
         if auth:
-            from flask import session, g
+            from flask import g, session
 
             app.logger.debug("Found Basic user: {}".format(auth.username))
             refresh = True
             if "login" in session and session["login"] == auth.username:
                 refresh = False
             session["language"] = request.headers.get("X-Language", "en")
             user = app.uhandler.user(auth.username, refresh)
             if user and user.active and user.login(auth.password):
                 from flask_login import login_user
+
                 from .sessions import session_manager
 
                 if "login" in session and session["login"] != auth.username:
                     session.clear()
                     session["login"] = auth.username
                     session["language"] = request.headers.get("X-Language", "en")
                 login_user(user)
```

### Comparing `burp-ui-1.0.0/burpui/sessions.py` & `burp-ui-1.1.0/burpui/sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 .. module:: burpui.sessions
     :platform: Unix
     :synopsis: Burp-UI sessions module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
+import datetime
 import re
 import uuid
-import datetime
 
-from flask import session, request
+from flask import request, session
 
 # used for completion
 try:
     from redis import Redis  # noqa
 except ImportError:  # pragma: no cover
     pass
```

### Comparing `burp-ui-1.0.0/burpui/static/3rdparty/highlightjs/highlight.pack.js` & `burp-ui-1.1.0/burpui/static/3rdparty/highlightjs/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/3rdparty/highlightjs/style.css` & `burp-ui-1.1.0/burpui/static/3rdparty/highlightjs/style.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/dashboard.css` & `burp-ui-1.1.0/burpui/static/dashboard.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/extra/i18n/datatable-es.json` & `burp-ui-1.1.0/burpui/static/extra/i18n/datatable-es.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/extra/i18n/datatable-fr.json` & `burp-ui-1.1.0/burpui/static/extra/i18n/datatable-fr.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/extra/i18n/datatable-it.json` & `burp-ui-1.1.0/burpui/static/extra/i18n/datatable-it.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/images/favicon.ico` & `burp-ui-1.1.0/burpui/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/ace-builds/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/ace-builds/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/ace-builds/package.json` & `burp-ui-1.1.0/burpui/static/vendor/ace-builds/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/ace-builds/src-min-noconflict/ace.js` & `burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/ace.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/ace-builds/src-min-noconflict/mode-json.js` & `burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/mode-json.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/ace-builds/src-min-noconflict/theme-ambiance.js` & `burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/theme-ambiance.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/ace-builds/src-min-noconflict/worker-json.js` & `burp-ui-1.1.0/burpui/static/vendor/ace-builds/src-min-noconflict/worker-json.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular/angular.min.js` & `burp-ui-1.1.0/burpui/static/vendor/angular/angular.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular/package.json` & `burp-ui-1.1.0/burpui/static/vendor/angular/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-animate/angular-animate.min.js` & `burp-ui-1.1.0/burpui/static/vendor/angular-animate/angular-animate.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-animate/package.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-animate/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap/package.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap/ui-bootstrap-tpls.min.js` & `burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/ui-bootstrap-tpls.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap/ui-bootstrap.min.js` & `burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap/ui-bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap-switch/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap-switch/dist/angular-bootstrap-switch.min.js` & `burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/dist/angular-bootstrap-switch.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-bootstrap-switch/package.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-bootstrap-switch/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-datatables-0.6.2/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-datatables-0.6.2/dist/angular-datatables.min.js` & `burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/dist/angular-datatables.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-datatables-0.6.2/package.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-datatables-0.6.2/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-highlightjs/build/angular-highlightjs.min.js` & `burp-ui-1.1.0/burpui/static/vendor/angular-highlightjs/build/angular-highlightjs.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-onbeforeunload/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-onbeforeunload/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-onbeforeunload/build/angular-onbeforeunload.js` & `burp-ui-1.1.0/burpui/static/vendor/angular-onbeforeunload/build/angular-onbeforeunload.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-resource/angular-resource.min.js` & `burp-ui-1.1.0/burpui/static/vendor/angular-resource/angular-resource.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-resource/package.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-resource/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-route/angular-route.min.js` & `burp-ui-1.1.0/burpui/static/vendor/angular-route/angular-route.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-route/package.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-route/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-sanitize/angular-sanitize.min.js` & `burp-ui-1.1.0/burpui/static/vendor/angular-sanitize/angular-sanitize.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-sanitize/package.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-sanitize/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-strap/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-strap/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-strap/dist/angular-strap.min.js` & `burp-ui-1.1.0/burpui/static/vendor/angular-strap/dist/angular-strap.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-strap/dist/angular-strap.tpl.min.js` & `burp-ui-1.1.0/burpui/static/vendor/angular-strap/dist/angular-strap.tpl.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-strap/package.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-strap/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-ui-calendar/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-ui-calendar/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-ui-calendar/src/calendar.js` & `burp-ui-1.1.0/burpui/static/vendor/angular-ui-calendar/src/calendar.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-ui-select/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-ui-select/dist/select.min.css` & `burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/dist/select.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-ui-select/dist/select.min.js` & `burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/dist/select.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-ui-select/package.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-ui-select/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/angular-ui-select3/package.json` & `burp-ui-1.1.0/burpui/static/vendor/angular-ui-select3/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/bootstrap/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/bootstrap/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/bootstrap/dist/js/bootstrap.min.js` & `burp-ui-1.1.0/burpui/static/vendor/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/bootstrap/package.json` & `burp-ui-1.1.0/burpui/static/vendor/bootstrap/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/bootstrap-switch/dist/css/bootstrap3/bootstrap-switch.min.css` & `burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/css/bootstrap3/bootstrap-switch.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/bootstrap-switch/dist/js/bootstrap-switch.min.js` & `burp-ui-1.1.0/burpui/static/vendor/bootstrap-switch/dist/js/bootstrap-switch.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/bootswatch/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/bootswatch/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.eot` & `burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.svg` & `burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.ttf` & `burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff` & `burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff2` & `burp-ui-1.1.0/burpui/static/vendor/bootswatch/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/bootswatch/slate/bootstrap.min.css` & `burp-ui-1.1.0/burpui/static/vendor/bootswatch/slate/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/css/font-awesome.min.css` & `burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/fonts/FontAwesome.otf` & `burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.eot` & `burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.svg` & `burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.ttf` & `burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff` & `burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff2` & `burp-ui-1.1.0/burpui/static/vendor/components-font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/d3/d3.min.js` & `burp-ui-1.1.0/burpui/static/vendor/d3/d3.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net/js/jquery.dataTables.min.js` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-bs/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-bs/css/dataTables.bootstrap.min.css` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/css/dataTables.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-bs/js/dataTables.bootstrap.min.js` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-bs/js/dataTables.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-buttons/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-buttons/js/dataTables.buttons.min.js` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons/js/dataTables.buttons.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-buttons-bs/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-buttons-bs/css/buttons.bootstrap.min.css` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/css/buttons.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-buttons-bs/js/buttons.bootstrap.min.js` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-buttons-bs/js/buttons.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-fixedheader/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-fixedheader/js/dataTables.fixedHeader.min.js` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader/js/dataTables.fixedHeader.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-fixedheader-bs/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-fixedheader-bs/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-responsive/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-responsive/js/dataTables.responsive.min.js` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive/js/dataTables.responsive.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-responsive-bs/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-responsive-bs/css/responsive.bootstrap.min.css` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/css/responsive.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-responsive-bs/js/responsive.bootstrap.min.js` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-responsive-bs/js/responsive.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-select/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-select/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-select/js/dataTables.select.min.js` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-select/js/dataTables.select.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-select-bs/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-select-bs/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/datatables.net-select-bs/css/select.bootstrap.min.css` & `burp-ui-1.1.0/burpui/static/vendor/datatables.net-select-bs/css/select.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/fullcalendar/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.css` & `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.js` & `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.print.min.css` & `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/fullcalendar.print.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/gcal.min.js` & `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/gcal.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/locale/es.js` & `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/locale/es.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/locale/fr.js` & `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/locale/fr.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/fullcalendar/dist/locale/it.js` & `burp-ui-1.1.0/burpui/static/vendor/fullcalendar/dist/locale/it.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/jquery/dist/jquery.min.js` & `burp-ui-1.1.0/burpui/static/vendor/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/jquery-file-download/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/jquery-file-download/src/Scripts/jquery.fileDownload.js` & `burp-ui-1.1.0/burpui/static/vendor/jquery-file-download/src/Scripts/jquery.fileDownload.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/jquery-ui/jquery-ui.min.js` & `burp-ui-1.1.0/burpui/static/vendor/jquery-ui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/jquery-ui/package.json` & `burp-ui-1.1.0/burpui/static/vendor/jquery-ui/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/jquery.fancytree/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/jquery.fancytree/dist/jquery.fancytree-all.min.js` & `burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/dist/jquery.fancytree-all.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/jquery.fancytree/dist/skin-bootstrap/ui.fancytree.min.css` & `burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/dist/skin-bootstrap/ui.fancytree.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/jquery.fancytree/package.json` & `burp-ui-1.1.0/burpui/static/vendor/jquery.fancytree/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/jquery.floatThead/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/jquery.floatThead/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/jquery.floatThead/dist/jquery.floatThead.min.js` & `burp-ui-1.1.0/burpui/static/vendor/jquery.floatThead/dist/jquery.floatThead.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/js-cookie/src/js.cookie.js` & `burp-ui-1.1.0/burpui/static/vendor/js-cookie/src/js.cookie.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/lodash/dist/lodash.min.js` & `burp-ui-1.1.0/burpui/static/vendor/lodash/dist/lodash.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/lodash/package.json` & `burp-ui-1.1.0/burpui/static/vendor/lodash/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/moment/locale/es.js` & `burp-ui-1.1.0/burpui/static/vendor/moment/locale/es.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/moment/locale/fr.js` & `burp-ui-1.1.0/burpui/static/vendor/moment/locale/fr.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/moment/locale/it.js` & `burp-ui-1.1.0/burpui/static/vendor/moment/locale/it.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/moment/min/moment.min.js` & `burp-ui-1.1.0/burpui/static/vendor/moment/min/moment.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/moment-timezone/builds/moment-timezone-with-data-10-year-range.min.js` & `burp-ui-1.1.0/burpui/static/vendor/moment-timezone/builds/moment-timezone-with-data-10-year-range.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/nvd3/bower.json` & `burp-ui-1.1.0/burpui/static/vendor/nvd3/bower.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/nvd3/build/nv.d3.min.css` & `burp-ui-1.1.0/burpui/static/vendor/nvd3/build/nv.d3.min.css`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/nvd3/build/nv.d3.min.js` & `burp-ui-1.1.0/burpui/static/vendor/nvd3/build/nv.d3.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/select2/package.json` & `burp-ui-1.1.0/burpui/static/vendor/select2/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/socket.io-client/dist/socket.io.min.js` & `burp-ui-1.1.0/burpui/static/vendor/socket.io-client/dist/socket.io.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/socket.io-client/package.json` & `burp-ui-1.1.0/burpui/static/vendor/socket.io-client/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/typeahead.js/dist/typeahead.jquery.min.js` & `burp-ui-1.1.0/burpui/static/vendor/typeahead.js/dist/typeahead.jquery.min.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/static/vendor/typeahead.js/package.json` & `burp-ui-1.1.0/burpui/static/vendor/typeahead.js/package.json`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/tasks.py` & `burp-ui-1.1.0/burpui/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 .. module:: burpui.tasks
     :platform: Unix
     :synopsis: Burp-UI tasks module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 """
 import os
+from datetime import datetime, timedelta
+from time import gmtime, sleep, strftime
 
-from flask import current_app
-from datetime import timedelta, datetime
 from celery.schedules import crontab
 from celery.utils.log import get_task_logger
-from time import gmtime, strftime, sleep
+from flask import current_app
 
 from burpui._compat import to_unicode  # noqa
+from burpui.api.client import ClientTreeAll  # noqa
 from burpui.config import config  # noqa
-from burpui.ext.tasks import celery  # noqa
-from burpui.ext.cache import cache  # noqa
-from burpui.sessions import session_manager  # noqa
 from burpui.engines.server import BUIServer  # noqa
 from burpui.exceptions import BUIserverException, TooManyRecordsException  # noqa
-from burpui.api.client import ClientTreeAll  # noqa
+from burpui.ext.cache import cache  # noqa
+from burpui.ext.tasks import celery  # noqa
+from burpui.sessions import session_manager  # noqa
 from burpui.utils import NOTIF_ERROR
 
 try:
     from burpui.ext.ws import socketio
 
     WS_AVAILABLE = True
 except ImportError:
```

### Comparing `burp-ui-1.0.0/burpui/templates/.ropeproject/config.py` & `burp-ui-1.1.0/burpui/templates/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/about.html` & `burp-ui-1.1.0/burpui/templates/about.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/admin/authentication.html` & `burp-ui-1.1.0/burpui/templates/admin/authentication.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/admin/grant-authorization.html` & `burp-ui-1.1.0/burpui/templates/admin/grant-authorization.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/admin/group-authorization.html` & `burp-ui-1.1.0/burpui/templates/admin/group-authorization.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/admin/sessions.html` & `burp-ui-1.1.0/burpui/templates/admin/sessions.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/admin-authentications.html` & `burp-ui-1.1.0/burpui/templates/admin-authentications.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/admin-authorizations.html` & `burp-ui-1.1.0/burpui/templates/admin-authorizations.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/admin-backends.html` & `burp-ui-1.1.0/burpui/templates/admin-backends.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/backup-report.html` & `burp-ui-1.1.0/burpui/templates/backup-report.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/calendar.html` & `burp-ui-1.1.0/burpui/templates/calendar.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/client-browse.html` & `burp-ui-1.1.0/burpui/templates/client-browse.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/client-report.html` & `burp-ui-1.1.0/burpui/templates/client-report.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/client.html` & `burp-ui-1.1.0/burpui/templates/client.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/clients-report.html` & `burp-ui-1.1.0/burpui/templates/clients-report.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/clients.html` & `burp-ui-1.1.0/burpui/templates/clients.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/gerard.js` & `burp-ui-1.1.0/burpui/templates/gerard.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/about.js` & `burp-ui-1.1.0/burpui/templates/js/about.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/admin/authentication.js` & `burp-ui-1.1.0/burpui/templates/js/admin/authentication.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/admin/grant-authorization.js` & `burp-ui-1.1.0/burpui/templates/js/admin/grant-authorization.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/admin/group-authorization.js` & `burp-ui-1.1.0/burpui/templates/js/admin/group-authorization.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/admin/sessions.js` & `burp-ui-1.1.0/burpui/templates/js/admin/sessions.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/admin-authentications.js` & `burp-ui-1.1.0/burpui/templates/js/admin-authentications.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/admin-authorizations.js` & `burp-ui-1.1.0/burpui/templates/js/admin-authorizations.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/admin-backends.js` & `burp-ui-1.1.0/burpui/templates/js/admin-backends.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/backup-report.js` & `burp-ui-1.1.0/burpui/templates/js/backup-report.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/calendar.js` & `burp-ui-1.1.0/burpui/templates/js/calendar.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/client-browse.js` & `burp-ui-1.1.0/burpui/templates/js/client-browse.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/client-report.js` & `burp-ui-1.1.0/burpui/templates/js/client-report.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/client.js` & `burp-ui-1.1.0/burpui/templates/js/client.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/clients-report.js` & `burp-ui-1.1.0/burpui/templates/js/clients-report.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/clients.js` & `burp-ui-1.1.0/burpui/templates/js/clients.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/live-monitor.js` & `burp-ui-1.1.0/burpui/templates/js/live-monitor.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/servers-report.js` & `burp-ui-1.1.0/burpui/templates/js/servers-report.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/servers.js` & `burp-ui-1.1.0/burpui/templates/js/servers.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/settings.js` & `burp-ui-1.1.0/burpui/templates/js/settings.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/js/user.js` & `burp-ui-1.1.0/burpui/templates/js/user.js`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/layout.html` & `burp-ui-1.1.0/burpui/templates/layout.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/live-monitor.html` & `burp-ui-1.1.0/burpui/templates/live-monitor.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/login.html` & `burp-ui-1.1.0/burpui/templates/login.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/macros.html` & `burp-ui-1.1.0/burpui/templates/macros.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/notifications.html` & `burp-ui-1.1.0/burpui/templates/notifications.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/servers-report.html` & `burp-ui-1.1.0/burpui/templates/servers-report.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/servers.html` & `burp-ui-1.1.0/burpui/templates/servers.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/settings.html` & `burp-ui-1.1.0/burpui/templates/settings.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/sideadmin.html` & `burp-ui-1.1.0/burpui/templates/sideadmin.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/sidebar.html` & `burp-ui-1.1.0/burpui/templates/sidebar.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/sideconfig.html` & `burp-ui-1.1.0/burpui/templates/sideconfig.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/sideuser.html` & `burp-ui-1.1.0/burpui/templates/sideuser.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/small_topbar.html` & `burp-ui-1.1.0/burpui/templates/small_topbar.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/topbar.html` & `burp-ui-1.1.0/burpui/templates/topbar.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/templates/user.html` & `burp-ui-1.1.0/burpui/templates/user.html`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/thirdparty/flask_bower.py` & `burp-ui-1.1.0/burpui/thirdparty/flask_bower.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,17 +338,18 @@
 This General Public License does not permit incorporating your program into
 proprietary programs.  If your program is a subroutine library, you may
 consider it more useful to permit linking proprietary applications with the
 library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.
 """
 import os
-from flask import abort, json, send_file, Blueprint, current_app, url_for
 import sys
 
+from flask import Blueprint, abort, current_app, json, send_file, url_for
+
 
 def validate_parameter(param):
     if ".." in param or param.startswith("/"):
         abort(404)
 
 
 def serve(component, filename):
@@ -417,15 +418,14 @@
     See http://flask.pocoo.org/docs/0.10/api/#flask.url_for
     """
     default_url_for_args = values.copy()
     if filename:
         default_url_for_args["filename"] = filename
 
     if endpoint == "static" or endpoint.endswith(".static"):
-
         if os.path.sep in filename:
             filename_parts = filename.split(os.path.sep)
             component = filename_parts[0]
             # Using * magic here to expand list
             filename = os.path.join(*filename_parts[1:])
 
             returned_url = build_url(component, filename, **values)
```

### Comparing `burp-ui-1.0.0/burpui/tools/logging.py` & `burp-ui-1.1.0/burpui/tools/logging.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/translations/es/LC_MESSAGES/messages.mo` & `burp-ui-1.1.0/burpui/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/translations/es/LC_MESSAGES/messages.po` & `burp-ui-1.1.0/burpui/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/translations/fr/LC_MESSAGES/messages.mo` & `burp-ui-1.1.0/burpui/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/translations/fr/LC_MESSAGES/messages.po` & `burp-ui-1.1.0/burpui/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/translations/it/LC_MESSAGES/messages.mo` & `burp-ui-1.1.0/burpui/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/translations/it/LC_MESSAGES/messages.po` & `burp-ui-1.1.0/burpui/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/burpui/utils.py` & `burp-ui-1.1.0/burpui/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 .. module:: burpui.utils
     :platform: Unix
     :synopsis: Burp-UI utils module.
 
 .. moduleauthor:: Ziirish <hi+burpui@ziirish.me>
 
 """
-import os
+import datetime
 import math
+import os
 import string
 import sys
-import datetime
-import zipfile
 import tarfile
-
+import zipfile
 from uuid import UUID
 
 NOTIF_OK = 0
 NOTIF_WARN = 1
 NOTIF_ERROR = 2
 NOTIF_INFO = 3
```

### Comparing `burp-ui-1.0.0/burpui/ws/namespace.py` & `burp-ui-1.1.0/burpui/ws/namespace.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/contrib/centos/init.sh` & `burp-ui-1.1.0/contrib/centos/init.sh`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/contrib/freebsd/gunicorn.rc` & `burp-ui-1.1.0/contrib/freebsd/gunicorn.rc`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/contrib/gunicorn/burpui_gunicorn.py` & `burp-ui-1.1.0/contrib/gunicorn/burpui_gunicorn.py`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/migrations/alembic.ini` & `burp-ui-1.1.0/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/migrations/env.py` & `burp-ui-1.1.0/migrations/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import with_statement
+
+import logging
+from logging.config import fileConfig
+
 from alembic import context
 from sqlalchemy import engine_from_config, pool
-from logging.config import fileConfig
-import logging
 
 # this is the Alembic Config object, which provides
 # access to the values within the .ini file in use.
 config = context.config
 
 # Interpret the config file for Python logging.
 # This line sets up loggers basically.
```

### Comparing `burp-ui-1.0.0/migrations/versions/225d9b2f0fb1_initial.py` & `burp-ui-1.1.0/migrations/versions/225d9b2f0fb1_initial.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 """
 
 # revision identifiers, used by Alembic.
 revision = "225d9b2f0fb1"
 down_revision = None
 
-from alembic import op
 import sqlalchemy as sa
+from alembic import op
 
 
 def upgrade():
     ### commands auto generated by Alembic - please adjust! ###
     op.create_table(
         "task",
         sa.Column("id", sa.Integer(), nullable=False),
```

### Comparing `burp-ui-1.0.0/migrations/versions/4445080944ee_hidden_hosts_management.py` & `burp-ui-1.1.0/migrations/versions/4445080944ee_hidden_hosts_management.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 """
 
 # revision identifiers, used by Alembic.
 revision = "4445080944ee"
 down_revision = "695dcbd29d4f"
 
-from alembic import op
 import sqlalchemy as sa
+from alembic import op
 
 
 def upgrade():
     # ### commands auto generated by Alembic - please adjust! ###
     op.create_table(
         "hidden",
         sa.Column("id", sa.Integer(), nullable=False),
```

### Comparing `burp-ui-1.0.0/migrations/versions/56de018f4d88_user_prefs.py` & `burp-ui-1.1.0/migrations/versions/56de018f4d88_user_prefs.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 """
 
 # revision identifiers, used by Alembic.
 revision = "56de018f4d88"
 down_revision = "fc07e3fa0086"
 
-from alembic import op
 import sqlalchemy as sa
+from alembic import op
 
 
 def upgrade():
     ### commands auto generated by Alembic - please adjust! ###
     op.create_table(
         "pref",
         sa.Column("id", sa.Integer(), nullable=False),
```

### Comparing `burp-ui-1.0.0/migrations/versions/695dcbd29d4f_increase_pref_value_size.py` & `burp-ui-1.1.0/migrations/versions/695dcbd29d4f_increase_pref_value_size.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 """
 
 # revision identifiers, used by Alembic.
 revision = "695dcbd29d4f"
 down_revision = "56de018f4d88"
 
-from alembic import op
 import sqlalchemy as sa
+from alembic import op
 
 
 def upgrade():
     ### commands auto generated by Alembic - please adjust! ###
     with op.batch_alter_table("pref", schema=None) as batch_op:
         batch_op.alter_column(
             "value",
```

### Comparing `burp-ui-1.0.0/migrations/versions/7f317474332d_handle_sessions.py` & `burp-ui-1.1.0/migrations/versions/7f317474332d_handle_sessions.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 """
 
 # revision identifiers, used by Alembic.
 revision = "7f317474332d"
 down_revision = "225d9b2f0fb1"
 
-from alembic import op
 import sqlalchemy as sa
+from alembic import op
 
 
 def upgrade():
     ### commands auto generated by Alembic - please adjust! ###
     op.create_table(
         "session",
         sa.Column("id", sa.Integer(), nullable=False),
```

### Comparing `burp-ui-1.0.0/migrations/versions/fc07e3fa0086_sql_compatibility.py` & `burp-ui-1.1.0/migrations/versions/fc07e3fa0086_sql_compatibility.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 """
 
 # revision identifiers, used by Alembic.
 revision = "fc07e3fa0086"
 down_revision = "7f317474332d"
 
-from alembic import op
 import sqlalchemy as sa
+from alembic import op
 
 
 def upgrade():
     ### commands auto generated by Alembic - please adjust! ###
     with op.batch_alter_table("session", schema=None) as batch_op:
         batch_op.alter_column(
             "ip",
```

### Comparing `burp-ui-1.0.0/setup.py` & `burp-ui-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import os
 import sys
-
-from subprocess import check_output, call, STDOUT
 from distutils import log
 from distutils.core import Command
-from setuptools import setup, find_packages
-from setuptools.command.develop import develop
-from setuptools.command.sdist import sdist
-from setuptools.command.install import install
+from subprocess import STDOUT, call, check_output
+
+from setuptools import find_packages, setup
 from setuptools.command.bdist_egg import bdist_egg
+from setuptools.command.develop import develop
 from setuptools.command.egg_info import egg_info
+from setuptools.command.install import install
+from setuptools.command.sdist import sdist
 
 ROOT = os.path.join(os.path.dirname(os.path.realpath(__file__)))
 DEVNULL = open(os.devnull, "wb")
 
 # Not sure bower was a great idea...
 VENDOR_TO_KEEP = [
     "burpui/static/vendor/bootswatch/slate/bootstrap.min.css",
@@ -241,21 +241,16 @@
                 continue
             desc += line
     return desc
 
 
 sys.path.insert(0, os.path.join(ROOT))
 
-from burpui.desc import (
-    __author__,
-    __author_email__,
-    __description__,
-    __url__,
-    __title__,
-)  # noqa
+from burpui.desc import __description__  # noqa
+from burpui.desc import __author__, __author_email__, __title__, __url__
 
 name = __title__
 author = __author__
 author_email = __author_email__
 description = __description__
 url = __url__
```

### Comparing `burp-ui-1.0.0/share/burpui/etc/buimonitor.sample.cfg` & `burp-ui-1.1.0/share/burpui/etc/buimonitor.sample.cfg`

 * *Files identical despite different names*

### Comparing `burp-ui-1.0.0/share/burpui/etc/burpui.sample.cfg` & `burp-ui-1.1.0/share/burpui/etc/burpui.sample.cfg`

 * *Files identical despite different names*

