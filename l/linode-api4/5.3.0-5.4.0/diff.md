# Comparing `tmp/linode_api4-5.3.0.tar.gz` & `tmp/linode_api4-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linode_api4-5.3.0.tar", last modified: Fri Sep 30 14:55:11 2022, max compression
+gzip compressed data, was "linode_api4-5.4.0.tar", last modified: Mon May  1 17:35:25 2023, max compression
```

## Comparing `linode_api4-5.3.0.tar` & `linode_api4-5.4.0.tar`

### file list

```diff
@@ -1,118 +1,200 @@
-drwxr-xr-x   0 lgarber    (501) staff       (20)        0 2022-09-30 14:55:11.168202 linode_api4-5.3.0/
--rw-r--r--   0 lgarber    (501) staff       (20)     1482 2022-09-30 14:48:06.000000 linode_api4-5.3.0/LICENSE
--rw-r--r--   0 lgarber    (501) staff       (20)       32 2022-09-30 14:48:06.000000 linode_api4-5.3.0/MANIFEST.in
--rw-r--r--   0 lgarber    (501) staff       (20)     4412 2022-09-30 14:55:11.167534 linode_api4-5.3.0/PKG-INFO
--rw-r--r--   0 lgarber    (501) staff       (20)     3609 2022-09-30 14:48:06.000000 linode_api4-5.3.0/README.rst
-drwxr-xr-x   0 lgarber    (501) staff       (20)        0 2022-09-30 14:55:11.037251 linode_api4-5.3.0/linode_api4/
--rw-r--r--   0 lgarber    (501) staff       (20)      271 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/__init__.py
--rw-r--r--   0 lgarber    (501) staff       (20)     1545 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/common.py
--rw-r--r--   0 lgarber    (501) staff       (20)     1079 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/errors.py
--rw-r--r--   0 lgarber    (501) staff       (20)    70459 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/linode_client.py
--rw-r--r--   0 lgarber    (501) staff       (20)    14828 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/login_client.py
-drwxr-xr-x   0 lgarber    (501) staff       (20)        0 2022-09-30 14:55:11.062281 linode_api4-5.3.0/linode_api4/objects/
--rw-r--r--   0 lgarber    (501) staff       (20)      526 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/__init__.py
--rw-r--r--   0 lgarber    (501) staff       (20)    11939 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/account.py
--rw-r--r--   0 lgarber    (501) staff       (20)    12703 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/base.py
--rw-r--r--   0 lgarber    (501) staff       (20)    11862 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/database.py
--rw-r--r--   0 lgarber    (501) staff       (20)      874 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/dbase.py
--rw-r--r--   0 lgarber    (501) staff       (20)     2123 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/domain.py
--rw-r--r--   0 lgarber    (501) staff       (20)     7440 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/filtering.py
--rw-r--r--   0 lgarber    (501) staff       (20)      610 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/image.py
--rw-r--r--   0 lgarber    (501) staff       (20)    32327 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/linode.py
--rw-r--r--   0 lgarber    (501) staff       (20)     5776 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/lke.py
--rw-r--r--   0 lgarber    (501) staff       (20)      683 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/longview.py
--rw-r--r--   0 lgarber    (501) staff       (20)     4382 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/networking.py
--rw-r--r--   0 lgarber    (501) staff       (20)     6413 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/nodebalancer.py
--rw-r--r--   0 lgarber    (501) staff       (20)      806 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/object_storage.py
--rw-r--r--   0 lgarber    (501) staff       (20)     3962 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/profile.py
--rw-r--r--   0 lgarber    (501) staff       (20)      315 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/region.py
--rw-r--r--   0 lgarber    (501) staff       (20)     3198 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/support.py
--rw-r--r--   0 lgarber    (501) staff       (20)     3873 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/tag.py
--rw-r--r--   0 lgarber    (501) staff       (20)     2252 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/objects/volume.py
--rw-r--r--   0 lgarber    (501) staff       (20)     7832 2022-09-30 14:48:06.000000 linode_api4-5.3.0/linode_api4/paginated_list.py
-drwxr-xr-x   0 lgarber    (501) staff       (20)        0 2022-09-30 14:55:11.040648 linode_api4-5.3.0/linode_api4.egg-info/
--rw-r--r--   0 lgarber    (501) staff       (20)     4412 2022-09-30 14:55:10.000000 linode_api4-5.3.0/linode_api4.egg-info/PKG-INFO
--rw-r--r--   0 lgarber    (501) staff       (20)     4121 2022-09-30 14:55:10.000000 linode_api4-5.3.0/linode_api4.egg-info/SOURCES.txt
--rw-r--r--   0 lgarber    (501) staff       (20)        1 2022-09-30 14:55:10.000000 linode_api4-5.3.0/linode_api4.egg-info/dependency_links.txt
--rw-r--r--   0 lgarber    (501) staff       (20)       21 2022-09-30 14:55:10.000000 linode_api4-5.3.0/linode_api4.egg-info/requires.txt
--rw-r--r--   0 lgarber    (501) staff       (20)       12 2022-09-30 14:55:10.000000 linode_api4-5.3.0/linode_api4.egg-info/top_level.txt
--rw-r--r--   0 lgarber    (501) staff       (20)       38 2022-09-30 14:55:11.168398 linode_api4-5.3.0/setup.cfg
--rwxr-xr-x   0 lgarber    (501) staff       (20)     2713 2022-09-30 14:50:14.000000 linode_api4-5.3.0/setup.py
-drwxr-xr-x   0 lgarber    (501) staff       (20)        0 2022-09-30 14:55:11.067645 linode_api4-5.3.0/test/
--rw-r--r--   0 lgarber    (501) staff       (20)        0 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/__init__.py
--rw-r--r--   0 lgarber    (501) staff       (20)     5252 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/base.py
-drwxr-xr-x   0 lgarber    (501) staff       (20)        0 2022-09-30 14:55:11.149021 linode_api4-5.3.0/test/fixtures/
--rw-r--r--   0 lgarber    (501) staff       (20)      398 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/account.json
--rw-r--r--   0 lgarber    (501) staff       (20)      186 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/account_invoices.json
--rw-r--r--   0 lgarber    (501) staff       (20)      283 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/account_invoices_123456_items.json
--rw-r--r--   0 lgarber    (501) staff       (20)      123 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/account_settings.json
--rw-r--r--   0 lgarber    (501) staff       (20)      253 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_engines.json
--rw-r--r--   0 lgarber    (501) staff       (20)      869 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_instances.json
--rw-r--r--   0 lgarber    (501) staff       (20)     1055 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_mongodb_instances.json
--rw-r--r--   0 lgarber    (501) staff       (20)      208 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_mongodb_instances_123_backups.json
--rw-r--r--   0 lgarber    (501) staff       (20)        2 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_mongodb_instances_123_backups_456_restore.json
--rw-r--r--   0 lgarber    (501) staff       (20)       59 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_mongodb_instances_123_credentials.json
--rw-r--r--   0 lgarber    (501) staff       (20)        2 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_mongodb_instances_123_credentials_reset.json
--rw-r--r--   0 lgarber    (501) staff       (20)        2 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_mongodb_instances_123_patch.json
--rw-r--r--   0 lgarber    (501) staff       (20)       43 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_mongodb_instances_123_ssl.json
--rw-r--r--   0 lgarber    (501) staff       (20)      900 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_mysql_instances.json
--rw-r--r--   0 lgarber    (501) staff       (20)      208 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_mysql_instances_123_backups.json
--rw-r--r--   0 lgarber    (501) staff       (20)        2 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_mysql_instances_123_backups_456_restore.json
--rw-r--r--   0 lgarber    (501) staff       (20)       59 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_mysql_instances_123_credentials.json
--rw-r--r--   0 lgarber    (501) staff       (20)        2 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_mysql_instances_123_credentials_reset.json
--rw-r--r--   0 lgarber    (501) staff       (20)        2 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_mysql_instances_123_patch.json
--rw-r--r--   0 lgarber    (501) staff       (20)       43 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_mysql_instances_123_ssl.json
--rw-r--r--   0 lgarber    (501) staff       (20)      941 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_postgresql_instances.json
--rw-r--r--   0 lgarber    (501) staff       (20)      208 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_postgresql_instances_123_backups.json
--rw-r--r--   0 lgarber    (501) staff       (20)        2 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_postgresql_instances_123_backups_456_restore.json
--rw-r--r--   0 lgarber    (501) staff       (20)       59 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_postgresql_instances_123_credentials.json
--rw-r--r--   0 lgarber    (501) staff       (20)        2 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_postgresql_instances_123_credentials_reset.json
--rw-r--r--   0 lgarber    (501) staff       (20)        2 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_postgresql_instances_123_patch.json
--rw-r--r--   0 lgarber    (501) staff       (20)       43 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_postgresql_instances_123_ssl.json
--rw-r--r--   0 lgarber    (501) staff       (20)      812 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/databases_types.json
--rw-r--r--   0 lgarber    (501) staff       (20)      440 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/domains.json
--rw-r--r--   0 lgarber    (501) staff       (20)     1546 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/images.json
--rw-r--r--   0 lgarber    (501) staff       (20)     1731 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/linode_instances.json
--rw-r--r--   0 lgarber    (501) staff       (20)     1788 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/linode_instances_123_backups.json
--rw-r--r--   0 lgarber    (501) staff       (20)     1076 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/linode_instances_123_configs.json
--rw-r--r--   0 lgarber    (501) staff       (20)      878 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/linode_instances_123_configs_456789.json
--rw-r--r--   0 lgarber    (501) staff       (20)      502 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/linode_instances_123_disks.json
--rw-r--r--   0 lgarber    (501) staff       (20)       56 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/linode_instances_123_transfer.json
--rw-r--r--   0 lgarber    (501) staff       (20)     1820 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/linode_types.json
--rw-r--r--   0 lgarber    (501) staff       (20)      222 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/lke_clusters.json
--rw-r--r--   0 lgarber    (501) staff       (20)      149 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/lke_versions.json
--rw-r--r--   0 lgarber    (501) staff       (20)      770 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/longview_clients.json
--rw-r--r--   0 lgarber    (501) staff       (20)      783 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/longview_subscriptions.json
--rw-r--r--   0 lgarber    (501) staff       (20)       43 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/mongodb.json
--rw-r--r--   0 lgarber    (501) staff       (20)      424 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/networking_firewalls.json
--rw-r--r--   0 lgarber    (501) staff       (20)      276 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/networking_firewalls_123.json
--rw-r--r--   0 lgarber    (501) staff       (20)      314 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/networking_firewalls_123_devices.json
--rw-r--r--   0 lgarber    (501) staff       (20)      212 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/networking_firewalls_123_devices_123.json
--rw-r--r--   0 lgarber    (501) staff       (20)       94 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/networking_firewalls_123_rules.json
--rw-r--r--   0 lgarber    (501) staff       (20)      226 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/networking_vlans.json
--rw-r--r--   0 lgarber    (501) staff       (20)      809 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/nodebalancers.json
--rw-r--r--   0 lgarber    (501) staff       (20)      660 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/nodebalancers_123456_configs.json
--rw-r--r--   0 lgarber    (501) staff       (20)      282 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/nodebalancers_123456_configs_65432_nodes.json
--rw-r--r--   0 lgarber    (501) staff       (20)      269 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/object-storage_clusters.json
--rw-r--r--   0 lgarber    (501) staff       (20)      350 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/object-storage_keys.json
--rw-r--r--   0 lgarber    (501) staff       (20)     1787 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/profile_sshkeys.json
--rw-r--r--   0 lgarber    (501) staff       (20)     6293 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/regions.json
--rw-r--r--   0 lgarber    (501) staff       (20)      140 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/tags.json
--rw-r--r--   0 lgarber    (501) staff       (20)       60 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/tags_nothing.json
--rw-r--r--   0 lgarber    (501) staff       (20)     2242 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/tags_something.json
--rw-r--r--   0 lgarber    (501) staff       (20)      831 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures/volumes.json
--rw-r--r--   0 lgarber    (501) staff       (20)     1253 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/fixtures.py
--rw-r--r--   0 lgarber    (501) staff       (20)    26595 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/linode_client_test.py
-drwxr-xr-x   0 lgarber    (501) staff       (20)        0 2022-09-30 14:55:11.166478 linode_api4-5.3.0/test/objects/
--rw-r--r--   0 lgarber    (501) staff       (20)        0 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/objects/__init__.py
--rw-r--r--   0 lgarber    (501) staff       (20)     1274 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/objects/account_test.py
--rw-r--r--   0 lgarber    (501) staff       (20)    19219 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/objects/database_test.py
--rw-r--r--   0 lgarber    (501) staff       (20)     2693 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/objects/firewall_test.py
--rw-r--r--   0 lgarber    (501) staff       (20)      820 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/objects/image_test.py
--rw-r--r--   0 lgarber    (501) staff       (20)    11358 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/objects/linode_test.py
--rw-r--r--   0 lgarber    (501) staff       (20)     2531 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/objects/longview_test.py
--rw-r--r--   0 lgarber    (501) staff       (20)     4205 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/objects/nodebalancers_test.py
--rw-r--r--   0 lgarber    (501) staff       (20)     2553 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/objects/profile_test.py
--rw-r--r--   0 lgarber    (501) staff       (20)     1331 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/objects/tag_test.py
--rw-r--r--   0 lgarber    (501) staff       (20)     2997 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/objects/volume_test.py
--rw-r--r--   0 lgarber    (501) staff       (20)     4123 2022-09-30 14:48:06.000000 linode_api4-5.3.0/test/paginated_list_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:35:25.631433 linode_api4-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-01 17:34:52.000000 linode_api4-5.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-01 17:34:52.000000 linode_api4-5.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-01 17:35:25.627433 linode_api4-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-01 17:34:52.000000 linode_api4-5.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 17:35:25.000000 linode_api4-5.4.0/baked_version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:35:25.595433 linode_api4-5.4.0/linode_api4/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:35:25.603433 linode_api4-5.4.0/linode_api4/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/linode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/lke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/longview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/nodebalancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/groups/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14516 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/linode_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14902 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/login_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:35:25.603433 linode_api4-5.4.0/linode_api4/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19006 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17892 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/dbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51940 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/linode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/lke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/longview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/nodebalancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/objects/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-01 17:34:52.000000 linode_api4-5.4.0/linode_api4/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:35:25.599433 linode_api4-5.4.0/linode_api4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-01 17:35:25.000000 linode_api4-5.4.0/linode_api4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-05-01 17:35:25.000000 linode_api4-5.4.0/linode_api4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 17:35:25.000000 linode_api4-5.4.0/linode_api4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 17:35:25.000000 linode_api4-5.4.0/linode_api4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-01 17:35:25.000000 linode_api4-5.4.0/linode_api4.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-01 17:34:52.000000 linode_api4-5.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 17:35:25.631433 linode_api4-5.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3818 2023-05-01 17:34:52.000000 linode_api4-5.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:35:25.607433 linode_api4-5.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:35:25.627433 linode_api4-5.4.0/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account.json
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_events_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_invoices.json
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_invoices_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_invoices_123456_items.json
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_logins.json
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_logins_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_maintenance.json
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_notifications.json
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_oauth-clients_2737bf16b39ab5d7b4a1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_payment-method_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_payment-methods.json
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_payments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_promo-codes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_service-transfers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_service-transfers_12345.json
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/account_users_test-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_engines.json
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_instances.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_mongodb_instances.json
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_mongodb_instances_123_backups.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_mongodb_instances_123_backups_456_restore.json
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_mongodb_instances_123_credentials.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_mongodb_instances_123_credentials_reset.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_mongodb_instances_123_patch.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_mongodb_instances_123_ssl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_mysql_instances.json
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_mysql_instances_123_backups.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_mysql_instances_123_backups_456_restore.json
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_mysql_instances_123_credentials.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_mysql_instances_123_credentials_reset.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_mysql_instances_123_patch.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_mysql_instances_123_ssl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_postgresql_instances.json
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_postgresql_instances_123_backups.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_postgresql_instances_123_backups_456_restore.json
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_postgresql_instances_123_credentials.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_postgresql_instances_123_credentials_reset.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_postgresql_instances_123_patch.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_postgresql_instances_123_ssl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/databases_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/domains.json
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/domains_12345_clone.json
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/domains_12345_records.json
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/domains_12345_zone-file.json
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/domains_import.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/images.json
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/images_private_1337.json
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/images_upload.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/linode_instances.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/linode_instances_123_backups.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/linode_instances_123_configs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/linode_instances_123_configs_456789.json
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/linode_instances_123_disks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/linode_instances_123_disks_12345_clone.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/linode_instances_123_firewalls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/linode_instances_123_ips.json
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/linode_instances_123_nodebalancers.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/linode_instances_123_transfer.json
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/linode_instances_123_transfer_2023_4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/linode_instances_123_volumes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/linode_stackscripts_10079.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/linode_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/lke_clusters.json
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/lke_clusters_18881.json
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/lke_clusters_18881_dashboard.json
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/lke_clusters_18881_nodes_123456.json
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/lke_clusters_18881_pools_456.json
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/lke_versions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/longview_clients.json
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/longview_plan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/longview_subscriptions.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/mongodb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/networking_firewalls.json
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/networking_firewalls_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/networking_firewalls_123_devices.json
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/networking_firewalls_123_devices_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/networking_firewalls_123_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/networking_ips_127.0.0.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/networking_ipv6_pools.json
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/networking_ipv6_ranges.json
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/networking_ipv6_ranges_2600:3c01::.json
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/networking_vlans.json
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/nodebalancers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/nodebalancers_123456_configs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/nodebalancers_123456_configs_65432_nodes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/object-storage_buckets.json
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/object-storage_buckets_us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/object-storage_buckets_us-east-1_example-bucket.json
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/object-storage_buckets_us-east-1_example-bucket_object-acl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/object-storage_buckets_us-east-1_example-bucket_object-list.json
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/object-storage_buckets_us-east-1_example-bucket_object-url.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/object-storage_buckets_us-east-1_example-bucket_ssl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/object-storage_clusters.json
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/object-storage_keys.json
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/object-storage_transfer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/profile_device_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/profile_devices.json
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/profile_logins.json
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/profile_logins_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/profile_preferences.json
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/profile_security-questions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/profile_sshkeys.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/regions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/support_tickets_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/tags_nothing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/tags_something.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures/volumes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42521 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/linode_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/login_client_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 17:35:25.627433 linode_api4-5.4.0/test/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/account_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20034 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/domain_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/firewall_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/linode_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/lke_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/longview_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/networking_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/nodebalancers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/object_storage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/profile_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/region_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/support_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/tag_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/objects/volume_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/paginated_list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-01 17:34:52.000000 linode_api4-5.4.0/test/util_test.py
```

### Comparing `linode_api4-5.3.0/LICENSE` & `linode_api4-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linode_api4-5.3.0/PKG-INFO` & `linode_api4-5.4.0/linode_api4.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
-Name: linode_api4
-Version: 5.3.0
+Name: linode-api4
+Version: 5.4.0
 Summary: The official python SDK for Linode API v4
 Home-page: https://github.com/linode/linode_api4-python
 Author: Linode
 Author-email: developers@linode.com
 License: BSD 3-Clause License
 Keywords: linode cloud hosting infrastructure
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE
 
 linode_api4
 ===========
 
 The official python library for the `Linode API v4`_ in python.
 
 .. _Linode API v4: https://developers.linode.com/api/v4/
 
-.. image:: https://travis-ci.com/linode/linode_api4-python.svg?branch=master
-    :target: https://travis-ci.com/linode/linode_api4-python
+.. image:: https://img.shields.io/github/actions/workflow/status/linode/linode_api4-python/main.yml?label=tests
+    :target: https://img.shields.io/github/actions/workflow/status/linode/linode_api4-python/main.yml?label=tests
 
 .. image:: https://badge.fury.io/py/linode-api4.svg
    :target: https://badge.fury.io/py/linode-api4
 
 .. image:: https://readthedocs.org/projects/linode-api4/badge/?version=latest
    :target: https://linode-api4.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
@@ -48,21 +50,70 @@
 
 To build and install this package:
 
 - Clone this repository
 - ``./setup.py install``
 
 Usage
------
+=====
+
+Quick Start
+-----------
+
+In order to authenticate with the Linode API, you will first need to create a
+`Linode Personal Access Token`_ with your desired account permissions.
+
+The following code sample can help you quickly get started using this package.
+
+.. code-block:: python
+
+    from linode_api4 import LinodeClient, Instance
+
+    # Create a Linode API client
+    client = LinodeClient("MY_PERSONAL_ACCESS_TOKEN")
+
+    # Create a new Linode
+    new_linode, root_pass = client.linode.instance_create(
+        ltype="g6-nanode-1",
+        region="us-southeast",
+        image="linode/ubuntu22.04",
+        label="my-ubuntu-linode"
+    )
+
+    # Print info about the Linode
+    print("Linode IP:", new_linode.ipv4[0])
+    print("Linode Root Password:", root_pass)
+
+    # List all Linodes on the account
+    my_linodes = client.linode.instances()
+
+    # Print the Label of every Linode on the account
+    print("All Instances:")
+    for instance in my_linodes:
+        print(instance.label)
 
-Check out the `Getting Started guide`_ to start using this library, or read
-`the docs`_ for extensive documentation.
+    # List Linodes in the us-southeast region
+    specific_linodes = client.linode.instances(
+        Instance.region == "us-southeast"
+    )
 
-.. _Getting Started guide: http://linode_api4.readthedocs.io/en/latest/guides/getting_started.html
-.. _the docs: http://linode_api4.readthedocs.io/en/latest/index.html
+    # Print the label of each Linode in us-southeast
+    print("Instances in us-southeast:")
+    for instance in specific_linodes:
+        print(instance.label)
+
+    # Delete the new instance
+    new_linode.delete()
+
+Check out the `Getting Started guide`_ for more details on getting started
+with this library, or read `the docs`_ for more extensive documentation.
+
+.. _Linode Personal Access Token: https://www.linode.com/docs/products/tools/api/guides/manage-api-tokens/
+.. _Getting Started guide: https://linode-api4.readthedocs.io/en/latest/guides/getting_started.html
+.. _the docs: https://linode-api4.readthedocs.io/en/latest/index.html
 
 Examples
 --------
 
 See the `Install on a Linode`_ example project for a simple use case demonstrating
 many of the features of this library.
 
@@ -107,21 +158,33 @@
 .. _tox: http://tox.readthedocs.io
 
 Documentation
 -------------
 
 This library is documented with Sphinx_.  Docs live in the ``docs`` directory.
 The easiest way to build the docs is to run ``sphinx-autobuild`` in that
-folder.
+folder::
+
+    sphinx-autobuild docs docs/build
+
+After running this command, ``sphinx-autobuild`` will host a local web server
+with the rendered documentation.
 
 Classes and functions inside the library should be annotated with sphinx-compliant
 docstrings which will be used to automatically generate documentation for the
 library.  When contributing, be sure to update documentation or include new
 docstrings where applicable to keep the library's documentation up to date
 and useful.
 
 **Missing or inaccurate documentation is a bug**.  If you notice that the
 documentation for this library is out of date or unclear, please
 `open an issue`_ to make us aware of the problem.
 
 .. _Sphinx: http://www.sphinx-doc.org/en/master/index.html
 .. _open an issue: https://github.com/linode/linode_api4-python/issues/new
+
+Contributing
+------------
+
+Please follow the `Contributing Guidelines`_ when making a contribution.
+
+.. _Contributing Guidelines: https://github.com/linode/linode_api4-python/blob/master/CONTRIBUTING.md
```

### Comparing `linode_api4-5.3.0/linode_api4/common.py` & `linode_api4-5.4.0/linode_api4/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import os
 
-
-SSH_KEY_TYPES = ("ssh-dss", "ssh-rsa", "ssh-ed25519", "ecdsa-sha2-nistp256",
-                 "ecdsa-sha2-nistp384", "ecdsa-sha2-nistp521")
+SSH_KEY_TYPES = (
+    "ssh-dss",
+    "ssh-rsa",
+    "ssh-ed25519",
+    "ecdsa-sha2-nistp256",
+    "ecdsa-sha2-nistp384",
+    "ecdsa-sha2-nistp521",
+)
 
 
 def load_and_validate_keys(authorized_keys):
     """
     Loads authorized_keys as taken by :any:`instance_create`,
     :any:`disk_create` or :any:`rebuild`, and loads in any keys from any files
     provided.
@@ -22,22 +27,33 @@
 
     if not isinstance(authorized_keys, list):
         authorized_keys = [authorized_keys]
 
     ret = []
 
     for k in authorized_keys:
-        accepted_types = ('ssh-dss', 'ssh-rsa', 'ecdsa-sha2-nistp', 'ssh-ed25519')
-        if any([ t for t in accepted_types if k.startswith(t) ]): # pylint: disable=use-a-generator
+        accepted_types = (
+            "ssh-dss",
+            "ssh-rsa",
+            "ecdsa-sha2-nistp",
+            "ssh-ed25519",
+        )
+        if any(
+            [t for t in accepted_types if k.startswith(t)]
+        ):  # pylint: disable=use-a-generator
             # this looks like a key, cool
             ret.append(k)
         else:
             # it doesn't appear to be a key.. is it a path to the key?
             k = os.path.expanduser(k)
             if os.path.isfile(k):
                 with open(k) as f:
                     ret.append(f.read().rstrip())
             else:
-                raise ValueError("authorized_keys must either be paths "
-                                 "to the key files or a list of raw "
-                                 "public key of one of these types: {}".format(accepted_types))
+                raise ValueError(
+                    "authorized_keys must either be paths "
+                    "to the key files or a list of raw "
+                    "public key of one of these types: {}".format(
+                        accepted_types
+                    )
+                )
     return ret
```

### Comparing `linode_api4-5.3.0/linode_api4/errors.py` & `linode_api4-5.4.0/linode_api4/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 
 class ApiError(RuntimeError):
     """
     An API Error is any error returned from the API.  These
     typically have a status code in the 400s or 500s.  Most
     often, this will be caused by invalid input to the API.
     """
+
     def __init__(self, message, status=400, json=None):
         super().__init__(message)
         self.status = status
         self.json = json
         self.errors = []
-        if json and 'errors' in json and isinstance(json['errors'], list):
-            self.errors = [ e['reason'] for e in json['errors'] ]
+        if json and "errors" in json and isinstance(json["errors"], list):
+            self.errors = [e["reason"] for e in json["errors"]]
+
 
 class UnexpectedResponseError(RuntimeError):
     """
     An Unexpected Response Error occurs when the API returns
     something that this library is unable to parse, usually
     because it expected something specific and didn't get it.
     These typically indicate an oversight in developing this
     library, and should be fixed with changes to this codebase.
     """
+
     def __init__(self, message, status=200, json=None):
         super().__init__(message)
         self.status = status
         self.json = json
```

### Comparing `linode_api4-5.3.0/linode_api4/login_client.py` & `linode_api4-5.4.0/linode_api4/login_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+import re
 from datetime import datetime, timedelta
 from enum import Enum
 
 import requests
 
 from linode_api4.errors import ApiError
 
 try:
-    from urllib.parse import urlparse
-    from urllib.parse import urlencode
-    from urllib.parse import urlunparse
+    from urllib.parse import urlencode, urlparse, urlunparse
 except ImportError:
-    from urlparse import urlparse
     from urllib import urlencode
-    from urlparse import urlunparse
 
-class AllWrapper():
+    from urlparse import urlparse, urlunparse
+
+
+class AllWrapper:
     def __repr__(self):
-        return '*'
+        return "*"
+
 
 class OAuthScopes:
     """
     Represents the OAuth Scopes available to an application.  In general, an
     application should request no more scopes than it requires.  This class
     should be treated like a Enum, and used as follows::
 
@@ -40,278 +41,295 @@
     #: If necessary, an application may request all scopes by using OAuthScopes.all
     all = AllWrapper()
 
     class Linodes(Enum):
         """
         Access to Linodes
         """
+
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "linodes:*"
             return "linodes:{}".format(self.name)
 
     class Domains(Enum):
         """
         Access to Domains
         """
+
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "domains:*"
             return "domains:{}".format(self.name)
 
     class StackScripts(Enum):
         """
         Access to private StackScripts
         """
+
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "stackscripts:*"
             return "stackscripts:{}".format(self.name)
 
     class Users(Enum):
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "users:*"
             return "users:{}".format(self.name)
 
     class NodeBalancers(Enum):
         """
         Access to NodeBalancers
         """
+
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "nodebalancers:*"
             return "nodebalancers:{}".format(self.name)
 
     class Tokens(Enum):
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "tokens:*"
             return "tokens:{}".format(self.name)
 
     class IPs(Enum):
         """
         Access to IPs and networking managements
         """
+
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "ips:*"
             return "ips:{}".format(self.name)
 
     class Firewalls(Enum):
         """
         Access to Firewalls
         """
+
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "firewall:*"
             return "firewall:{}".format(self.name)
 
     class Tickets(Enum):
         """
         Access to view, open, and respond to Support Tickets
         """
+
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "tickets:*"
             return "tickets:{}".format(self.name)
 
     class Clients(Enum):
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "clients:*"
             return "clients:{}".format(self.name)
 
     class Account(Enum):
         """
         Access to the user's account, including billing information, tokens
         management, user management, etc.
         """
+
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "account:*"
             return "account:{}".format(self.name)
 
     class Events(Enum):
         """
         Access to a user's Events
         """
+
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "events:*"
             return "events:{}".format(self.name)
 
     class Volumes(Enum):
         """
         Access to Block Storage Volumes
         """
+
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "volumes:*"
             return "volumes:{}".format(self.name)
 
     class LKE(Enum):
         """
         Access to LKE Endpoint
         """
+
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "lke:*"
             return "lke:{}".format(self.name)
 
     class ObjectStorage(Enum):
         """
         Access to Object Storage
         """
+
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "object_storage:*"
             return "object_storage:{}".format(self.name)
 
     class Longview(Enum):
         """
         Access to Longview
         """
+
         read_only = 0
         read_write = 1
         all = 2
 
         def __repr__(self):
-            if(self.name == 'all'):
+            if self.name == "all":
                 return "longview:*"
             return "longview:{}".format(self.name)
 
     _scope_families = {
-        'linodes': Linodes,
-        'domains': Domains,
-        'stackscripts': StackScripts,
-        'users': Users,
-        'tokens': Tokens,
-        'ips': IPs,
-        'firewall': Firewalls,
-        'tickets': Tickets,
-        'clients': Clients,
-        'account': Account,
-        'events': Events,
-        'volumes': Volumes,
-        'lke': LKE,
-        'object_storage': ObjectStorage,
-        'nodebalancers': NodeBalancers,
-        'longview': Longview,
+        "linodes": Linodes,
+        "domains": Domains,
+        "stackscripts": StackScripts,
+        "users": Users,
+        "tokens": Tokens,
+        "ips": IPs,
+        "firewall": Firewalls,
+        "tickets": Tickets,
+        "clients": Clients,
+        "account": Account,
+        "events": Events,
+        "volumes": Volumes,
+        "lke": LKE,
+        "object_storage": ObjectStorage,
+        "nodebalancers": NodeBalancers,
+        "longview": Longview,
     }
 
     @staticmethod
     def parse(scopes):
         ret = []
 
         # special all-scope case
-        if scopes == '*':
-            return [ getattr(OAuthScopes._scope_families[s], 'all')
-                    for s in OAuthScopes._scope_families ] # pylint: disable=consider-using-dict-items
+        if scopes == "*":
+            return [
+                getattr(scope, "all")
+                for scope in OAuthScopes._scope_families.values()
+            ]
 
-        for scope in scopes.split(','):
+        for scope in re.split("[, ]", scopes):
             resource = access = None
-            if ':' in scope:
-                resource, access = scope.split(':')
+            if ":" in scope:
+                resource, access = scope.split(":")
             else:
                 resource = scope
-                access = '*'
+                access = "*"
 
             parsed_scope = OAuthScopes._get_parsed_scope(resource, access)
             if parsed_scope:
                 ret.append(parsed_scope)
 
         return ret
 
     @staticmethod
     def _get_parsed_scope(resource, access):
         resource = resource.lower()
         access = access.lower()
         if resource in OAuthScopes._scope_families:
-            if access == '*':
-                access = 'delete'
+            if access == "*":
+                access = "all"
             if hasattr(OAuthScopes._scope_families[resource], access):
                 return getattr(OAuthScopes._scope_families[resource], access)
 
         return None
 
     @staticmethod
     def serialize(scopes):
-        ret = ''
+        ret = ""
         if not type(scopes) is list:
-            scopes = [ scopes ]
+            scopes = [scopes]
         for scope in scopes:
             ret += "{},".format(repr(scope))
         if ret:
             ret = ret[:-1]
         return ret
 
+
 class LinodeLoginClient:
-    def __init__(self, client_id, client_secret,
-                 base_url="https://login.linode.com"):
+    def __init__(
+        self, client_id, client_secret, base_url="https://login.linode.com"
+    ):
         """
         Create a new LinodeLoginClient.  These clients do not make any requests
         on creation, and can safely be created and thrown away as needed.
 
         For complete usage information, see the :doc:`OAuth guide<../guides/oauth>`.
 
         :param client_id: The OAuth Client ID for this client.
@@ -352,15 +370,15 @@
         :returns: The uri to send users to for this login attempt.
         :rtype: str
         """
         url = self.base_url + "/oauth/authorize"
         split = list(urlparse(url))
         params = {
             "client_id": self.client_id,
-            "response_type": "code", # needed for all logins
+            "response_type": "code",  # needed for all logins
         }
         if scopes:
             params["scopes"] = OAuthScopes.serialize(scopes)
         if redirect_uri:
             params["redirect_uri"] = redirect_uri
         split[4] = urlencode(params)
         return urlunparse(split)
@@ -394,27 +412,34 @@
         :returns: The new OAuth token, and a list of scopes the token has, when
                   the token expires, and a refresh token that can generate a new
                   valid token when this one is expired.
         :rtype: tuple(str, list)
 
         :raise ApiError: If the OAuth exchange fails.
         """
-        r = requests.post(self._login_uri("/oauth/token"), data={
+        r = requests.post(
+            self._login_uri("/oauth/token"),
+            data={
                 "code": code,
                 "client_id": self.client_id,
-                "client_secret": self.client_secret
-            })
+                "client_secret": self.client_secret,
+            },
+        )
 
         if r.status_code != 200:
-            raise ApiError("OAuth token exchange failed", status=r.status_code, json=r.json())
+            raise ApiError(
+                "OAuth token exchange failed",
+                status=r.status_code,
+                json=r.json(),
+            )
 
         token = r.json()["access_token"]
         scopes = OAuthScopes.parse(r.json()["scopes"])
-        expiry = datetime.now() + timedelta(seconds=r.json()['expires_in'])
-        refresh_token = r.json()['refresh_token']
+        expiry = datetime.now() + timedelta(seconds=r.json()["expires_in"])
+        refresh_token = r.json()["refresh_token"]
 
         return token, scopes, expiry, refresh_token
 
     def refresh_oauth_token(self, refresh_token):
         """
         Some tokens are generated with refresh tokens (namely tokens generated
         through an OAuth Exchange).  These tokens may be renewed, or "refreshed",
@@ -430,28 +455,31 @@
         :returns: The new OAuth token, and a list of scopes the token has, when
                   the token expires, and a refresh token that can generate a new
                   valid token when this one is expired.
         :rtype: tuple(str, list)
 
         :raise ApiError: If the refresh fails..
         """
-        r = requests.post(self._login_uri("/oauth/token"), data={
-            "grant_type": "refresh_token",
-            "client_id": self.client_id,
-            "client_secret": self.client_secret,
-            "refresh_token": refresh_token,
-        })
+        r = requests.post(
+            self._login_uri("/oauth/token"),
+            data={
+                "grant_type": "refresh_token",
+                "client_id": self.client_id,
+                "client_secret": self.client_secret,
+                "refresh_token": refresh_token,
+            },
+        )
 
         if r.status_code != 200:
             raise ApiError("Refresh failed", r)
 
         token = r.json()["access_token"]
         scopes = OAuthScopes.parse(r.json()["scopes"])
-        expiry = datetime.now() + timedelta(seconds=r.json()['expires_in'])
-        refresh_token = r.json()['refresh_token']
+        expiry = datetime.now() + timedelta(seconds=r.json()["expires_in"])
+        refresh_token = r.json()["refresh_token"]
 
         return token, scopes, expiry, refresh_token
 
     def expire_token(self, token):
         """
         Given a token, makes a request to the authentication server to expire
         it immediately.  This is considered a responsible way to log out a
@@ -462,17 +490,19 @@
         :type token: str
 
         :returns: If the expiration attempt succeeded.
         :rtype: bool
 
         :raises ApiError: If the expiration attempt failed.
         """
-        r = requests.post(self._login_uri("/oauth/token/expire"),
+        r = requests.post(
+            self._login_uri("/oauth/token/expire"),
             data={
                 "client_id": self.client_id,
                 "client_secret": self.client_secret,
                 "token": token,
-            })
+            },
+        )
 
         if r.status_code != 200:
             raise ApiError("Failed to expire token!", r)
         return True
```

### Comparing `linode_api4-5.3.0/linode_api4/objects/base.py` & `linode_api4-5.4.0/linode_api4/objects/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,203 +1,287 @@
 import time
 from datetime import datetime, timedelta
 
 from .filtering import FilterableMetaclass
 
-
 DATE_FORMAT = "%Y-%m-%dT%H:%M:%S"
 
 
 # The interval to reload volatile properties
 volatile_refresh_timeout = timedelta(seconds=15)
 
+
+class ExplicitNullValue:
+    """
+    An explicitly null value to set a property to.
+    Instances of `NullValue` differ from None as they will be explicitly
+    included in the resource PUT requests.
+    """
+
+
 class Property:
-    def __init__(self, mutable=False, identifier=False, volatile=False, relationship=None,
-            derived_class=None, is_datetime=False, filterable=False, id_relationship=False,
-            slug_relationship=False):
+    def __init__(
+        self,
+        mutable=False,
+        identifier=False,
+        volatile=False,
+        relationship=None,
+        derived_class=None,
+        is_datetime=False,
+        id_relationship=False,
+        slug_relationship=False,
+        nullable=False,
+    ):
         """
         A Property is an attribute returned from the API, and defines metadata
         about that value.  These are expected to be used as the values of a
         class-level dict named 'properties' in subclasses of Base.
 
         mutable - This Property should be sent in a call to save()
         identifier - This Property identifies the object in the API
         volatile - Re-query for this Property if the local value is older than the
             volatile refresh timeout
         relationship - The API Object this Property represents
         derived_class - The sub-collection type this Property represents
         is_datetime - True if this Property should be parsed as a datetime.datetime
-        filterable - True if the API allows filtering on this property
         id_relationship - This Property should create a relationship with this key as the ID
             (This should be used on fields ending with '_id' only)
         slug_relationship - This property is a slug related for a given type.
+        nullable - This property can be explicitly null on PUT requests.
         """
         self.mutable = mutable
         self.identifier = identifier
         self.volatile = volatile
         self.relationship = relationship
         self.derived_class = derived_class
         self.is_datetime = is_datetime
-        self.filterable = filterable
         self.id_relationship = id_relationship
         self.slug_relationship = slug_relationship
 
+
 class MappedObject:
     """
     Converts a dict into values accessible with the dot notation.
 
     object = {
         "this": "that"
     }
 
     becomes
 
     object.this # "that"
     """
+
     def __init__(self, **vals):
         self._expand_vals(self.__dict__, **vals)
 
     def _expand_vals(self, target, **vals):
         for v in vals:
             if type(vals[v]) is dict:
                 vals[v] = MappedObject(**vals[v])
             elif type(vals[v]) is list:
                 # oh mama
-                vals[v] = [ MappedObject(**i) if type(i) is dict else i for i in vals[v] ]
+                vals[v] = [
+                    MappedObject(**i) if type(i) is dict else i for i in vals[v]
+                ]
         target.update(vals)
 
     def __repr__(self):
         return "Mapping containing {}".format(vars(self).keys())
-    
+
     @property
     def dict(self):
         return dict(self.__dict__)
 
+
 class Base(object, metaclass=FilterableMetaclass):
     """
     The Base class knows how to look up api properties of a model, and lazy-load them.
     """
+
     properties = {}
 
     def __init__(self, client, id, json={}):
-        self._set('_populated', False)
-        self._set('_last_updated', datetime.min)
-        self._set('_client', client)
+        self._set("_populated", False)
+        self._set("_last_updated", datetime.min)
+        self._set("_client", client)
+        self._set("_changed", False)
 
         #: self._raw_json is a copy of the json received from the API on population,
         #: and cannot be relied upon to be current.  Local changes to mutable fields
         #: that have not been saved will not be present, and volatile fields will not
         #: be updated on access.
-        self._set('_raw_json', None)
+        self._set("_raw_json", None)
 
         for prop in type(self).properties:
             self._set(prop, None)
 
-        self._set('id', id)
-        if hasattr(type(self), 'id_attribute'):
-            self._set(getattr(type(self), 'id_attribute'), id)
+        self._set("id", id)
+        if hasattr(type(self), "id_attribute"):
+            self._set(getattr(type(self), "id_attribute"), id)
 
         self._populate(json)
 
     def __getattribute__(self, name):
         """
         Handles lazy-loading/refreshing an object from the server, and
         getting related objects, as defined in this object's 'properties'
         """
         if name in type(self).properties.keys():
             # We are accessing a Property
             if type(self).properties[name].identifier:
-                pass # don't load identifiers from the server, we have those
-            elif (object.__getattribute__(self, name) is None and not self._populated \
-                    or type(self).properties[name].derived_class) \
-                    or (type(self).properties[name].volatile \
-                    and object.__getattribute__(self, '_last_updated')
-                    + volatile_refresh_timeout < datetime.now()):
+                pass  # don't load identifiers from the server, we have those
+            elif (
+                object.__getattribute__(self, name) is None
+                and not self._populated
+                or type(self).properties[name].derived_class
+            ) or (
+                type(self).properties[name].volatile
+                and object.__getattribute__(self, "_last_updated")
+                + volatile_refresh_timeout
+                < datetime.now()
+            ):
                 # needs to be loaded from the server
                 if type(self).properties[name].derived_class:
-                    #load derived object(s)
-                    self._set(name, type(self).properties[name].derived_class
-                            ._api_get_derived(self, getattr(self, '_client')))
+                    # load derived object(s)
+                    self._set(
+                        name,
+                        type(self)
+                        .properties[name]
+                        .derived_class._api_get_derived(
+                            self, getattr(self, "_client")
+                        ),
+                    )
                 else:
                     self._api_get()
         elif "{}_id".format(name) in type(self).properties.keys():
             # possible id-based relationship
-            related_type = type(self).properties['{}_id'.format(name)].id_relationship
+            related_type = (
+                type(self).properties["{}_id".format(name)].id_relationship
+            )
             if related_type:
                 # no id, no related object
                 if not getattr(self, "{}_id".format(name)):
                     return None
                 # it is a relationship
-                relcache_name = '_{}_relcache'.format(name)
+                relcache_name = "_{}_relcache".format(name)
                 if not hasattr(self, relcache_name):
-                    self._set(relcache_name, related_type(self._client, getattr(self, '{}_id'.format(name))))
+                    self._set(
+                        relcache_name,
+                        related_type(
+                            self._client, getattr(self, "{}_id".format(name))
+                        ),
+                    )
                 return object.__getattribute__(self, relcache_name)
 
         return object.__getattribute__(self, name)
 
     def __repr__(self):
         """
         Returns a safe representation of this object without accessing the server
         """
         return "{}: {}".format(type(self).__name__, self.id)
 
     def __setattr__(self, name, value):
         """
         Enforces allowing editing of only Properties defined as mutable
         """
-        if name in type(self).properties.keys() and not type(self).properties[name].mutable:
-            raise AttributeError("'{}' is not a mutable field of '{}'"
-                .format(name, type(self).__name__))
+        if name in type(self).properties.keys():
+            if not type(self).properties[name].mutable:
+                raise AttributeError(
+                    "'{}' is not a mutable field of '{}'".format(
+                        name, type(self).__name__
+                    )
+                )
+
+            self._changed = True
+
         self._set(name, value)
 
-    def save(self):
+    def save(self, force=True) -> bool:
         """
-        Send this object's mutable values to the server in a PUT request
+        Send this object's mutable values to the server in a PUT request.
+
+        :param force: If true, this method will always send a PUT request regardless of
+                      whether the field has been explicitly updated. For optimization
+                      purposes, this field should be set to false for typical update
+                      operations. (Defaults to True)
+        :type force: bool
         """
-        resp = self._client.put(type(self).api_endpoint, model=self,
-            data=self._serialize())
+        if not force and not self._changed:
+            return False
 
-        if 'error' in resp:
+        resp = self._client.put(
+            type(self).api_endpoint, model=self, data=self._serialize()
+        )
+
+        if "error" in resp:
             return False
+
+        self._set("_changed", False)
+
         return True
 
     def delete(self):
         """
         Sends a DELETE request for this object
         """
         resp = self._client.delete(type(self).api_endpoint, model=self)
 
-        if 'error' in resp:
+        if "error" in resp:
             return False
         self.invalidate()
         return True
 
     def invalidate(self):
         """
         Invalidates all non-identifier Properties this object has locally,
         causing the next access to re-fetch them from the server
         """
-        for key in [k for k in type(self).properties.keys()
-                if not type(self).properties[k].identifier]:
+        for key in [
+            k
+            for k in type(self).properties.keys()
+            if not type(self).properties[k].identifier
+        ]:
             self._set(key, None)
 
-        self._set('_populated', False)
+        self._set("_populated", False)
 
     def _serialize(self):
         """
         A helper method to build a dict of all mutable Properties of
         this object
         """
-        result = { a: getattr(self, a) for a in type(self).properties
-            if type(self).properties[a].mutable }
 
+        result = {}
+
+        # Aggregate mutable values into a dict
+        for k, v in type(self).properties.items():
+            if not v.mutable:
+                continue
+
+            value = getattr(self, k)
+
+            if not value:
+                continue
+
+            # Let's allow explicit null values as both classes and instances
+            if (
+                isinstance(value, ExplicitNullValue)
+                or value == ExplicitNullValue
+            ):
+                value = None
+
+            result[k] = value
+
+        # Resolve the underlying IDs of results
         for k, v in result.items():
             if isinstance(v, Base):
                 result[k] = v.id
-            elif isinstance(v,MappedObject):
+            elif isinstance(v, MappedObject):
                 result[k] = v.dict
 
         return result
 
     def _api_get(self):
         """
         A helper method to GET this object from the server
@@ -211,98 +295,114 @@
         assigns values based on the properties dict and the attributes of
         its Properties.
         """
         if not json:
             return
 
         # hide the raw JSON away in case someone needs it
-        self._set('_raw_json', json)
+        self._set("_raw_json", json)
+        self._set("_updated", False)
 
         for key in json:
-            if key in (k for k in type(self).properties.keys()
-                    if not type(self).properties[k].identifier):
-                if type(self).properties[key].relationship \
-                    and not json[key] is None:
+            if key in (
+                k
+                for k in type(self).properties.keys()
+                if not type(self).properties[k].identifier
+            ):
+                if (
+                    type(self).properties[key].relationship
+                    and not json[key] is None
+                ):
                     if isinstance(json[key], list):
                         objs = []
                         for d in json[key]:
-                            if not 'id' in d:
+                            if not "id" in d:
                                 continue
                             new_class = type(self).properties[key].relationship
-                            obj = new_class.make_instance(d['id'],
-                                    getattr(self,'_client'))
+                            obj = new_class.make_instance(
+                                d["id"], getattr(self, "_client")
+                            )
                             if obj:
                                 obj._populate(d)
                             objs.append(obj)
                         self._set(key, objs)
                     else:
                         if isinstance(json[key], dict):
-                            related_id = json[key]['id']
+                            related_id = json[key]["id"]
                         else:
                             related_id = json[key]
                         new_class = type(self).properties[key].relationship
-                        obj = new_class.make_instance(related_id, getattr(self,'_client'))
+                        obj = new_class.make_instance(
+                            related_id, getattr(self, "_client")
+                        )
                         if obj and isinstance(json[key], dict):
                             obj._populate(json[key])
                         self._set(key, obj)
-                elif  type(self).properties[key].slug_relationship \
-                        and not json[key] is None:
+                elif (
+                    type(self).properties[key].slug_relationship
+                    and not json[key] is None
+                ):
                     # create an object of the expected type with the given slug
-                    self._set(key, type(self).properties[key].slug_relationship(self._client, json[key]))
+                    self._set(
+                        key,
+                        type(self)
+                        .properties[key]
+                        .slug_relationship(self._client, json[key]),
+                    )
                 elif type(json[key]) is dict:
                     self._set(key, MappedObject(**json[key]))
                 elif type(json[key]) is list:
                     # we're going to use MappedObject's behavior with lists to
                     # expand these, then grab the resulting value to set
                     mapping = MappedObject(_list=json[key])
-                    self._set(key, mapping._list) # pylint: disable=no-member
+                    self._set(key, mapping._list)  # pylint: disable=no-member
                 elif type(self).properties[key].is_datetime:
                     try:
                         t = time.strptime(json[key], DATE_FORMAT)
                         self._set(key, datetime.fromtimestamp(time.mktime(t)))
                     except:
                         # if this came back, there's probably an issue with the
                         # python library; a field was marked as a datetime but
                         # wasn't in the expected format.
                         self._set(key, json[key])
                 else:
                     self._set(key, json[key])
 
-        self._set('_populated', True)
-        self._set('_last_updated', datetime.now())
+        self._set("_populated", True)
+        self._set("_last_updated", datetime.now())
 
     def _set(self, name, value):
         """
         A helper method to set values of Properties without invoking
         the overloaded __setattr__
         """
         object.__setattr__(self, name, value)
 
     @classmethod
     def api_list(cls):
         """
         Returns a URL that will produce a list of JSON objects
         of this class' type
         """
-        return '/'.join(cls.api_endpoint.split('/')[:-1])
+        return "/".join(cls.api_endpoint.split("/")[:-1])
 
     @staticmethod
     def make(id, client, cls, parent_id=None, json=None):
         """
         Makes an api object based on an id and class.
 
         :param id: The id of the object to create
         :param client: The LinodeClient to give the new object
         :param cls: The class type to instantiate
         :param parent_id: The parent id for derived classes
         :param json: The JSON to use to populate the new class
 
         :returns: An instance of cls with the given id
         """
-        from .dbase import DerivedBase # pylint: disable-all
+        from .dbase import DerivedBase  # pylint: disable-all
 
         if issubclass(cls, DerivedBase):
             return cls(client, id, parent_id, json)
         else:
             return cls(client, id, json)
 
     @classmethod
```

### Comparing `linode_api4-5.3.0/linode_api4/objects/dbase.py` & `linode_api4-5.4.0/linode_api4/objects/dbase.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,20 +3,25 @@
 
 class DerivedBase(Base):
     """
     The DerivedBase class holds information about an object who belongs to another object
     (for example, a disk belongs to a linode).  These objects have their own endpoints,
     but they are below another object in the hierarchy (i.e. /linodes/lnde_123/disks/disk_123)
     """
-    derived_url_path = '' #override in child classes
-    parent_id_name = 'parent_id' #override in child classes
+
+    derived_url_path = ""  # override in child classes
+    parent_id_name = "parent_id"  # override in child classes
 
     def __init__(self, client, id, parent_id, json={}):
         Base.__init__(self, client, id, json=json)
 
         self._set(type(self).parent_id_name, parent_id)
 
     @classmethod
     def _api_get_derived(cls, parent, client):
-        base_url = "{}/{}".format(type(parent).api_endpoint, cls.derived_url_path)
-         
-        return client._get_objects(base_url, cls, model=parent, parent_id=parent.id)
+        base_url = "{}/{}".format(
+            type(parent).api_endpoint, cls.derived_url_path
+        )
+
+        return client._get_objects(
+            base_url, cls, model=parent, parent_id=parent.id
+        )
```

### Comparing `linode_api4-5.3.0/linode_api4/objects/filtering.py` & `linode_api4-5.4.0/linode_api4/objects/filtering.py`

 * *Files 5% similar despite different names*

```diff
@@ -243,223 +243,231 @@
 00000f20: 6565 6e20 636c 6173 7320 6174 7472 6962  een class attrib
 00000f30: 7574 6573 206f 6620 6669 6c74 6572 6162  utes of filterab
 00000f40: 6c65 2063 6c61 7373 6573 2028 7365 6520  le classes (see 
 00000f50: 6162 6f76 6529 2e20 2046 696c 7465 7273  above).  Filters
 00000f60: 2063 616e 0a20 2020 2062 6520 636f 6d62   can.    be comb
 00000f70: 696e 6564 2077 6974 6820 3a61 6e79 3a60  ined with :any:`
 00000f80: 616e 645f 6020 616e 6420 3a61 6e79 3a60  and_` and :any:`
-00000f90: 6f72 5f60 2e0a 2020 2020 2222 220a 2020  or_`..    """.  
-00000fa0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00000fb0: 656c 662c 2064 6374 293a 0a20 2020 2020  elf, dct):.     
-00000fc0: 2020 2073 656c 662e 6463 7420 3d20 6463     self.dct = dc
-00000fd0: 740a 0a20 2020 2064 6566 205f 5f6f 725f  t..    def __or_
-00000fe0: 5f28 7365 6c66 2c20 6f74 6865 7229 3a0a  _(self, other):.
-00000ff0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00001000: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
-00001010: 2046 696c 7465 7229 3a0a 2020 2020 2020   Filter):.      
-00001020: 2020 2020 2020 7261 6973 6520 5479 7065        raise Type
-00001030: 4572 726f 7228 2259 6f75 2063 616e 206f  Error("You can o
-00001040: 6e6c 7920 6f72 2046 696c 7465 7220 7479  nly or Filter ty
-00001050: 7065 7321 2229 0a20 2020 2020 2020 2069  pes!").        i
-00001060: 6620 272b 6f72 2720 696e 2073 656c 662e  f '+or' in self.
-00001070: 6463 743a 0a20 2020 2020 2020 2020 2020  dct:.           
-00001080: 2072 6574 7572 6e20 4669 6c74 6572 287b   return Filter({
-00001090: 2027 2b6f 7227 3a20 7365 6c66 2e64 6374   '+or': self.dct
-000010a0: 5b27 2b6f 7227 5d20 2b20 5b20 6f74 6865  ['+or'] + [ othe
-000010b0: 722e 6463 7420 5d20 7d29 0a20 2020 2020  r.dct ] }).     
-000010c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000010d0: 2020 2020 2072 6574 7572 6e20 4669 6c74       return Filt
-000010e0: 6572 287b 2027 2b6f 7227 3a20 5b73 656c  er({ '+or': [sel
-000010f0: 662e 6463 742c 206f 7468 6572 2e64 6374  f.dct, other.dct
-00001100: 5d20 7d29 0a0a 2020 2020 6465 6620 5f5f  ] })..    def __
-00001110: 616e 645f 5f28 7365 6c66 2c20 6f74 6865  and__(self, othe
-00001120: 7229 3a0a 2020 2020 2020 2020 6966 206e  r):.        if n
-00001130: 6f74 2069 7369 6e73 7461 6e63 6528 6f74  ot isinstance(ot
-00001140: 6865 722c 2046 696c 7465 7229 3a0a 2020  her, Filter):.  
-00001150: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00001160: 5479 7065 4572 726f 7228 2259 6f75 2063  TypeError("You c
-00001170: 616e 206f 6e6c 7920 616e 6420 4669 6c74  an only and Filt
-00001180: 6572 2074 7970 6573 2122 290a 2020 2020  er types!").    
-00001190: 2020 2020 6966 2027 2b61 6e64 2720 696e      if '+and' in
-000011a0: 2073 656c 662e 6463 743a 0a20 2020 2020   self.dct:.     
-000011b0: 2020 2020 2020 2072 6574 7572 6e20 4669         return Fi
-000011c0: 6c74 6572 287b 2027 2b61 6e64 273a 2073  lter({ '+and': s
-000011d0: 656c 662e 6463 745b 272b 616e 6427 5d20  elf.dct['+and'] 
-000011e0: 2b20 5b20 6f74 6865 722e 6463 7420 5d20  + [ other.dct ] 
-000011f0: 7d29 0a20 2020 2020 2020 2065 6c73 653a  }).        else:
-00001200: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00001210: 7572 6e20 4669 6c74 6572 287b 2027 2b61  urn Filter({ '+a
-00001220: 6e64 273a 205b 7365 6c66 2e64 6374 2c20  nd': [self.dct, 
-00001230: 6f74 6865 722e 6463 745d 207d 290a 0a20  other.dct] }).. 
-00001240: 2020 2064 6566 206f 7264 6572 5f62 7928     def order_by(
-00001250: 7365 6c66 2c20 6669 656c 642c 2064 6573  self, field, des
-00001260: 633d 4661 6c73 6529 3a0a 2020 2020 2020  c=False):.      
-00001270: 2020 2320 7765 2063 616e 2774 2069 6e63    # we can't inc
-00001280: 6c75 6465 2074 776f 206f 7264 6572 5f62  lude two order_b
-00001290: 7973 0a20 2020 2020 2020 2069 6620 272b  ys.        if '+
-000012a0: 6f72 6465 725f 6279 2720 696e 2073 656c  order_by' in sel
-000012b0: 662e 6463 743a 0a20 2020 2020 2020 2020  f.dct:.         
-000012c0: 2020 2072 6169 7365 2041 7373 6572 7469     raise Asserti
-000012d0: 6f6e 4572 726f 7228 2259 6f75 206d 6179  onError("You may
-000012e0: 206f 6e6c 7920 6f72 6465 7220 6279 206f   only order by o
-000012f0: 6e63 6521 2229 0a0a 2020 2020 2020 2020  nce!")..        
-00001300: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-00001310: 6528 6669 656c 642c 2046 696c 7465 7261  e(field, Filtera
-00001320: 626c 6541 7474 7269 6275 7465 293a 0a20  bleAttribute):. 
-00001330: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00001340: 2054 7970 6545 7272 6f72 2822 4361 6e20   TypeError("Can 
-00001350: 6f6e 6c79 206f 7264 6572 2062 7920 6669  only order by fi
-00001360: 6c74 6572 6162 6c65 2061 7474 7269 6275  lterable attribu
-00001370: 7465 7321 2229 0a0a 2020 2020 2020 2020  tes!")..        
-00001380: 7365 6c66 2e64 6374 5b27 2b6f 7264 6572  self.dct['+order
-00001390: 5f62 7927 5d20 3d20 6669 656c 642e 6e61  _by'] = field.na
-000013a0: 6d65 0a20 2020 2020 2020 2069 6620 6465  me.        if de
-000013b0: 7363 3a0a 2020 2020 2020 2020 2020 2020  sc:.            
-000013c0: 7365 6c66 2e64 6374 5b27 2b6f 7264 6572  self.dct['+order
-000013d0: 275d 203d 2027 6465 7363 270a 0a20 2020  '] = 'desc'..   
-000013e0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000013f0: 0a0a 2020 2020 6465 6620 6c69 6d69 7428  ..    def limit(
-00001400: 7365 6c66 2c20 6c69 6d69 7429 3a0a 2020  self, limit):.  
-00001410: 2020 2020 2020 2320 7765 2063 616e 2774        # we can't
-00001420: 206c 696d 6974 2074 7769 6365 0a20 2020   limit twice.   
-00001430: 2020 2020 2069 6620 272b 6c69 6d69 7427       if '+limit'
-00001440: 2069 6e20 7365 6c66 2e64 6374 3a0a 2020   in self.dct:.  
-00001450: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00001460: 4173 7365 7274 696f 6e45 7272 6f72 2822  AssertionError("
-00001470: 596f 7520 6d61 7920 6f6e 6c79 206c 696d  You may only lim
-00001480: 6974 206f 6e63 6521 2229 0a0a 2020 2020  it once!")..    
-00001490: 2020 2020 6966 206e 6f74 2074 7970 6528      if not type(
-000014a0: 6c69 6d69 7429 203d 3d20 696e 743a 0a20  limit) == int:. 
-000014b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000014c0: 2054 7970 6545 7272 6f72 2822 4c69 6d69   TypeError("Limi
-000014d0: 7420 6d75 7374 2062 6520 616e 2069 6e74  t must be an int
-000014e0: 2122 290a 0a20 2020 2020 2020 2073 656c  !")..        sel
-000014f0: 662e 6463 745b 272b 6c69 6d69 7427 5d20  f.dct['+limit'] 
-00001500: 3d20 6c69 6d69 740a 0a20 2020 2020 2020  = limit..       
-00001510: 2072 6574 7572 6e20 7365 6c66 0a0a 636c   return self..cl
-00001520: 6173 7320 4669 6c74 6572 6162 6c65 4174  ass FilterableAt
-00001530: 7472 6962 7574 653a 0a20 2020 2064 6566  tribute:.    def
-00001540: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00001550: 6e61 6d65 293a 0a20 2020 2020 2020 2073  name):.        s
-00001560: 656c 662e 6e61 6d65 203d 206e 616d 650a  elf.name = name.
-00001570: 0a20 2020 2064 6566 205f 5f65 715f 5f28  .    def __eq__(
-00001580: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
-00001590: 2020 2020 2020 7265 7475 726e 2046 696c        return Fil
-000015a0: 7465 7228 7b20 7365 6c66 2e6e 616d 653a  ter({ self.name:
-000015b0: 206f 7468 6572 207d 290a 0a20 2020 2064   other })..    d
-000015c0: 6566 205f 5f6e 655f 5f28 7365 6c66 2c20  ef __ne__(self, 
-000015d0: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
-000015e0: 7265 7475 726e 2046 696c 7465 7228 7b20  return Filter({ 
-000015f0: 7365 6c66 2e6e 616d 653a 207b 2022 2b6e  self.name: { "+n
-00001600: 6571 223a 206f 7468 6572 207d 207d 290a  eq": other } }).
-00001610: 0a20 2020 2023 2022 696e 2220 6576 616c  .    # "in" eval
-00001620: 7561 7465 7320 7468 6520 7265 7475 726e  uates the return
-00001630: 2076 616c 7565 202d 2068 6176 6520 746f   value - have to
-00001640: 2075 7365 200a 2020 2020 2320 7479 7065   use .    # type
-00001650: 2e63 6f6e 7461 696e 7320 696e 7374 6561  .contains instea
-00001660: 640a 2020 2020 6465 6620 636f 6e74 6169  d.    def contai
-00001670: 6e73 2873 656c 662c 206f 7468 6572 293a  ns(self, other):
-00001680: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001690: 4669 6c74 6572 287b 2073 656c 662e 6e61  Filter({ self.na
-000016a0: 6d65 3a20 7b20 222b 636f 6e74 6169 6e73  me: { "+contains
-000016b0: 223a 206f 7468 6572 207d 207d 290a 0a20  ": other } }).. 
-000016c0: 2020 2064 6566 205f 5f67 745f 5f28 7365     def __gt__(se
-000016d0: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
-000016e0: 2020 2020 7265 7475 726e 2046 696c 7465      return Filte
-000016f0: 7228 7b20 7365 6c66 2e6e 616d 653a 207b  r({ self.name: {
-00001700: 2022 2b67 7422 3a20 6f74 6865 7220 7d20   "+gt": other } 
-00001710: 7d29 0a0a 2020 2020 6465 6620 5f5f 6c74  })..    def __lt
-00001720: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
-00001730: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001740: 4669 6c74 6572 287b 2073 656c 662e 6e61  Filter({ self.na
-00001750: 6d65 3a20 7b20 222b 6c74 223a 206f 7468  me: { "+lt": oth
-00001760: 6572 207d 207d 290a 0a20 2020 2064 6566  er } })..    def
-00001770: 205f 5f67 655f 5f28 7365 6c66 2c20 6f74   __ge__(self, ot
-00001780: 6865 7229 3a0a 2020 2020 2020 2020 7265  her):.        re
-00001790: 7475 726e 2046 696c 7465 7228 7b20 7365  turn Filter({ se
-000017a0: 6c66 2e6e 616d 653a 207b 2022 2b67 7465  lf.name: { "+gte
-000017b0: 223a 206f 7468 6572 207d 207d 290a 0a20  ": other } }).. 
-000017c0: 2020 2064 6566 205f 5f6c 655f 5f28 7365     def __le__(se
-000017d0: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
-000017e0: 2020 2020 7265 7475 726e 2046 696c 7465      return Filte
-000017f0: 7228 7b20 7365 6c66 2e6e 616d 653a 207b  r({ self.name: {
-00001800: 2022 2b6c 7465 223a 206f 7468 6572 207d   "+lte": other }
-00001810: 207d 290a 0a63 6c61 7373 204e 6f6e 4669   })..class NonFi
-00001820: 6c74 6572 6162 6c65 4174 7472 6962 7574  lterableAttribut
-00001830: 653a 0a20 2020 2064 6566 205f 5f69 6e69  e:.    def __ini
-00001840: 745f 5f28 7365 6c66 2c20 636c 736e 616d  t__(self, clsnam
-00001850: 652c 2061 7472 6e61 6d65 293a 0a20 2020  e, atrname):.   
-00001860: 2020 2020 2073 656c 662e 636c 736e 616d       self.clsnam
-00001870: 6520 3d20 636c 736e 616d 650a 2020 2020  e = clsname.    
-00001880: 2020 2020 7365 6c66 2e61 7472 6e61 6d65      self.atrname
-00001890: 203d 2061 7472 6e61 6d65 0a0a 2020 2020   = atrname..    
-000018a0: 6465 6620 5f5f 6571 5f5f 2873 656c 662c  def __eq__(self,
-000018b0: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-000018c0: 2072 6169 7365 2041 7474 7269 6275 7465   raise Attribute
-000018d0: 4572 726f 7228 227b 7d20 6361 6e6e 6f74  Error("{} cannot
-000018e0: 2062 6520 6669 6c74 6572 6564 2062 7920   be filtered by 
-000018f0: 7b7d 222e 666f 726d 6174 2873 656c 662e  {}".format(self.
-00001900: 636c 736e 616d 652c 2073 656c 662e 6174  clsname, self.at
-00001910: 726e 616d 6529 290a 0a20 2020 2064 6566  rname))..    def
-00001920: 205f 5f6e 655f 5f28 7365 6c66 2c20 6f74   __ne__(self, ot
-00001930: 6865 7229 3a0a 2020 2020 2020 2020 7261  her):.        ra
-00001940: 6973 6520 4174 7472 6962 7574 6545 7272  ise AttributeErr
-00001950: 6f72 2822 7b7d 2063 616e 6e6f 7420 6265  or("{} cannot be
-00001960: 2066 696c 7465 7265 6420 6279 207b 7d22   filtered by {}"
-00001970: 2e66 6f72 6d61 7428 7365 6c66 2e63 6c73  .format(self.cls
-00001980: 6e61 6d65 2c20 7365 6c66 2e61 7472 6e61  name, self.atrna
-00001990: 6d65 2929 0a0a 2020 2020 6465 6620 636f  me))..    def co
-000019a0: 6e74 6169 6e73 2873 656c 662c 206f 7468  ntains(self, oth
-000019b0: 6572 293a 0a20 2020 2020 2020 2072 6169  er):.        rai
-000019c0: 7365 2041 7474 7269 6275 7465 4572 726f  se AttributeErro
-000019d0: 7228 227b 7d20 6361 6e6e 6f74 2062 6520  r("{} cannot be 
-000019e0: 6669 6c74 6572 6564 2062 7920 7b7d 222e  filtered by {}".
-000019f0: 666f 726d 6174 2873 656c 662e 636c 736e  format(self.clsn
-00001a00: 616d 652c 2073 656c 662e 6174 726e 616d  ame, self.atrnam
-00001a10: 6529 290a 0a20 2020 2064 6566 205f 5f67  e))..    def __g
-00001a20: 745f 5f28 7365 6c66 2c20 6f74 6865 7229  t__(self, other)
-00001a30: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00001a40: 4174 7472 6962 7574 6545 7272 6f72 2822  AttributeError("
-00001a50: 7b7d 2063 616e 6e6f 7420 6265 2066 696c  {} cannot be fil
-00001a60: 7465 7265 6420 6279 207b 7d22 2e66 6f72  tered by {}".for
-00001a70: 6d61 7428 7365 6c66 2e63 6c73 6e61 6d65  mat(self.clsname
-00001a80: 2c20 7365 6c66 2e61 7472 6e61 6d65 2929  , self.atrname))
-00001a90: 0a0a 2020 2020 6465 6620 5f5f 6c74 5f5f  ..    def __lt__
-00001aa0: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
-00001ab0: 2020 2020 2020 2072 6169 7365 2041 7474         raise Att
-00001ac0: 7269 6275 7465 4572 726f 7228 227b 7d20  ributeError("{} 
-00001ad0: 6361 6e6e 6f74 2062 6520 6669 6c74 6572  cannot be filter
-00001ae0: 6564 2062 7920 7b7d 222e 666f 726d 6174  ed by {}".format
-00001af0: 2873 656c 662e 636c 736e 616d 652c 2073  (self.clsname, s
-00001b00: 656c 662e 6174 726e 616d 6529 290a 0a20  elf.atrname)).. 
-00001b10: 2020 2064 6566 205f 5f67 655f 5f28 7365     def __ge__(se
-00001b20: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
-00001b30: 2020 2020 7261 6973 6520 4174 7472 6962      raise Attrib
-00001b40: 7574 6545 7272 6f72 2822 7b7d 2063 616e  uteError("{} can
-00001b50: 6e6f 7420 6265 2066 696c 7465 7265 6420  not be filtered 
-00001b60: 6279 207b 7d22 2e66 6f72 6d61 7428 7365  by {}".format(se
-00001b70: 6c66 2e63 6c73 6e61 6d65 2c20 7365 6c66  lf.clsname, self
-00001b80: 2e61 7472 6e61 6d65 2929 0a0a 2020 2020  .atrname))..    
-00001b90: 6465 6620 5f5f 6c65 5f5f 2873 656c 662c  def __le__(self,
-00001ba0: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-00001bb0: 2072 6169 7365 2041 7474 7269 6275 7465   raise Attribute
-00001bc0: 4572 726f 7228 227b 7d20 6361 6e6e 6f74  Error("{} cannot
-00001bd0: 2062 6520 6669 6c74 6572 6564 2062 7920   be filtered by 
-00001be0: 7b7d 222e 666f 726d 6174 2873 656c 662e  {}".format(self.
-00001bf0: 636c 736e 616d 652c 2073 656c 662e 6174  clsname, self.at
-00001c00: 726e 616d 6529 290a 0a63 6c61 7373 2046  rname))..class F
-00001c10: 696c 7465 7261 626c 654d 6574 6163 6c61  ilterableMetacla
-00001c20: 7373 2874 7970 6529 3a0a 2020 2020 6465  ss(type):.    de
-00001c30: 6620 5f5f 696e 6974 5f5f 2863 6c73 2c20  f __init__(cls, 
-00001c40: 6e61 6d65 2c20 6261 7365 732c 2064 6374  name, bases, dct
-00001c50: 293a 0a20 2020 2020 2020 2069 6620 6861  ):.        if ha
-00001c60: 7361 7474 7228 636c 732c 2027 7072 6f70  sattr(cls, 'prop
-00001c70: 6572 7469 6573 2729 3a0a 2020 2020 2020  erties'):.      
-00001c80: 2020 2020 2020 666f 7220 6b65 7920 696e        for key in
-00001c90: 2063 6c73 2e70 726f 7065 7274 6965 732e   cls.properties.
-00001ca0: 6b65 7973 2829 3a0a 2020 2020 2020 2020  keys():.        
-00001cb0: 2020 2020 2020 2020 7365 7461 7474 7228          setattr(
-00001cc0: 636c 732c 206b 6579 2c20 4669 6c74 6572  cls, key, Filter
-00001cd0: 6162 6c65 4174 7472 6962 7574 6528 6b65  ableAttribute(ke
-00001ce0: 7929 290a 0a20 2020 2020 2020 2073 7570  y))..        sup
-00001cf0: 6572 2829 2e5f 5f69 6e69 745f 5f28 6e61  er().__init__(na
-00001d00: 6d65 2c20 6261 7365 732c 2064 6374 290a  me, bases, dct).
+00000f90: 6f72 5f60 2e0a 2020 2020 2222 220a 0a20  or_`..    """.. 
+00000fa0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00000fb0: 7365 6c66 2c20 6463 7429 3a0a 2020 2020  self, dct):.    
+00000fc0: 2020 2020 7365 6c66 2e64 6374 203d 2064      self.dct = d
+00000fd0: 6374 0a0a 2020 2020 6465 6620 5f5f 6f72  ct..    def __or
+00000fe0: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
+00000ff0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00001000: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
+00001010: 2c20 4669 6c74 6572 293a 0a20 2020 2020  , Filter):.     
+00001020: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
+00001030: 6545 7272 6f72 2822 596f 7520 6361 6e20  eError("You can 
+00001040: 6f6e 6c79 206f 7220 4669 6c74 6572 2074  only or Filter t
+00001050: 7970 6573 2122 290a 2020 2020 2020 2020  ypes!").        
+00001060: 6966 2022 2b6f 7222 2069 6e20 7365 6c66  if "+or" in self
+00001070: 2e64 6374 3a0a 2020 2020 2020 2020 2020  .dct:.          
+00001080: 2020 7265 7475 726e 2046 696c 7465 7228    return Filter(
+00001090: 7b22 2b6f 7222 3a20 7365 6c66 2e64 6374  {"+or": self.dct
+000010a0: 5b22 2b6f 7222 5d20 2b20 5b6f 7468 6572  ["+or"] + [other
+000010b0: 2e64 6374 5d7d 290a 2020 2020 2020 2020  .dct]}).        
+000010c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000010d0: 2020 7265 7475 726e 2046 696c 7465 7228    return Filter(
+000010e0: 7b22 2b6f 7222 3a20 5b73 656c 662e 6463  {"+or": [self.dc
+000010f0: 742c 206f 7468 6572 2e64 6374 5d7d 290a  t, other.dct]}).
+00001100: 0a20 2020 2064 6566 205f 5f61 6e64 5f5f  .    def __and__
+00001110: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
+00001120: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+00001130: 696e 7374 616e 6365 286f 7468 6572 2c20  instance(other, 
+00001140: 4669 6c74 6572 293a 0a20 2020 2020 2020  Filter):.       
+00001150: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
+00001160: 7272 6f72 2822 596f 7520 6361 6e20 6f6e  rror("You can on
+00001170: 6c79 2061 6e64 2046 696c 7465 7220 7479  ly and Filter ty
+00001180: 7065 7321 2229 0a20 2020 2020 2020 2069  pes!").        i
+00001190: 6620 222b 616e 6422 2069 6e20 7365 6c66  f "+and" in self
+000011a0: 2e64 6374 3a0a 2020 2020 2020 2020 2020  .dct:.          
+000011b0: 2020 7265 7475 726e 2046 696c 7465 7228    return Filter(
+000011c0: 7b22 2b61 6e64 223a 2073 656c 662e 6463  {"+and": self.dc
+000011d0: 745b 222b 616e 6422 5d20 2b20 5b6f 7468  t["+and"] + [oth
+000011e0: 6572 2e64 6374 5d7d 290a 2020 2020 2020  er.dct]}).      
+000011f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00001200: 2020 2020 7265 7475 726e 2046 696c 7465      return Filte
+00001210: 7228 7b22 2b61 6e64 223a 205b 7365 6c66  r({"+and": [self
+00001220: 2e64 6374 2c20 6f74 6865 722e 6463 745d  .dct, other.dct]
+00001230: 7d29 0a0a 2020 2020 6465 6620 6f72 6465  })..    def orde
+00001240: 725f 6279 2873 656c 662c 2066 6965 6c64  r_by(self, field
+00001250: 2c20 6465 7363 3d46 616c 7365 293a 0a20  , desc=False):. 
+00001260: 2020 2020 2020 2023 2077 6520 6361 6e27         # we can'
+00001270: 7420 696e 636c 7564 6520 7477 6f20 6f72  t include two or
+00001280: 6465 725f 6279 730a 2020 2020 2020 2020  der_bys.        
+00001290: 6966 2022 2b6f 7264 6572 5f62 7922 2069  if "+order_by" i
+000012a0: 6e20 7365 6c66 2e64 6374 3a0a 2020 2020  n self.dct:.    
+000012b0: 2020 2020 2020 2020 7261 6973 6520 4173          raise As
+000012c0: 7365 7274 696f 6e45 7272 6f72 2822 596f  sertionError("Yo
+000012d0: 7520 6d61 7920 6f6e 6c79 206f 7264 6572  u may only order
+000012e0: 2062 7920 6f6e 6365 2122 290a 0a20 2020   by once!")..   
+000012f0: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
+00001300: 7374 616e 6365 2866 6965 6c64 2c20 4669  stance(field, Fi
+00001310: 6c74 6572 6162 6c65 4174 7472 6962 7574  lterableAttribut
+00001320: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00001330: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+00001340: 2243 616e 206f 6e6c 7920 6f72 6465 7220  "Can only order 
+00001350: 6279 2066 696c 7465 7261 626c 6520 6174  by filterable at
+00001360: 7472 6962 7574 6573 2122 290a 0a20 2020  tributes!")..   
+00001370: 2020 2020 2073 656c 662e 6463 745b 222b       self.dct["+
+00001380: 6f72 6465 725f 6279 225d 203d 2066 6965  order_by"] = fie
+00001390: 6c64 2e6e 616d 650a 2020 2020 2020 2020  ld.name.        
+000013a0: 6966 2064 6573 633a 0a20 2020 2020 2020  if desc:.       
+000013b0: 2020 2020 2073 656c 662e 6463 745b 222b       self.dct["+
+000013c0: 6f72 6465 7222 5d20 3d20 2264 6573 6322  order"] = "desc"
+000013d0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000013e0: 2073 656c 660a 0a20 2020 2064 6566 206c   self..    def l
+000013f0: 696d 6974 2873 656c 662c 206c 696d 6974  imit(self, limit
+00001400: 293a 0a20 2020 2020 2020 2023 2077 6520  ):.        # we 
+00001410: 6361 6e27 7420 6c69 6d69 7420 7477 6963  can't limit twic
+00001420: 650a 2020 2020 2020 2020 6966 2022 2b6c  e.        if "+l
+00001430: 696d 6974 2220 696e 2073 656c 662e 6463  imit" in self.dc
+00001440: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
+00001450: 6169 7365 2041 7373 6572 7469 6f6e 4572  aise AssertionEr
+00001460: 726f 7228 2259 6f75 206d 6179 206f 6e6c  ror("You may onl
+00001470: 7920 6c69 6d69 7420 6f6e 6365 2122 290a  y limit once!").
+00001480: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00001490: 7479 7065 286c 696d 6974 2920 3d3d 2069  type(limit) == i
+000014a0: 6e74 3a0a 2020 2020 2020 2020 2020 2020  nt:.            
+000014b0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
+000014c0: 224c 696d 6974 206d 7573 7420 6265 2061  "Limit must be a
+000014d0: 6e20 696e 7421 2229 0a0a 2020 2020 2020  n int!")..      
+000014e0: 2020 7365 6c66 2e64 6374 5b22 2b6c 696d    self.dct["+lim
+000014f0: 6974 225d 203d 206c 696d 6974 0a0a 2020  it"] = limit..  
+00001500: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00001510: 660a 0a0a 636c 6173 7320 4669 6c74 6572  f...class Filter
+00001520: 6162 6c65 4174 7472 6962 7574 653a 0a20  ableAttribute:. 
+00001530: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00001540: 7365 6c66 2c20 6e61 6d65 293a 0a20 2020  self, name):.   
+00001550: 2020 2020 2073 656c 662e 6e61 6d65 203d       self.name =
+00001560: 206e 616d 650a 0a20 2020 2064 6566 205f   name..    def _
+00001570: 5f65 715f 5f28 7365 6c66 2c20 6f74 6865  _eq__(self, othe
+00001580: 7229 3a0a 2020 2020 2020 2020 7265 7475  r):.        retu
+00001590: 726e 2046 696c 7465 7228 7b73 656c 662e  rn Filter({self.
+000015a0: 6e61 6d65 3a20 6f74 6865 727d 290a 0a20  name: other}).. 
+000015b0: 2020 2064 6566 205f 5f6e 655f 5f28 7365     def __ne__(se
+000015c0: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
+000015d0: 2020 2020 7265 7475 726e 2046 696c 7465      return Filte
+000015e0: 7228 7b73 656c 662e 6e61 6d65 3a20 7b22  r({self.name: {"
+000015f0: 2b6e 6571 223a 206f 7468 6572 7d7d 290a  +neq": other}}).
+00001600: 0a20 2020 2023 2022 696e 2220 6576 616c  .    # "in" eval
+00001610: 7561 7465 7320 7468 6520 7265 7475 726e  uates the return
+00001620: 2076 616c 7565 202d 2068 6176 6520 746f   value - have to
+00001630: 2075 7365 0a20 2020 2023 2074 7970 652e   use.    # type.
+00001640: 636f 6e74 6169 6e73 2069 6e73 7465 6164  contains instead
+00001650: 0a20 2020 2064 6566 2063 6f6e 7461 696e  .    def contain
+00001660: 7328 7365 6c66 2c20 6f74 6865 7229 3a0a  s(self, other):.
+00001670: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00001680: 696c 7465 7228 7b73 656c 662e 6e61 6d65  ilter({self.name
+00001690: 3a20 7b22 2b63 6f6e 7461 696e 7322 3a20  : {"+contains": 
+000016a0: 6f74 6865 727d 7d29 0a0a 2020 2020 6465  other}})..    de
+000016b0: 6620 5f5f 6774 5f5f 2873 656c 662c 206f  f __gt__(self, o
+000016c0: 7468 6572 293a 0a20 2020 2020 2020 2072  ther):.        r
+000016d0: 6574 7572 6e20 4669 6c74 6572 287b 7365  eturn Filter({se
+000016e0: 6c66 2e6e 616d 653a 207b 222b 6774 223a  lf.name: {"+gt":
+000016f0: 206f 7468 6572 7d7d 290a 0a20 2020 2064   other}})..    d
+00001700: 6566 205f 5f6c 745f 5f28 7365 6c66 2c20  ef __lt__(self, 
+00001710: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
+00001720: 7265 7475 726e 2046 696c 7465 7228 7b73  return Filter({s
+00001730: 656c 662e 6e61 6d65 3a20 7b22 2b6c 7422  elf.name: {"+lt"
+00001740: 3a20 6f74 6865 727d 7d29 0a0a 2020 2020  : other}})..    
+00001750: 6465 6620 5f5f 6765 5f5f 2873 656c 662c  def __ge__(self,
+00001760: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
+00001770: 2072 6574 7572 6e20 4669 6c74 6572 287b   return Filter({
+00001780: 7365 6c66 2e6e 616d 653a 207b 222b 6774  self.name: {"+gt
+00001790: 6522 3a20 6f74 6865 727d 7d29 0a0a 2020  e": other}})..  
+000017a0: 2020 6465 6620 5f5f 6c65 5f5f 2873 656c    def __le__(sel
+000017b0: 662c 206f 7468 6572 293a 0a20 2020 2020  f, other):.     
+000017c0: 2020 2072 6574 7572 6e20 4669 6c74 6572     return Filter
+000017d0: 287b 7365 6c66 2e6e 616d 653a 207b 222b  ({self.name: {"+
+000017e0: 6c74 6522 3a20 6f74 6865 727d 7d29 0a0a  lte": other}})..
+000017f0: 0a63 6c61 7373 204e 6f6e 4669 6c74 6572  .class NonFilter
+00001800: 6162 6c65 4174 7472 6962 7574 653a 0a20  ableAttribute:. 
+00001810: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00001820: 7365 6c66 2c20 636c 736e 616d 652c 2061  self, clsname, a
+00001830: 7472 6e61 6d65 293a 0a20 2020 2020 2020  trname):.       
+00001840: 2073 656c 662e 636c 736e 616d 6520 3d20   self.clsname = 
+00001850: 636c 736e 616d 650a 2020 2020 2020 2020  clsname.        
+00001860: 7365 6c66 2e61 7472 6e61 6d65 203d 2061  self.atrname = a
+00001870: 7472 6e61 6d65 0a0a 2020 2020 6465 6620  trname..    def 
+00001880: 5f5f 6571 5f5f 2873 656c 662c 206f 7468  __eq__(self, oth
+00001890: 6572 293a 0a20 2020 2020 2020 2072 6169  er):.        rai
+000018a0: 7365 2041 7474 7269 6275 7465 4572 726f  se AttributeErro
+000018b0: 7228 0a20 2020 2020 2020 2020 2020 2022  r(.            "
+000018c0: 7b7d 2063 616e 6e6f 7420 6265 2066 696c  {} cannot be fil
+000018d0: 7465 7265 6420 6279 207b 7d22 2e66 6f72  tered by {}".for
+000018e0: 6d61 7428 7365 6c66 2e63 6c73 6e61 6d65  mat(self.clsname
+000018f0: 2c20 7365 6c66 2e61 7472 6e61 6d65 290a  , self.atrname).
+00001900: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00001910: 6566 205f 5f6e 655f 5f28 7365 6c66 2c20  ef __ne__(self, 
+00001920: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
+00001930: 7261 6973 6520 4174 7472 6962 7574 6545  raise AttributeE
+00001940: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+00001950: 2020 227b 7d20 6361 6e6e 6f74 2062 6520    "{} cannot be 
+00001960: 6669 6c74 6572 6564 2062 7920 7b7d 222e  filtered by {}".
+00001970: 666f 726d 6174 2873 656c 662e 636c 736e  format(self.clsn
+00001980: 616d 652c 2073 656c 662e 6174 726e 616d  ame, self.atrnam
+00001990: 6529 0a20 2020 2020 2020 2029 0a0a 2020  e).        )..  
+000019a0: 2020 6465 6620 636f 6e74 6169 6e73 2873    def contains(s
+000019b0: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
+000019c0: 2020 2020 2072 6169 7365 2041 7474 7269       raise Attri
+000019d0: 6275 7465 4572 726f 7228 0a20 2020 2020  buteError(.     
+000019e0: 2020 2020 2020 2022 7b7d 2063 616e 6e6f         "{} canno
+000019f0: 7420 6265 2066 696c 7465 7265 6420 6279  t be filtered by
+00001a00: 207b 7d22 2e66 6f72 6d61 7428 7365 6c66   {}".format(self
+00001a10: 2e63 6c73 6e61 6d65 2c20 7365 6c66 2e61  .clsname, self.a
+00001a20: 7472 6e61 6d65 290a 2020 2020 2020 2020  trname).        
+00001a30: 290a 0a20 2020 2064 6566 205f 5f67 745f  )..    def __gt_
+00001a40: 5f28 7365 6c66 2c20 6f74 6865 7229 3a0a  _(self, other):.
+00001a50: 2020 2020 2020 2020 7261 6973 6520 4174          raise At
+00001a60: 7472 6962 7574 6545 7272 6f72 280a 2020  tributeError(.  
+00001a70: 2020 2020 2020 2020 2020 227b 7d20 6361            "{} ca
+00001a80: 6e6e 6f74 2062 6520 6669 6c74 6572 6564  nnot be filtered
+00001a90: 2062 7920 7b7d 222e 666f 726d 6174 2873   by {}".format(s
+00001aa0: 656c 662e 636c 736e 616d 652c 2073 656c  elf.clsname, sel
+00001ab0: 662e 6174 726e 616d 6529 0a20 2020 2020  f.atrname).     
+00001ac0: 2020 2029 0a0a 2020 2020 6465 6620 5f5f     )..    def __
+00001ad0: 6c74 5f5f 2873 656c 662c 206f 7468 6572  lt__(self, other
+00001ae0: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
+00001af0: 2041 7474 7269 6275 7465 4572 726f 7228   AttributeError(
+00001b00: 0a20 2020 2020 2020 2020 2020 2022 7b7d  .            "{}
+00001b10: 2063 616e 6e6f 7420 6265 2066 696c 7465   cannot be filte
+00001b20: 7265 6420 6279 207b 7d22 2e66 6f72 6d61  red by {}".forma
+00001b30: 7428 7365 6c66 2e63 6c73 6e61 6d65 2c20  t(self.clsname, 
+00001b40: 7365 6c66 2e61 7472 6e61 6d65 290a 2020  self.atrname).  
+00001b50: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00001b60: 205f 5f67 655f 5f28 7365 6c66 2c20 6f74   __ge__(self, ot
+00001b70: 6865 7229 3a0a 2020 2020 2020 2020 7261  her):.        ra
+00001b80: 6973 6520 4174 7472 6962 7574 6545 7272  ise AttributeErr
+00001b90: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+00001ba0: 227b 7d20 6361 6e6e 6f74 2062 6520 6669  "{} cannot be fi
+00001bb0: 6c74 6572 6564 2062 7920 7b7d 222e 666f  ltered by {}".fo
+00001bc0: 726d 6174 2873 656c 662e 636c 736e 616d  rmat(self.clsnam
+00001bd0: 652c 2073 656c 662e 6174 726e 616d 6529  e, self.atrname)
+00001be0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00001bf0: 6465 6620 5f5f 6c65 5f5f 2873 656c 662c  def __le__(self,
+00001c00: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
+00001c10: 2072 6169 7365 2041 7474 7269 6275 7465   raise Attribute
+00001c20: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+00001c30: 2020 2022 7b7d 2063 616e 6e6f 7420 6265     "{} cannot be
+00001c40: 2066 696c 7465 7265 6420 6279 207b 7d22   filtered by {}"
+00001c50: 2e66 6f72 6d61 7428 7365 6c66 2e63 6c73  .format(self.cls
+00001c60: 6e61 6d65 2c20 7365 6c66 2e61 7472 6e61  name, self.atrna
+00001c70: 6d65 290a 2020 2020 2020 2020 290a 0a0a  me).        )...
+00001c80: 636c 6173 7320 4669 6c74 6572 6162 6c65  class Filterable
+00001c90: 4d65 7461 636c 6173 7328 7479 7065 293a  Metaclass(type):
+00001ca0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00001cb0: 5f28 636c 732c 206e 616d 652c 2062 6173  _(cls, name, bas
+00001cc0: 6573 2c20 6463 7429 3a0a 2020 2020 2020  es, dct):.      
+00001cd0: 2020 6966 2068 6173 6174 7472 2863 6c73    if hasattr(cls
+00001ce0: 2c20 2270 726f 7065 7274 6965 7322 293a  , "properties"):
+00001cf0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00001d00: 206b 6579 2069 6e20 636c 732e 7072 6f70   key in cls.prop
+00001d10: 6572 7469 6573 2e6b 6579 7328 293a 0a20  erties.keys():. 
+00001d20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001d30: 6574 6174 7472 2863 6c73 2c20 6b65 792c  etattr(cls, key,
+00001d40: 2046 696c 7465 7261 626c 6541 7474 7269   FilterableAttri
+00001d50: 6275 7465 286b 6579 2929 0a0a 2020 2020  bute(key))..    
+00001d60: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+00001d70: 6974 5f5f 286e 616d 652c 2062 6173 6573  it__(name, bases
+00001d80: 2c20 6463 7429 0a                        , dct).
```

### Comparing `linode_api4-5.3.0/linode_api4/objects/image.py` & `linode_api4-5.4.0/linode_api4/objects/image.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from linode_api4.objects import Base, Property
 
 
 class Image(Base):
     """
     An Image is something a Linode Instance or Disk can be deployed from.
+
+    API Documentation: https://www.linode.com/docs/api/images/#image-view
     """
-    api_endpoint = '/images/{id}'
+
+    api_endpoint = "/images/{id}"
 
     properties = {
         "id": Property(identifier=True),
         "label": Property(mutable=True),
         "description": Property(mutable=True),
+        "eol": Property(is_datetime=True),
+        "expiry": Property(is_datetime=True),
         "status": Property(),
         "created": Property(is_datetime=True),
         "created_by": Property(),
+        "updated": Property(is_datetime=True),
         "type": Property(),
         "is_public": Property(),
         "vendor": Property(),
         "size": Property(),
-        "deprecated": Property()
+        "deprecated": Property(),
     }
```

### Comparing `linode_api4-5.3.0/linode_api4/objects/networking.py` & `linode_api4-5.4.0/linode_api4/objects/volume.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,137 +1,123 @@
 from linode_api4.errors import UnexpectedResponseError
-from linode_api4.objects import Base, DerivedBase, Property, Region
+from linode_api4.objects import Base, Instance, Property, Region
 
 
-class IPv6Pool(Base):
-    api_endpoint = '/networking/ipv6/pools/{}'
-    id_attribute = 'range'
-
-    properties = {
-        'range': Property(identifier=True),
-        'region': Property(slug_relationship=Region, filterable=True),
-    }
+class Volume(Base):
+    """
+    A single Block Storage Volume. Block Storage Volumes are persistent storage devices
+    that can be attached to a Compute Instance and used to store any type of data.
 
+    API Documentation: https://www.linode.com/docs/api/volumes/#volume-view
+    """
 
-class IPv6Range(Base):
-    api_endpoint = '/networking/ipv6/ranges/{}'
-    id_attribute = 'range'
+    api_endpoint = "/volumes/{id}"
 
     properties = {
-        'range': Property(identifier=True),
-        'region': Property(slug_relationship=Region, filterable=True),
+        "id": Property(identifier=True),
+        "created": Property(is_datetime=True),
+        "updated": Property(is_datetime=True),
+        "linode_id": Property(id_relationship=Instance),
+        "label": Property(mutable=True),
+        "size": Property(),
+        "status": Property(),
+        "region": Property(slug_relationship=Region),
+        "tags": Property(mutable=True),
+        "filesystem_path": Property(),
+        "hardware_type": Property(),
+        "linode_label": Property(),
     }
 
+    def attach(self, to_linode, config=None):
+        """
+        Attaches this Volume to the given Linode.
 
-class IPAddress(Base):
-    api_endpoint = '/networking/ips/{address}'
-    id_attribute = 'address'
+        API Documentation: https://www.linode.com/docs/api/volumes/#volume-attach
 
-    properties = {
-        "address": Property(identifier=True),
-        "gateway": Property(),
-        "subnet_mask": Property(),
-        "prefix": Property(),
-        "type": Property(),
-        "public": Property(),
-        "rdns": Property(mutable=True),
-        "linode_id": Property(),
-        "region": Property(slug_relationship=Region, filterable=True),
-    }
+        :param to_linode: The ID or object of the Linode to attach the volume to.
+        :type to_linode: Union[Instance, int]
 
-    @property
-    def linode(self):
-        from .linode import Instance # pylint: disable-all
-        if not hasattr(self, '_linode'):
-            self._set('_linode', Instance(self._client, self.linode_id))
-        return self._linode
-
-    def to(self, linode):
-        """
-        This is a helper method for ip-assign, and should not be used outside
-        of that context.  It's used to cleanly build an IP Assign request with
-        pretty python syntax.
+        :param config: The ID or object of the Linode Config to include this Volume in.
+                       Must belong to the Linode referenced by linode_id.
+                       If not given, the last booted Config will be chosen.
+        :type config: Union[Config, int]
         """
-        from .linode import Instance # pylint: disable-all
-        if not isinstance(linode, Instance):
-            raise ValueError("IP Address can only be assigned to a Linode!")
-        return { "address": self.address, "linode_id": linode.id }
+        result = self._client.post(
+            "{}/attach".format(Volume.api_endpoint),
+            model=self,
+            data={
+                "linode_id": to_linode.id
+                if issubclass(type(to_linode), Base)
+                else to_linode,
+                "config": None
+                if not config
+                else config.id
+                if issubclass(type(config), Base)
+                else config,
+            },
+        )
 
+        if not "id" in result:
+            raise UnexpectedResponseError(
+                "Unexpected response when attaching volume!", json=result
+            )
 
+        self._populate(result)
+        return True
 
-class VLAN(Base):
-    """
-    .. note:: At this time, the Linode API only supports listing VLANs.
-    .. note:: This endpoint is in beta. This will only function if base_url is set to `https://api.linode.com/v4beta`.
-    """
-    api_endpoint = '/networking/vlans/{}'
-    id_attribute = 'label'
-
-    properties = {
-        'label': Property(identifier=True),
-        'created': Property(is_datetime=True),
-        'linodes': Property(filterable=True),
-        'region': Property(slug_relationship=Region, filterable=True)
-    }
+    def detach(self):
+        """
+        Detaches this Volume if it is attached
 
+        API Documentation: https://www.linode.com/docs/api/volumes/#volume-detach
 
-class FirewallDevice(DerivedBase):
-    api_endpoint = '/networking/firewalls/{firewall_id}/devices/{id}'
-    derived_url_path = 'devices'
-    parent_id_name = 'firewall_id'
+        :returns: Returns true if operation was successful
+        :rtype: bool
+        """
+        self._client.post("{}/detach".format(Volume.api_endpoint), model=self)
 
-    properties = {
-        'created': Property(filterable=True, is_datetime=True),
-        'updated': Property(filterable=True, is_datetime=True),
-        'entity': Property(),
-        'id': Property(identifier=True)
-    }
+        return True
 
+    def resize(self, size):
+        """
+        Resizes this Volume
 
-class Firewall(Base):
-    """
-    .. note:: This endpoint is in beta. This will only function if base_url is set to `https://api.linode.com/v4beta`.
-    """
+        API Documentation: https://www.linode.com/docs/api/volumes/#volume-resize
 
-    api_endpoint = "/networking/firewalls/{id}"
+        :param size: The Volume’s size, in GiB.
+        :type size: int
 
-    properties = {
-        'id': Property(identifier=True),
-        'label': Property(mutable=True, filterable=True),
-        'tags': Property(mutable=True, filterable=True),
-        'status': Property(mutable=True),
-        'created': Property(filterable=True, is_datetime=True),
-        'updated': Property(filterable=True, is_datetime=True),
-        'devices': Property(derived_class=FirewallDevice),
-        'rules': Property(),
-    }
-    def update_rules(self, rules):
+        :returns: Returns true if operation was successful
+        :rtype: bool
         """
-        Sets the JSON rules for this Firewall
-        """
-        self._client.put('{}/rules'.format(self.api_endpoint), model=self, data=rules)
-        self.invalidate()
+        result = self._client.post(
+            "{}/resize".format(Volume.api_endpoint),
+            model=self,
+            data={"size": size},
+        )
 
-    def device_create(self, id, type='linode', **kwargs):
-        """
-        Creates and attaches a device to this Firewall
+        self._populate(result)
 
-        :param id: The ID of the entity to create a device for.
-        :type id: int
+        return True
 
-        :param type: The type of entity the device is being created for. (`linode`)
-        :type type: str
+    def clone(self, label):
         """
-        params = {
-            'id': id,
-            'type': type,
-        }
-        params.update(kwargs)
+        Clones this volume to a new volume in the same region with the given label
 
-        result = self._client.post("{}/devices".format(Firewall.api_endpoint), model=self, data=params)
-        self.invalidate()
+        API Documentation: https://www.linode.com/docs/api/volumes/#volume-clone
+
+        :param label: The label for the new volume.
+        :type label: str
+
+        :returns: The new volume object.
+        :rtype: Volume
+        """
+        result = self._client.post(
+            "{}/clone".format(Volume.api_endpoint),
+            model=self,
+            data={"label": label},
+        )
 
-        if not 'id' in result:
-            raise UnexpectedResponseError('Unexpected response creating device!', json=result)
+        if not "id" in result:
+            raise UnexpectedResponseError("Unexpected response cloning volume!")
 
-        c = FirewallDevice(self._client, result['id'], self.id, result)
-        return c
+        return Volume(self._client, result["id"], result)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `linode_api4-5.3.0/linode_api4/objects/nodebalancer.py` & `linode_api4-5.4.0/linode_api4/objects/nodebalancer.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,56 +2,72 @@
 
 from linode_api4.errors import UnexpectedResponseError
 from linode_api4.objects import Base, DerivedBase, Property, Region
 from linode_api4.objects.networking import IPAddress
 
 
 class NodeBalancerNode(DerivedBase):
-    api_endpoint = '/nodebalancers/{nodebalancer_id}/configs/{config_id}/nodes/{id}'
-    derived_url_path = 'nodes'
-    parent_id_name='config_id'
+    """
+    The information about a single Node, a backend for this NodeBalancer’s configured port.
+
+    API documentation: https://www.linode.com/docs/api/nodebalancers/#node-view
+    """
+
+    api_endpoint = (
+        "/nodebalancers/{nodebalancer_id}/configs/{config_id}/nodes/{id}"
+    )
+    derived_url_path = "nodes"
+    parent_id_name = "config_id"
 
     properties = {
-        'id': Property(identifier=True),
-        'config_id': Property(identifier=True),
-        'nodebalancer_id': Property(identifier=True),
+        "id": Property(identifier=True),
+        "config_id": Property(identifier=True),
+        "nodebalancer_id": Property(identifier=True),
         "label": Property(mutable=True),
         "address": Property(mutable=True),
         "weight": Property(mutable=True),
         "mode": Property(mutable=True),
         "status": Property(),
-        'tags': Property(mutable=True),
+        "tags": Property(mutable=True),
     }
 
     def __init__(self, client, id, parent_id, nodebalancer_id=None, json=None):
         """
         We need a special constructor here because this object's parent
         has a parent itself.
         """
         if not nodebalancer_id and not isinstance(parent_id, tuple):
-            raise ValueError('NodeBalancerNode must either be created with a nodebalancer_id or a tuple of '
-                    '(config_id, nodebalancer_id) for parent_id!')
+            raise ValueError(
+                "NodeBalancerNode must either be created with a nodebalancer_id or a tuple of "
+                "(config_id, nodebalancer_id) for parent_id!"
+            )
 
         if isinstance(parent_id, tuple):
             nodebalancer_id = parent_id[1]
             parent_id = parent_id[0]
 
         DerivedBase.__init__(self, client, id, parent_id, json=json)
 
-        self._set('nodebalancer_id', nodebalancer_id)
+        self._set("nodebalancer_id", nodebalancer_id)
 
 
 class NodeBalancerConfig(DerivedBase):
-    api_endpoint = '/nodebalancers/{nodebalancer_id}/configs/{id}'
-    derived_url_path = 'configs'
-    parent_id_name='nodebalancer_id'
+    """
+    The configuration information for a single port of this NodeBalancer.
+
+    API documentation: https://www.linode.com/docs/api/nodebalancers/#config-view
+    """
+
+    api_endpoint = "/nodebalancers/{nodebalancer_id}/configs/{id}"
+    derived_url_path = "configs"
+    parent_id_name = "nodebalancer_id"
 
     properties = {
-        'id': Property(identifier=True),
-        'nodebalancer_id': Property(identifier=True),
+        "id": Property(identifier=True),
+        "nodebalancer_id": Property(identifier=True),
         "port": Property(mutable=True),
         "protocol": Property(mutable=True),
         "algorithm": Property(mutable=True),
         "stickiness": Property(mutable=True),
         "check": Property(mutable=True),
         "check_interval": Property(mutable=True),
         "check_timeout": Property(mutable=True),
@@ -61,46 +77,88 @@
         "check_passive": Property(mutable=True),
         "ssl_cert": Property(mutable=True),
         "ssl_key": Property(mutable=True),
         "ssl_commonname": Property(),
         "ssl_fingerprint": Property(),
         "cipher_suite": Property(mutable=True),
         "nodes_status": Property(),
-        'proxy_protocol': Property(mutable=True),
+        "proxy_protocol": Property(mutable=True),
     }
 
     @property
     def nodes(self):
         """
         This is a special derived_class relationship because NodeBalancerNode is the
         only api object that requires two parent_ids
+
+        Returns a paginated list of NodeBalancer nodes associated with this Config.
+        These are the backends that will be sent traffic for this port.
+
+        API documentation: https://www.linode.com/docs/api/nodebalancers/#nodes-list
+
+        :returns: A paginated list of NodeBalancer nodes.
+        :rtype: PaginatedList of NodeBalancerNode
         """
-        if not hasattr(self, '_nodes'):
-            base_url = "{}/{}".format(NodeBalancerConfig.api_endpoint, NodeBalancerNode.derived_url_path)
-            result = self._client._get_objects(base_url, NodeBalancerNode, model=self, parent_id=(self.id, self.nodebalancer_id))
+        if not hasattr(self, "_nodes"):
+            base_url = "{}/{}".format(
+                NodeBalancerConfig.api_endpoint,
+                NodeBalancerNode.derived_url_path,
+            )
+            result = self._client._get_objects(
+                base_url,
+                NodeBalancerNode,
+                model=self,
+                parent_id=(self.id, self.nodebalancer_id),
+            )
 
-            self._set('_nodes', result)
+            self._set("_nodes", result)
 
         return self._nodes
 
     def node_create(self, label, address, **kwargs):
+        """
+        Creates a NodeBalancer Node, a backend that can accept traffic for this
+        NodeBalancer Config. Nodes are routed requests on the configured port based
+        on their status.
+
+        API documentation: https://www.linode.com/docs/api/nodebalancers/#node-create
+
+        :param address: The private IP Address where this backend can be reached.
+                        This must be a private IP address.
+        :type address: str
+
+        :param label: The label for this node. This is for display purposes only.
+                      Must have a length between 2 and 32 characters.
+        :type label: str
+
+        :returns: The node which is created successfully.
+        :rtype: NodeBalancerNode
+        """
         params = {
             "label": label,
             "address": address,
         }
         params.update(kwargs)
 
-        result = self._client.post("{}/nodes".format(NodeBalancerConfig.api_endpoint), model=self, data=params)
+        result = self._client.post(
+            "{}/nodes".format(NodeBalancerConfig.api_endpoint),
+            model=self,
+            data=params,
+        )
         self.invalidate()
 
-        if not 'id' in result:
-            raise UnexpectedResponseError('Unexpected response creating node!', json=result)
+        if not "id" in result:
+            raise UnexpectedResponseError(
+                "Unexpected response creating node!", json=result
+            )
 
         # this is three levels deep, so we need a special constructor
-        n = NodeBalancerNode(self._client, result['id'], self.id, self.nodebalancer_id, result)
+        n = NodeBalancerNode(
+            self._client, result["id"], self.id, self.nodebalancer_id, result
+        )
         return n
 
     def load_ssl_data(self, cert_file, key_file):
         """
         A convenience method that loads a cert and a key from files and sets them
         on this object.  This can make enabling ssl easier (instead of you needing
         to load the files yourself).
@@ -120,44 +178,64 @@
         # occur on a save()
         _ = self.ssl_fingerprint
 
         # we're disabling warnings here because these attributes are defined dynamically
         # through linode.objects.Base, and pylint isn't privy
         if os.path.isfile(os.path.expanduser(cert_file)):
             with open(os.path.expanduser(cert_file)) as f:
-                self.ssl_cert = f.read() # pylint: disable=attribute-defined-outside-init
+                self.ssl_cert = f.read()
 
         if os.path.isfile(os.path.expanduser(key_file)):
             with open(os.path.expanduser(key_file)) as f:
-                self.ssl_key = f.read() # pylint: disable=attribute-defined-outside-init
+                self.ssl_key = f.read()
 
 
 class NodeBalancer(Base):
-    api_endpoint = '/nodebalancers/{id}'
+    """
+    A single NodeBalancer you can access.
+
+    API documentation: https://www.linode.com/docs/api/nodebalancers/#nodebalancer-view
+    """
+
+    api_endpoint = "/nodebalancers/{id}"
     properties = {
-        'id': Property(identifier=True),
-        'label': Property(mutable=True),
-        'hostname': Property(),
-        'client_conn_throttle': Property(mutable=True),
-        'status': Property(),
-        'created': Property(is_datetime=True),
-        'updated': Property(is_datetime=True),
-        'ipv4': Property(relationship=IPAddress),
-        'ipv6': Property(),
-        'region': Property(slug_relationship=Region, filterable=True),
-        'configs': Property(derived_class=NodeBalancerConfig),
+        "id": Property(identifier=True),
+        "label": Property(mutable=True),
+        "hostname": Property(),
+        "client_conn_throttle": Property(mutable=True),
+        "status": Property(),
+        "created": Property(is_datetime=True),
+        "updated": Property(is_datetime=True),
+        "ipv4": Property(relationship=IPAddress),
+        "ipv6": Property(),
+        "region": Property(slug_relationship=Region),
+        "configs": Property(derived_class=NodeBalancerConfig),
     }
 
     # create derived objects
-    def config_create(self, label=None, **kwargs):
+    def config_create(self, **kwargs):
+        """
+        Creates a NodeBalancer Config, which allows the NodeBalancer to accept traffic
+        on a new port. You will need to add NodeBalancer Nodes to the new Config before
+        it can actually serve requests.
+
+        API documentation: https://www.linode.com/docs/api/nodebalancers/#config-create
+
+        :returns: The config that created successfully.
+        :rtype: NodeBalancerConfig
+        """
         params = kwargs
-        if label:
-            params['label'] = label
 
-        result = self._client.post("{}/configs".format(NodeBalancer.api_endpoint), model=self, data=params)
+        result = self._client.post(
+            "{}/configs".format(NodeBalancer.api_endpoint),
+            model=self,
+            data=params,
+        )
         self.invalidate()
 
-        if not 'id' in result:
-            raise UnexpectedResponseError('Unexpected response creating config!', json=result)
+        if not "id" in result:
+            raise UnexpectedResponseError(
+                "Unexpected response creating config!", json=result
+            )
 
-        c = NodeBalancerConfig(self._client, result['id'], self.id, result)
+        c = NodeBalancerConfig(self._client, result["id"], self.id, result)
         return c
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `linode_api4-5.3.0/linode_api4/objects/tag.py` & `linode_api4-5.4.0/linode_api4/objects/tag.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,54 @@
-import string
-import sys
-from datetime import datetime
-from enum import Enum
-from os import urandom
-from random import randint
-
 from linode_api4.errors import UnexpectedResponseError
+from linode_api4.objects import (
+    Base,
+    DerivedBase,
+    Domain,
+    Instance,
+    NodeBalancer,
+    Property,
+    Volume,
+)
 from linode_api4.paginated_list import PaginatedList
-from linode_api4.objects import (Base, DerivedBase, Property, Instance, Volume,
-                                 NodeBalancer, Domain)
-
 
 CLASS_MAP = {
-    'linode': Instance,
-    'domain': Domain,
-    'nodebalancer': NodeBalancer,
-    'volume': Volume,
+    "linode": Instance,
+    "domain": Domain,
+    "nodebalancer": NodeBalancer,
+    "volume": Volume,
 }
 
 
 class Tag(Base):
-    api_endpoint = '/tags/{label}'
-    id_attribute = 'label'
+    """
+    A User-defined labels attached to objects in your Account, such as Linodes.
+    Used for specifying and grouping attributes of objects that are relevant to the User.
+
+    API Documentation: https://www.linode.com/docs/api/tags/#tags-list
+    """
+
+    api_endpoint = "/tags/{label}"
+    id_attribute = "label"
 
     properties = {
-        'label': Property(identifier=True),
+        "label": Property(identifier=True),
     }
 
     def _get_raw_objects(self):
         """
         Helper function to populate the first page of raw objects for this tag.
         This has the side effect of creating the ``_raw_objects`` attribute of
         this object.
         """
-        if not hasattr(self, '_raw_objects'):
+        if not hasattr(self, "_raw_objects"):
             result = self._client.get(type(self).api_endpoint, model=self)
 
             # I want to cache this to avoid making duplicate requests, but I don't
             # want it in the __init__
-            self._raw_objects = result # pylint: disable=attribute-defined-outside-init
+            self._raw_objects = result
 
         return self._raw_objects
 
     def _api_get(self):
         """
         Override the default behavior and just return myself if I exist - this
         is how the python library works, but calling a GET to this endpoint in
@@ -55,57 +61,74 @@
         return self
 
     @property
     def objects(self):
         """
         Returns a list of objects with this Tag.  This list may contain any
         taggable object type.
+
+        API Documentation: https://www.linode.com/docs/api/tags/#tagged-objects-list
+
+        :returns: Objects with this Tag
+        :rtype: PaginatedList of objects with this Tag
         """
         data = self._get_raw_objects()
 
-        return PaginatedList.make_paginated_list(data, self._client, TaggedObjectProxy,
-                                                 page_url=type(self).api_endpoint.format(**vars(self)))
+        return PaginatedList.make_paginated_list(
+            data,
+            self._client,
+            TaggedObjectProxy,
+            page_url=type(self).api_endpoint.format(**vars(self)),
+        )
 
 
 class TaggedObjectProxy:
     """
     This class accepts an object from a list of Tagged objects and returns
     the correct type of object based on the response data.
 
     .. warning::
 
        It is incorrect to instantiate this class.  This class is a proxy for the
        enveloped objects returned from the tagged objects collection, and should
        only be used in that context.
     """
-    id_attribute = 'type' # the envelope containing tagged objects has a `type` field
-                          # that defined what type of object is in the envelope.  We'll
-                          # use that as the ID for the proxy class so ``make_instance``
-                          # below can easily tell what type it should actually be
-                          # making and returning.
+
+    id_attribute = (
+        "type"  # the envelope containing tagged objects has a `type` field
+    )
+    # that defined what type of object is in the envelope.  We'll
+    # use that as the ID for the proxy class so ``make_instance``
+    # below can easily tell what type it should actually be
+    # making and returning.
 
     @classmethod
     def make_instance(cls, id, client, parent_id=None, json=None):
         """
         Overrides Base's ``make_instance`` to allow dynamic creation of objects
         based on the defined type in the response json.
 
         :param cls: The class this was called on
         :param id: The id of the instance to create
         :param client: The client to use for this instance
         :param parent_id: The parent id for derived classes
         :param json: The JSON to populate the instance with
 
         :returns: A new instance of this type, populated with json
+        :rtype: TaggedObjectProxy
         """
-        make_cls = CLASS_MAP.get(id) # in this case, ID is coming in as the type
+        make_cls = CLASS_MAP.get(
+            id
+        )  # in this case, ID is coming in as the type
 
         if make_cls is None:
             # we don't recognize this entity type - do nothing?
             return None
 
         # discard the envelope
-        real_json = json['data']
-        real_id = real_json['id']
+        real_json = json["data"]
+        real_id = real_json["id"]
 
         # make the real object type
-        return Base.make(real_id, client, make_cls, parent_id=None, json=real_json)
+        return Base.make(
+            real_id, client, make_cls, parent_id=None, json=real_json
+        )
```

### Comparing `linode_api4-5.3.0/linode_api4/paginated_list.py` & `linode_api4-5.4.0/linode_api4/paginated_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,27 +25,38 @@
     You may access the number of items in a collection by calling `len` on the
     PaginatedList::
 
        num_linodes = len(linodes)
 
     This will _not_ emit another API request.
     """
-    def __init__(self, client, page_endpoint, page=[], max_pages=1,
-            total_items=None, parent_id=None, filters=None):
+
+    def __init__(
+        self,
+        client,
+        page_endpoint,
+        page=[],
+        max_pages=1,
+        total_items=None,
+        parent_id=None,
+        filters=None,
+    ):
         self.client = client
         self.page_endpoint = page_endpoint
         self.query_filters = filters
         self.page_size = len(page)
         self.max_pages = max_pages
-        self.lists = [ None for _ in range(0, self.max_pages) ]
+        self.lists = [None for _ in range(0, self.max_pages)]
         if self.lists:
             self.lists[0] = page
-        self.list_cls = type(page[0]) if page else None # TODO if this is None that's bad
+        self.list_cls = (
+            type(page[0]) if page else None
+        )  # TODO if this is None that's bad
         self.objects_parent_id = parent_id
-        self.cur = 0 # for being a generator
+        self.cur = 0  # for being a generator
 
         self.total_items = total_items
         if not total_items:
             self.total_items = len(page)
 
     def first(self):
         """
@@ -81,39 +92,49 @@
             return self[0]
         raise ValueError("List {} has more than one element!".format(self))
 
     def __repr__(self):
         return "PaginatedList ({} items)".format(self.total_items)
 
     def _load_page(self, page_number):
-        j = self.client.get("/{}?page={}&page_size={}".format(self.page_endpoint, page_number+1, self.page_size),
-                filters=self.query_filters)
-
-        if j['pages'] != self.max_pages or j['results'] != len(self):
-            raise RuntimeError('List {} has changed since creation!'.format(self))
-
-        l = PaginatedList.make_list(j["data"], self.client, self.list_cls,
-                parent_id=self.objects_parent_id)
+        j = self.client.get(
+            "/{}?page={}&page_size={}".format(
+                self.page_endpoint, page_number + 1, self.page_size
+            ),
+            filters=self.query_filters,
+        )
+
+        if j["pages"] != self.max_pages or j["results"] != len(self):
+            raise RuntimeError(
+                "List {} has changed since creation!".format(self)
+            )
+
+        l = PaginatedList.make_list(
+            j["data"],
+            self.client,
+            self.list_cls,
+            parent_id=self.objects_parent_id,
+        )
         self.lists[page_number] = l
 
     def __getitem__(self, index):
         # this comes in here now, but we're hadling it elsewhere
         if isinstance(index, slice):
             return self._get_slice(index)
 
         # handle negative indexing
         if index < 0:
             index = len(self) + index
             if index < 0:
-                raise IndexError('list index out of range')
+                raise IndexError("list index out of range")
 
         if index >= self.page_size * self.max_pages:
-            raise IndexError('list index out of range')
+            raise IndexError("list index out of range")
         normalized_index = index % self.page_size
-        target_page = math.ceil((index+1.0)/self.page_size)-1
+        target_page = math.ceil((index + 1.0) / self.page_size) - 1
         target_page = int(target_page)
 
         if not self.lists[target_page]:
             self._load_page(target_page)
 
         return self.lists[target_page][normalized_index]
 
@@ -123,48 +144,52 @@
     def _get_slice(self, s):
         # get range
         i = s.start if s.start is not None else 0
         j = s.stop if s.stop is not None else self.total_items
 
         # we do not support steps outside of 1 yet
         if s.step is not None and s.step != 1:
-            raise NotImplementedError('Only step sizes of 1 are currently supported.')
+            raise NotImplementedError(
+                "Only step sizes of 1 are currently supported."
+            )
 
         # if i or j are negative, normalize them
         if i < 0:
             i = self.total_items + i
 
         if j < 0:
             j = self.total_items + j
 
         # if i or j are still negative, that's an IndexError
         if i < 0 or j < 0:
-            raise IndexError('list index out of range')
+            raise IndexError("list index out of range")
 
         # if we're going nowhere or backward, return nothing
         if j <= i:
             return []
 
         result = []
 
         for c in range(i, j):
             result.append(self[c])
 
         return result
 
     def __setitem__(self, index, value):
-        raise AttributeError('Assigning to indicies in paginated lists is not supported')
+        raise AttributeError(
+            "Assigning to indicies in paginated lists is not supported"
+        )
 
     def __delitem__(self, index):
-        raise AttributeError('Deleting from paginated lists is not supported')
+        raise AttributeError("Deleting from paginated lists is not supported")
 
     def __next__(self):
         if self.cur < len(self):
             self.cur += 1
-            return self[self.cur-1]
+            return self[self.cur - 1]
         else:
             raise StopIteration()
 
     @staticmethod
     def make_list(json_arr, client, cls, parent_id=None):
         """
         Returns a list of Populated objects of the given class type.  This
@@ -177,28 +202,32 @@
         :returns: A list of models from the JSON
         """
         result = []
 
         for obj in json_arr:
             id_val = None
 
-            if 'id' in obj:
-                id_val = obj['id']
-            elif hasattr(cls, 'id_attribute') and getattr(cls, 'id_attribute') in obj:
-                id_val = obj[getattr(cls, 'id_attribute')]
+            if "id" in obj:
+                id_val = obj["id"]
+            elif (
+                hasattr(cls, "id_attribute")
+                and getattr(cls, "id_attribute") in obj
+            ):
+                id_val = obj[getattr(cls, "id_attribute")]
             else:
                 continue
             o = cls.make_instance(id_val, client, parent_id=parent_id, json=obj)
             result.append(o)
 
         return result
 
     @staticmethod
-    def make_paginated_list(json, client, cls, parent_id=None, page_url=None,
-            filters=None):
+    def make_paginated_list(
+        json, client, cls, parent_id=None, page_url=None, filters=None
+    ):
         """
         Returns a PaginatedList populated with the first page of data provided,
         and the ability to load additional pages.  This should not be called
         outside of the :any:`LinodeClient` class.
 
         :param json: The JSON list to use as the first page
         :param client: A LinodeClient to use to load additional pages
@@ -208,11 +237,20 @@
         :param filters: The filters used when making the call that generated
                         this list.  If not provided, this will fail when
                         loading additional pages.
 
         :returns: An instance of PaginatedList that will represent the entire
                   collection whose first page is json
         """
-        l = PaginatedList.make_list(json["data"], client, cls, parent_id=parent_id)
-        p = PaginatedList(client, page_url, page=l, max_pages=json['pages'],
-                total_items=json['results'], parent_id=parent_id, filters=filters)
+        l = PaginatedList.make_list(
+            json["data"], client, cls, parent_id=parent_id
+        )
+        p = PaginatedList(
+            client,
+            page_url,
+            page=l,
+            max_pages=json["pages"],
+            total_items=json["results"],
+            parent_id=parent_id,
+            filters=filters,
+        )
         return p
```

### Comparing `linode_api4-5.3.0/linode_api4.egg-info/PKG-INFO` & `linode_api4-5.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
-Name: linode-api4
-Version: 5.3.0
+Name: linode_api4
+Version: 5.4.0
 Summary: The official python SDK for Linode API v4
 Home-page: https://github.com/linode/linode_api4-python
 Author: Linode
 Author-email: developers@linode.com
 License: BSD 3-Clause License
 Keywords: linode cloud hosting infrastructure
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE
 
 linode_api4
 ===========
 
 The official python library for the `Linode API v4`_ in python.
 
 .. _Linode API v4: https://developers.linode.com/api/v4/
 
-.. image:: https://travis-ci.com/linode/linode_api4-python.svg?branch=master
-    :target: https://travis-ci.com/linode/linode_api4-python
+.. image:: https://img.shields.io/github/actions/workflow/status/linode/linode_api4-python/main.yml?label=tests
+    :target: https://img.shields.io/github/actions/workflow/status/linode/linode_api4-python/main.yml?label=tests
 
 .. image:: https://badge.fury.io/py/linode-api4.svg
    :target: https://badge.fury.io/py/linode-api4
 
 .. image:: https://readthedocs.org/projects/linode-api4/badge/?version=latest
    :target: https://linode-api4.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
@@ -48,21 +50,70 @@
 
 To build and install this package:
 
 - Clone this repository
 - ``./setup.py install``
 
 Usage
------
+=====
+
+Quick Start
+-----------
+
+In order to authenticate with the Linode API, you will first need to create a
+`Linode Personal Access Token`_ with your desired account permissions.
+
+The following code sample can help you quickly get started using this package.
+
+.. code-block:: python
+
+    from linode_api4 import LinodeClient, Instance
+
+    # Create a Linode API client
+    client = LinodeClient("MY_PERSONAL_ACCESS_TOKEN")
+
+    # Create a new Linode
+    new_linode, root_pass = client.linode.instance_create(
+        ltype="g6-nanode-1",
+        region="us-southeast",
+        image="linode/ubuntu22.04",
+        label="my-ubuntu-linode"
+    )
+
+    # Print info about the Linode
+    print("Linode IP:", new_linode.ipv4[0])
+    print("Linode Root Password:", root_pass)
+
+    # List all Linodes on the account
+    my_linodes = client.linode.instances()
+
+    # Print the Label of every Linode on the account
+    print("All Instances:")
+    for instance in my_linodes:
+        print(instance.label)
 
-Check out the `Getting Started guide`_ to start using this library, or read
-`the docs`_ for extensive documentation.
+    # List Linodes in the us-southeast region
+    specific_linodes = client.linode.instances(
+        Instance.region == "us-southeast"
+    )
 
-.. _Getting Started guide: http://linode_api4.readthedocs.io/en/latest/guides/getting_started.html
-.. _the docs: http://linode_api4.readthedocs.io/en/latest/index.html
+    # Print the label of each Linode in us-southeast
+    print("Instances in us-southeast:")
+    for instance in specific_linodes:
+        print(instance.label)
+
+    # Delete the new instance
+    new_linode.delete()
+
+Check out the `Getting Started guide`_ for more details on getting started
+with this library, or read `the docs`_ for more extensive documentation.
+
+.. _Linode Personal Access Token: https://www.linode.com/docs/products/tools/api/guides/manage-api-tokens/
+.. _Getting Started guide: https://linode-api4.readthedocs.io/en/latest/guides/getting_started.html
+.. _the docs: https://linode-api4.readthedocs.io/en/latest/index.html
 
 Examples
 --------
 
 See the `Install on a Linode`_ example project for a simple use case demonstrating
 many of the features of this library.
 
@@ -107,21 +158,33 @@
 .. _tox: http://tox.readthedocs.io
 
 Documentation
 -------------
 
 This library is documented with Sphinx_.  Docs live in the ``docs`` directory.
 The easiest way to build the docs is to run ``sphinx-autobuild`` in that
-folder.
+folder::
+
+    sphinx-autobuild docs docs/build
+
+After running this command, ``sphinx-autobuild`` will host a local web server
+with the rendered documentation.
 
 Classes and functions inside the library should be annotated with sphinx-compliant
 docstrings which will be used to automatically generate documentation for the
 library.  When contributing, be sure to update documentation or include new
 docstrings where applicable to keep the library's documentation up to date
 and useful.
 
 **Missing or inaccurate documentation is a bug**.  If you notice that the
 documentation for this library is out of date or unclear, please
 `open an issue`_ to make us aware of the problem.
 
 .. _Sphinx: http://www.sphinx-doc.org/en/master/index.html
 .. _open an issue: https://github.com/linode/linode_api4-python/issues/new
+
+Contributing
+------------
+
+Please follow the `Contributing Guidelines`_ when making a contribution.
+
+.. _Contributing Guidelines: https://github.com/linode/linode_api4-python/blob/master/CONTRIBUTING.md
```

### Comparing `linode_api4-5.3.0/setup.py` & `linode_api4-5.4.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,78 @@
 #!/usr/bin/env python3
 """
 A setuptools based setup module
 
 Based on a template here:
 https://github.com/pypa/sampleproject/blob/master/setup.py
 """
-
+import os
 # Always prefer setuptools over distutils
 import sys
 # To use a consistent encoding
 from codecs import open
 from os import path
 from unittest import TestLoader
 
 from setuptools import find_packages, setup
 
 here = path.abspath(path.dirname(__file__))
 
+
 def get_test_suite():
     test_loader = TestLoader()
     return test_loader.discover('test', pattern='*_test.py')
 
+
+def get_baked_version():
+    """
+    Attempts to read the version from the baked_version file
+    """
+    with open("./baked_version", "r", encoding="utf-8") as f:
+        result = f.read()
+
+    return result
+
+
+def bake_version(v):
+    """
+    Writes the given version to the baked_version file
+    """
+    with open("./baked_version", "w", encoding="utf-8") as f:
+        f.write(v)
+
+
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
+# If there's already a baked version, use it rather than attempting
+# to resolve the version from env.
+# This is useful for installing from an SDist where the version
+# cannot be dynamically resolved.
+#
+# NOTE: baked_version is deleted when running `make build` and `make install`,
+# so it should always be recreated during the build process.
+if path.isfile("baked_version"):
+    version = get_baked_version()
+else:
+    # Otherwise, retrieve and bake the version as normal
+    version = os.getenv("LINODE_SDK_VERSION", "0.0.0")
+    bake_version(version)
+
+if version.startswith("v"):
+    version = version[1:]
+
 setup(
     name='linode_api4',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='5.3.0',
+    version=version,
 
     description='The official python SDK for Linode API v4',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://github.com/linode/linode_api4-python',
 
@@ -61,31 +98,33 @@
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: BSD License',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 
     # What does your project relate to?
     keywords='linode cloud hosting infrastructure',
 
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     packages=find_packages(exclude=['contrib', 'docs', 'test', 'test.*']),
 
     # What do we need for this to run
-    python_requires=">=3.6",
+    python_requires=">=3.7",
 
     install_requires=[
         "requests",
     ],
 
     extras_require={
         "test": ["tox"],
     },
-    test_suite = 'setup.get_test_suite'
+    test_suite='setup.get_test_suite'
 )
```

### Comparing `linode_api4-5.3.0/test/base.py` & `linode_api4-5.4.0/test/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from linode_api4 import LinodeClient
 
 from .fixtures import TestFixtures
 
 FIXTURES = TestFixtures()
 
+
 class MockResponse:
     def __init__(self, status_code, json, headers={}):
         self.status_code = status_code
         self._json = json
         # Headers is a dict, do not want to use a getter here
         self.headers = headers
 
@@ -26,15 +27,15 @@
 
     :param url: The URL being accessed whose JSON is to be returned
 
     :returns: A dict containing the loaded JSON from that file
     """
     formatted_url = url
 
-    while formatted_url.startswith('/'):
+    while formatted_url.startswith("/"):
         formatted_url = formatted_url[1:]
 
     return FIXTURES.get_fixture(formatted_url)
 
 
 def mock_get(url, headers=None, data=None):
     """
@@ -46,38 +47,41 @@
 
 
 class MethodMock:
     """
     This class is used to mock methods on requests and store the parameters
     and headers it was called with.
     """
+
     def __init__(self, method, return_dct):
         """
         Creates and initiates a new MethodMock with the given details
 
         :param method: The HTTP method we are mocking
         :param return_dct: The python dct to returned, or the URL for a JSON
             file to return
         """
         self.method = method
         if isinstance(return_dct, dict):
             self.return_dct = return_dct
         elif isinstance(return_dct, str):
             self.return_dct = load_json(return_dct)
         else:
-            raise TypeError('return_dct must be a dict or a URL from which the '
-                            'JSON could be loaded')
+            raise TypeError(
+                "return_dct must be a dict or a URL from which the "
+                "JSON could be loaded"
+            )
 
     def __enter__(self):
         """
         Begins the method mocking
         """
         self.patch = patch(
-            'linode_api4.linode_client.requests.Session.'+self.method,
-            return_value=MockResponse(200, self.return_dct)
+            "linode_api4.linode_client.requests.Session." + self.method,
+            return_value=MockResponse(200, self.return_dct),
         )
         self.mock = self.patch.start()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         """
         Removed the mocked method
@@ -92,16 +96,15 @@
         return self.mock.call_args
 
     @property
     def call_data_raw(self):
         """
         A shortcut to access the raw call data, not parsed as JSON
         """
-        return self.mock.call_args[1]['data']
-
+        return self.mock.call_args[1]["data"]
 
     @property
     def call_url(self):
         """
         A shortcut to accessing the URL called on the underlying mock.  We
         chop off the first character because our testing base_url has a leading
         / we don't want to see.
@@ -110,78 +113,86 @@
 
     @property
     def call_data(self):
         """
         A shortcut to getting the data param this was called with.  Removes all
         keys whose values are None
         """
-        data = json.loads(self.mock.call_args[1]['data'])
+        data = json.loads(self.mock.call_args[1]["data"])
 
-        return { k: v for k, v in data.items() if v is not None }
+        return {k: v for k, v in data.items() if v is not None}
 
     @property
     def call_headers(self):
         """
         A shortcut to getting the headers param this was called with
         """
-        return self.mock.call_args[1]['headers']
+        return self.mock.call_args[1]["headers"]
+
+    @property
+    def called(self):
+        """
+        A shortcut to check whether the mock function was called.
+        """
+        return self.mock.called
 
 
 class ClientBaseCase(TestCase):
     def setUp(self):
-        self.client = LinodeClient('testing', base_url='/')
+        self.client = LinodeClient("testing", base_url="/")
 
-        self.get_patch = patch('linode_api4.linode_client.requests.Session.get',
-                side_effect=mock_get)
+        self.get_patch = patch(
+            "linode_api4.linode_client.requests.Session.get",
+            side_effect=mock_get,
+        )
         self.get_patch.start()
 
     def tearDown(self):
         self.get_patch.stop()
 
-
     def mock_get(self, return_dct):
         """
         Returns a MethodMock mocking a GET.  This should be used in a with
         statement.
 
         :param return_dct: The JSON that should be returned from this GET
 
         :returns: A MethodMock object who will capture the parameters of the
             mocked requests
         """
-        return MethodMock('get', return_dct)
+        return MethodMock("get", return_dct)
 
     def mock_post(self, return_dct):
         """
         Returns a MethodMock mocking a POST.  This should be used in a with
         statement.
 
         :param return_dct: The JSON that should be returned from this POST
 
         :returns: A MethodMock object who will capture the parameters of the
             mocked requests
         """
-        return MethodMock('post', return_dct)
+        return MethodMock("post", return_dct)
 
     def mock_put(self, return_dct):
         """
         Returns a MethodMock mocking a PUT.  This should be used in a with
         statement.
 
         :param return_dct: The JSON that should be returned from this PUT
 
         :returns: A MethodMock object who will capture the parameters of the
             mocked requests
         """
-        return MethodMock('put', return_dct)
+        return MethodMock("put", return_dct)
 
     def mock_delete(self):
         """
         Returns a MethodMock mocking a DELETE.  This should be used in a with
         statement.
 
         :param return_dct: The JSON that should be returned from this DELETE
 
         :returns: A MethodMock object who will capture the parameters of the
             mocked requests
         """
-        return MethodMock('delete', {})
+        return MethodMock("delete", {})
```

### Comparing `linode_api4-5.3.0/test/fixtures/databases_instances.json` & `linode_api4-5.4.0/test/fixtures/databases_instances.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.3.0/test/fixtures/databases_mongodb_instances.json` & `linode_api4-5.4.0/test/fixtures/databases_mongodb_instances.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.3.0/test/fixtures/databases_mysql_instances.json` & `linode_api4-5.4.0/test/fixtures/databases_mysql_instances.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.3.0/test/fixtures/databases_postgresql_instances.json` & `linode_api4-5.4.0/test/fixtures/databases_postgresql_instances.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.3.0/test/fixtures/databases_types.json` & `linode_api4-5.4.0/test/fixtures/databases_types.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.3.0/test/fixtures/images.json` & `linode_api4-5.4.0/test/fixtures/linode_instances_123_backups.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('automatic', [OrderedDict([('region', 'us-east-1a'), ('finished', "*

 * *            "'2018-01-09T00:01:01'), ('updated', '2018-01-09T00:01:01'), ('disks', "*

 * *            "[OrderedDict([('size', 1024), ('label', 'Debian 8.1 Disk'), ('filesystem', 'ext4')]), "*

 * *            "OrderedDict([('size', 0), ('label', '256MB Swap Image'), ('filesystem', 'swap')])]), "*

 * *            "('label', None), ('configs', ['My Debian 8.1 Profile']), ('id', 12345), ('status', "*

 * *            "'successful'), ('cre […]*

```diff
@@ -1,59 +1,86 @@
 {
-    "data": [
+    "automatic": [
         {
-            "created": "2017-01-01T00:01:01",
-            "created_by": "linode",
-            "deprecated": false,
-            "description": null,
-            "id": "linode/debian9",
-            "is_public": true,
-            "label": "Debian 9",
-            "size": 1100,
-            "status": "available",
-            "type": "manual",
-            "vendor": "Debian"
+            "available": true,
+            "configs": [
+                "My Debian 8.1 Profile"
+            ],
+            "created": "2018-01-09T00:01:01",
+            "disks": [
+                {
+                    "filesystem": "ext4",
+                    "label": "Debian 8.1 Disk",
+                    "size": 1024
+                },
+                {
+                    "filesystem": "swap",
+                    "label": "256MB Swap Image",
+                    "size": 0
+                }
+            ],
+            "finished": "2018-01-09T00:01:01",
+            "id": 12345,
+            "label": null,
+            "region": "us-east-1a",
+            "status": "successful",
+            "type": "auto",
+            "updated": "2018-01-09T00:01:01"
         },
         {
-            "created": "2017-01-01T00:01:01",
-            "created_by": "linode",
-            "deprecated": false,
-            "description": null,
-            "id": "linode/ubuntu17.04",
-            "is_public": true,
-            "label": "Ubuntu 17.04",
-            "size": 1500,
-            "status": "available",
-            "type": "manual",
-            "vendor": "Ubuntu"
+            "available": true,
+            "configs": [
+                "My Debian 8.1 Profile"
+            ],
+            "created": "2018-01-01T00:01:01",
+            "disks": [
+                {
+                    "filesystem": "ext4",
+                    "label": "Debian 8.1 Disk",
+                    "size": 1024
+                },
+                {
+                    "filesystem": "swap",
+                    "label": "256MB Swap Image",
+                    "size": 0
+                }
+            ],
+            "finished": "2018-01-01T00:01:01",
+            "id": 12456,
+            "label": null,
+            "region": "us-east-1a",
+            "status": "successful",
+            "type": "auto",
+            "updated": "2018-01-01T00:01:01"
         },
         {
-            "created": "2017-01-01T00:01:01",
-            "created_by": "linode",
-            "deprecated": false,
-            "description": null,
-            "id": "linode/fedora26",
-            "is_public": true,
-            "label": "Fedora 26",
-            "size": 1500,
-            "status": "available",
-            "type": "manual",
-            "vendor": "Fedora"
-        },
-        {
-            "created": "2017-08-20T14:01:01",
-            "created_by": "testguy",
-            "deprecated": false,
-            "description": null,
-            "id": "private/123",
-            "is_public": false,
-            "label": "Gold Master",
-            "size": 650,
-            "status": "available",
-            "type": "manual",
-            "vendor": null
+            "available": false,
+            "configs": [
+                "My Debian 8.1 Profile"
+            ],
+            "created": "2018-01-07T00:01:01",
+            "disks": [
+                {
+                    "filesystem": "ext4",
+                    "label": "Debian 8.1 Disk",
+                    "size": 1024
+                },
+                {
+                    "filesystem": "swap",
+                    "label": "256MB Swap Image",
+                    "size": 0
+                }
+            ],
+            "finished": "2018-01-07T00:01:01",
+            "id": 12567,
+            "label": null,
+            "region": "us-east-1a",
+            "status": "successful",
+            "type": "auto",
+            "updated": "2018-01-07T00:01:01"
         }
     ],
-    "page": 1,
-    "pages": 1,
-    "results": 4
+    "snapshot": {
+        "current": null,
+        "in_progress": null
+    }
 }
```

### Comparing `linode_api4-5.3.0/test/fixtures/linode_instances.json` & `linode_api4-5.4.0/test/fixtures/images.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7578125%*

 * *Differences: {"'data'": "{2: {'id': 'linode/fedora26', 'status': 'available', 'type': 'manual', 'label': "*

 * *           "'Fedora 26', 'created': '2017-01-01T00:01:01', 'updated': '2020-07-01T04:00:00', "*

 * *           "'description': None, 'deprecated': False, 'created_by': 'linode', 'size': 1500, "*

 * *           "'is_public': True, 'vendor': 'Fedora', 'eol': '2026-07-01T04:00:00', 'expiry': "*

 * *           "'2026-08-01T04:00:00', delete: ['group', 'hypervisor', 'alerts', 'backups', 'specs', "*

 * *           "'ipv6', 'region', 'ipv4', […]*

```diff
@@ -1,83 +1,71 @@
 {
     "data": [
         {
-            "alerts": {
-                "cpu": 90,
-                "io": 5000,
-                "network_in": 5,
-                "network_out": 5,
-                "transfer_quota": 80
-            },
-            "backups": {
-                "enabled": true,
-                "schedule": {
-                    "day": "Scheduling",
-                    "window": "W02"
-                }
-            },
-            "created": "2017-01-01T00:00:00",
-            "group": "test",
-            "hypervisor": "kvm",
-            "id": 123,
-            "image": "linode/ubuntu17.04",
-            "ipv4": [
-                "123.45.67.89"
-            ],
-            "ipv6": "1234:abcd::1234:abcd:89ef:67cd/64",
-            "label": "linode123",
-            "region": "us-east-1a",
-            "specs": {
-                "disk": 30720,
-                "memory": 2048,
-                "transfer": 2000,
-                "vcpus": 1
-            },
-            "status": "running",
-            "tags": [
-                "something"
-            ],
-            "type": "g5-standard-1",
-            "updated": "2017-01-01T00:00:00"
+            "created": "2017-01-01T00:01:01",
+            "created_by": "linode",
+            "deprecated": false,
+            "description": null,
+            "eol": "2026-07-01T04:00:00",
+            "expiry": "2026-08-01T04:00:00",
+            "id": "linode/debian9",
+            "is_public": true,
+            "label": "Debian 9",
+            "size": 1100,
+            "status": "available",
+            "type": "manual",
+            "updated": "2020-07-01T04:00:00",
+            "vendor": "Debian"
         },
         {
-            "alerts": {
-                "cpu": 90,
-                "io": 5000,
-                "network_in": 5,
-                "network_out": 5,
-                "transfer_quota": 80
-            },
-            "backups": {
-                "enabled": false,
-                "schedule": {
-                    "day": null,
-                    "window": null
-                }
-            },
-            "created": "2017-01-01T00:00:00",
-            "group": "test",
-            "hypervisor": "kvm",
-            "id": 456,
-            "image": "linode/debian9",
-            "ipv4": [
-                "123.45.67.89"
-            ],
-            "ipv6": "1234:abcd::1234:abcd:89ef:67cd/64",
-            "label": "linode456",
-            "region": "us-east-1a",
-            "specs": {
-                "disk": 30720,
-                "memory": 2048,
-                "transfer": 2000,
-                "vcpus": 1
-            },
-            "status": "running",
-            "tags": [],
-            "type": "g5-standard-1",
-            "updated": "2017-01-01T00:00:00"
+            "created": "2017-01-01T00:01:01",
+            "created_by": "linode",
+            "deprecated": false,
+            "description": null,
+            "eol": "2026-07-01T04:00:00",
+            "expiry": "2026-08-01T04:00:00",
+            "id": "linode/ubuntu17.04",
+            "is_public": true,
+            "label": "Ubuntu 17.04",
+            "size": 1500,
+            "status": "available",
+            "type": "manual",
+            "updated": "2020-07-01T04:00:00",
+            "vendor": "Ubuntu"
+        },
+        {
+            "created": "2017-01-01T00:01:01",
+            "created_by": "linode",
+            "deprecated": false,
+            "description": null,
+            "eol": "2026-07-01T04:00:00",
+            "expiry": "2026-08-01T04:00:00",
+            "id": "linode/fedora26",
+            "is_public": true,
+            "label": "Fedora 26",
+            "size": 1500,
+            "status": "available",
+            "type": "manual",
+            "updated": "2020-07-01T04:00:00",
+            "vendor": "Fedora"
+        },
+        {
+            "created": "2017-08-20T14:01:01",
+            "created_by": "testguy",
+            "deprecated": false,
+            "description": null,
+            "eol": "2026-07-01T04:00:00",
+            "expiry": "2026-08-01T04:00:00",
+            "id": "private/123",
+            "is_public": false,
+            "label": "Gold Master",
+            "size": 650,
+            "status": "available",
+            "type": "manual",
+            "updated": "2020-07-01T04:00:00",
+            "vendor": null
         }
     ],
     "page": 1,
     "pages": 1,
-    "results": 2
+    "results": 4
 }
```

### Comparing `linode_api4-5.3.0/test/fixtures/linode_instances_123_configs.json` & `linode_api4-5.4.0/test/fixtures/linode_instances_123_configs.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.3.0/test/fixtures/linode_instances_123_configs_456789.json` & `linode_api4-5.4.0/test/fixtures/linode_instances_123_configs_456789.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.3.0/test/fixtures/linode_types.json` & `linode_api4-5.4.0/test/fixtures/linode_types.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333333%*

 * *Differences: {"'data'": "{0: {'successor': None}, 1: {'successor': None}, 2: {'successor': None}, 3: "*

 * *           "{'successor': None}}"}*

```diff
@@ -16,14 +16,15 @@
             "label": "Linode 1024",
             "memory": 1024,
             "network_out": 1000,
             "price": {
                 "hourly": 0.0075,
                 "monthly": 5
             },
+            "successor": null,
             "transfer": 1000,
             "vcpus": 1
         },
         {
             "addons": {
                 "backups": {
                     "price": {
@@ -39,14 +40,15 @@
             "label": "Linode 16384",
             "memory": 16384,
             "network_out": 1000,
             "price": {
                 "hourly": 0.09,
                 "monthly": 60
             },
+            "successor": null,
             "transfer": 5000,
             "vcpus": 1
         },
         {
             "addons": {
                 "backups": {
                     "price": {
@@ -62,14 +64,15 @@
             "label": "Linode 2048",
             "memory": 2048,
             "network_out": 1000,
             "price": {
                 "hourly": 0.015,
                 "monthly": 10
             },
+            "successor": null,
             "transfer": 2000,
             "vcpus": 1
         },
         {
             "addons": {
                 "backups": {
                     "price": {
@@ -85,14 +88,15 @@
             "label": "Linode 4096",
             "memory": 4096,
             "network_out": 1000,
             "price": {
                 "hourly": 0.03,
                 "monthly": 20
             },
+            "successor": null,
             "transfer": 3000,
             "vcpus": 2
         }
     ],
     "page": 1,
     "pages": 1,
     "results": 4
```

### Comparing `linode_api4-5.3.0/test/fixtures/longview_clients.json` & `linode_api4-5.4.0/test/fixtures/longview_clients.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.3.0/test/fixtures/longview_subscriptions.json` & `linode_api4-5.4.0/test/fixtures/longview_subscriptions.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.3.0/test/fixtures/nodebalancers.json` & `linode_api4-5.4.0/test/fixtures/nodebalancers.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.3.0/test/fixtures/nodebalancers_123456_configs.json` & `linode_api4-5.4.0/test/fixtures/nodebalancers_123456_configs.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.3.0/test/fixtures/profile_sshkeys.json` & `linode_api4-5.4.0/test/fixtures/profile_sshkeys.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.3.0/test/fixtures/regions.json` & `linode_api4-5.4.0/test/fixtures/regions.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'data'": "{0: {'label': 'label1'}, 1: {'label': 'label2'}, 2: {'label': 'label3'}, 3: {'label': "*

 * *           "'label4'}, 4: {'label': 'label5'}, 5: {'label': 'label6'}, 6: {'label': 'label7'}, 7: "*

 * *           "{'label': 'label8'}, 8: {'label': 'label9'}, 9: {'label': 'label10'}, 10: {'label': "*

 * *           "'label11'}}"}*

```diff
@@ -4,84 +4,90 @@
             "capabilities": [
                 "Linodes",
                 "NodeBalancers",
                 "Block Storage"
             ],
             "country": "in",
             "id": "ap-west",
+            "label": "label1",
             "resolvers": {
                 "ipv4": "172.105.34.5,172.105.35.5,172.105.36.5,172.105.37.5,172.105.38.5,172.105.39.5,172.105.40.5,172.105.41.5,172.105.42.5,172.105.43.5",
                 "ipv6": "2400:8904::f03c:91ff:fea5:659,2400:8904::f03c:91ff:fea5:9282,2400:8904::f03c:91ff:fea5:b9b3,2400:8904::f03c:91ff:fea5:925a,2400:8904::f03c:91ff:fea5:22cb,2400:8904::f03c:91ff:fea5:227a,2400:8904::f03c:91ff:fea5:924c,2400:8904::f03c:91ff:fea5:f7e2,2400:8904::f03c:91ff:fea5:2205,2400:8904::f03c:91ff:fea5:9207"
             },
             "status": "ok"
         },
         {
             "capabilities": [
                 "Linodes",
                 "NodeBalancers",
                 "Block Storage"
             ],
             "country": "ca",
             "id": "ca-central",
+            "label": "label2",
             "resolvers": {
                 "ipv4": "172.105.0.5,172.105.3.5,172.105.4.5,172.105.5.5,172.105.6.5,172.105.7.5,172.105.8.5,172.105.9.5,172.105.10.5,172.105.11.5",
                 "ipv6": "2600:3c04::f03c:91ff:fea9:f63,2600:3c04::f03c:91ff:fea9:f6d,2600:3c04::f03c:91ff:fea9:f80,2600:3c04::f03c:91ff:fea9:f0f,2600:3c04::f03c:91ff:fea9:f99,2600:3c04::f03c:91ff:fea9:fbd,2600:3c04::f03c:91ff:fea9:fdd,2600:3c04::f03c:91ff:fea9:fe2,2600:3c04::f03c:91ff:fea9:f68,2600:3c04::f03c:91ff:fea9:f4a"
             },
             "status": "ok"
         },
         {
             "capabilities": [
                 "Linodes",
                 "NodeBalancers",
                 "Block Storage"
             ],
             "country": "au",
             "id": "ap-southeast",
+            "label": "label3",
             "resolvers": {
                 "ipv4": "172.105.166.5,172.105.169.5,172.105.168.5,172.105.172.5,172.105.162.5,172.105.170.5,172.105.167.5,172.105.171.5,172.105.181.5,172.105.161.5",
                 "ipv6": "2400:8907::f03c:92ff:fe6e:ec8,2400:8907::f03c:92ff:fe6e:98e4,2400:8907::f03c:92ff:fe6e:1c58,2400:8907::f03c:92ff:fe6e:c299,2400:8907::f03c:92ff:fe6e:c210,2400:8907::f03c:92ff:fe6e:c219,2400:8907::f03c:92ff:fe6e:1c5c,2400:8907::f03c:92ff:fe6e:c24e,2400:8907::f03c:92ff:fe6e:e6b,2400:8907::f03c:92ff:fe6e:e3d"
             },
             "status": "ok"
         },
         {
             "capabilities": [
                 "Linodes",
                 "NodeBalancers",
                 "Block Storage"
             ],
             "country": "us",
             "id": "us-central",
+            "label": "label4",
             "resolvers": {
                 "ipv4": "72.14.179.5,72.14.188.5,173.255.199.5,66.228.53.5,96.126.122.5,96.126.124.5,96.126.127.5,198.58.107.5,198.58.111.5,23.239.24.5",
                 "ipv6": "2600:3c00::2,2600:3c00::9,2600:3c00::7,2600:3c00::5,2600:3c00::3,2600:3c00::8,2600:3c00::6,2600:3c00::4,2600:3c00::c,2600:3c00::b"
             },
             "status": "ok"
         },
         {
             "capabilities": [
                 "Linodes",
                 "NodeBalancers",
                 "Block Storage"
             ],
             "country": "us",
             "id": "us-west",
+            "label": "label5",
             "resolvers": {
                 "ipv4": "173.230.145.5,173.230.147.5,173.230.155.5,173.255.212.5,173.255.219.5,173.255.241.5,173.255.243.5,173.255.244.5,74.207.241.5,74.207.242.5",
                 "ipv6": "2600:3c01::2,2600:3c01::9,2600:3c01::5,2600:3c01::7,2600:3c01::3,2600:3c01::8,2600:3c01::4,2600:3c01::b,2600:3c01::c,2600:3c01::6"
             },
             "status": "ok"
         },
         {
             "capabilities": [
                 "Linodes",
                 "NodeBalancers",
                 "Block Storage"
             ],
             "country": "us",
             "id": "us-southeast",
+            "label": "label6",
             "resolvers": {
                 "ipv4": "74.207.231.5,173.230.128.5,173.230.129.5,173.230.136.5,173.230.140.5,66.228.59.5,66.228.62.5,50.116.35.5,50.116.41.5,23.239.18.5",
                 "ipv6": "2600:3c02::3,2600:3c02::5,2600:3c02::4,2600:3c02::6,2600:3c02::c,2600:3c02::7,2600:3c02::2,2600:3c02::9,2600:3c02::8,2600:3c02::b"
             },
             "status": "ok"
         },
         {
@@ -89,28 +95,30 @@
                 "Linodes",
                 "NodeBalancers",
                 "Block Storage",
                 "Object Storage"
             ],
             "country": "us",
             "id": "us-east",
+            "label": "label7",
             "resolvers": {
                 "ipv4": "66.228.42.5,96.126.106.5,50.116.53.5,50.116.58.5,50.116.61.5,50.116.62.5,66.175.211.5,97.107.133.4,207.192.69.4,207.192.69.5",
                 "ipv6": "2600:3c03::7,2600:3c03::4,2600:3c03::9,2600:3c03::6,2600:3c03::3,2600:3c03::c,2600:3c03::5,2600:3c03::b,2600:3c03::2,2600:3c03::8"
             },
             "status": "ok"
         },
         {
             "capabilities": [
                 "Linodes",
                 "NodeBalancers",
                 "Block Storage"
             ],
             "country": "uk",
             "id": "eu-west",
+            "label": "label8",
             "resolvers": {
                 "ipv4": "178.79.182.5,176.58.107.5,176.58.116.5,176.58.121.5,151.236.220.5,212.71.252.5,212.71.253.5,109.74.192.20,109.74.193.20,109.74.194.20",
                 "ipv6": "2a01:7e00::9,2a01:7e00::3,2a01:7e00::c,2a01:7e00::5,2a01:7e00::6,2a01:7e00::8,2a01:7e00::b,2a01:7e00::4,2a01:7e00::7,2a01:7e00::2"
             },
             "status": "ok"
         },
         {
@@ -118,14 +126,15 @@
                 "Linodes",
                 "NodeBalancers",
                 "Block Storage",
                 "Object Storage"
             ],
             "country": "sg",
             "id": "ap-south",
+            "label": "label9",
             "resolvers": {
                 "ipv4": "139.162.11.5,139.162.13.5,139.162.14.5,139.162.15.5,139.162.16.5,139.162.21.5,139.162.27.5,103.3.60.18,103.3.60.19,103.3.60.20",
                 "ipv6": "2400:8901::5,2400:8901::4,2400:8901::b,2400:8901::3,2400:8901::9,2400:8901::2,2400:8901::8,2400:8901::7,2400:8901::c,2400:8901::6"
             },
             "status": "ok"
         },
         {
@@ -133,28 +142,30 @@
                 "Linodes",
                 "NodeBalancers",
                 "Block Storage",
                 "Object Storage"
             ],
             "country": "de",
             "id": "eu-central",
+            "label": "label10",
             "resolvers": {
                 "ipv4": "139.162.130.5,139.162.131.5,139.162.132.5,139.162.133.5,139.162.134.5,139.162.135.5,139.162.136.5,139.162.137.5,139.162.138.5,139.162.139.5",
                 "ipv6": "2a01:7e01::5,2a01:7e01::9,2a01:7e01::7,2a01:7e01::c,2a01:7e01::2,2a01:7e01::4,2a01:7e01::3,2a01:7e01::6,2a01:7e01::b,2a01:7e01::8"
             },
             "status": "ok"
         },
         {
             "capabilities": [
                 "Linodes",
                 "NodeBalancers",
                 "Block Storage"
             ],
             "country": "jp",
             "id": "ap-northeast",
+            "label": "label11",
             "resolvers": {
                 "ipv4": "139.162.66.5,139.162.67.5,139.162.68.5,139.162.69.5,139.162.70.5,139.162.71.5,139.162.72.5,139.162.73.5,139.162.74.5,139.162.75.5",
                 "ipv6": "2400:8902::3,2400:8902::6,2400:8902::c,2400:8902::4,2400:8902::2,2400:8902::8,2400:8902::7,2400:8902::5,2400:8902::b,2400:8902::9"
             },
             "status": "ok"
         }
     ],
```

### Comparing `linode_api4-5.3.0/test/fixtures/tags_something.json` & `linode_api4-5.4.0/test/fixtures/tags_something.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.3.0/test/fixtures.py` & `linode_api4-5.4.0/test/fixtures.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 import json
 import os
 import sys
 
-FIXTURES_DIR = sys.path[0] + '/test/fixtures'
+FIXTURES_DIR = sys.path[0] + "/test/fixtures"
+
 
 class TestFixtures:
     def __init__(self):
         """
         Creates and loads test fixtures
         """
         self._load_fixtures()
 
     def get_fixture(self, url):
         """
         Returns the test fixture data loaded at the given URL
         """
         return self.fixtures[url]
-    
+
     def _load_fixtures(self):
         """
         Handles loading JSON files and parsing them into responses.  Also splits
         returned lists into individual models that may be returned on their own.
         """
         self.fixtures = {}
 
         for json_file in os.listdir(FIXTURES_DIR):
-            if not json_file.endswith('.json'):
+            if not json_file.endswith(".json"):
                 continue
 
-            with open(FIXTURES_DIR + '/' + json_file) as f:
+            with open(FIXTURES_DIR + "/" + json_file) as f:
                 raw = f.read()
 
             data = json.loads(raw)
 
-            fixture_url = json_file.replace('_', '/')[:-5]
-            
+            fixture_url = json_file.replace("_", "/")[:-5]
+
             self.fixtures[fixture_url] = data
 
-            if 'results' in data:
+            if "results" in data:
                 # this is a paginated response
-                for obj in data['data']:
-                    if 'id' in obj: # tags don't have ids
-                        self.fixtures[fixture_url + '/' + str(obj['id'])] = obj
+                for obj in data["data"]:
+                    if "id" in obj:  # tags, obj-buckets don't have ids
+                        self.fixtures[fixture_url + "/" + str(obj["id"])] = obj
```

### Comparing `linode_api4-5.3.0/test/objects/account_test.py` & `linode_api4-5.4.0/test/objects/support_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,28 @@
-from datetime import datetime
-
 from test.base import ClientBaseCase
 
-from linode_api4.objects import Invoice
+from linode_api4.objects import SupportTicket
 
 
-class InvoiceTest(ClientBaseCase):
+class SupportTest(ClientBaseCase):
     """
-    Tests methods of the Invoice
+    Tests methods of the SupportTicket class
     """
-    def test_get_invoice(self):
-        invoice = Invoice(self.client, 123456)
-        self.assertEqual(invoice._populated, False)
-
-        self.assertEqual(invoice.label, 'Invoice #123456')
-        self.assertEqual(invoice._populated, True)
-
-        self.assertEqual(invoice.date, datetime(2015, 1, 1, 5, 1, 2))
-        self.assertEqual(invoice.total, 9.51)
-
-    def test_get_invoice_items(self):
-        """
-        Tests that you can get items for an invoice
-        """
-        invoice = Invoice(self.client, 123456)
-        items = invoice.items
-
-        self.assertEqual(len(items), 1)
-        item = items[0]
-
-        self.assertEqual(item.label, "Linode 2048 - Example")
-        self.assertEqual(item.type, "hourly")
-        self.assertEqual(item.amount, 9.51)
-        self.assertEqual(item.quantity, 317)
-        self.assertEqual(item.unit_price, "0.03")
-        self.assertEqual(item.from_date, datetime(year=2014, month=12, day=19, hour=0, minute=27, second=2))
-        self.assertEqual(item.to_date, datetime(year=2015, month=1, day=1, hour=4, minute=59, second=59))
+
+    def test_get_support_ticket(self):
+        ticket = SupportTicket(self.client, 123)
+
+        self.assertIsNotNone(ticket.attachments)
+        self.assertFalse(ticket.closable)
+        self.assertIsNotNone(ticket.entity)
+        self.assertEqual(ticket.gravatar_id, "474a1b7373ae0be4132649e69c36ce30")
+        self.assertEqual(ticket.id, 123)
+        self.assertEqual(ticket.opened_by, "some_user")
+        self.assertEqual(ticket.status, "open")
+        self.assertEqual(ticket.updated_by, "some_other_user")
+
+    def test_support_ticket_close(self):
+        ticket = SupportTicket(self.client, 123)
+
+        with self.mock_post({}) as m:
+            ticket.support_ticket_close()
+            self.assertEqual(m.call_url, "/support/tickets/123/close")
```

### Comparing `linode_api4-5.3.0/test/objects/database_test.py` & `linode_api4-5.4.0/test/objects/database_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from linode_api4 import PostgreSQLDatabase, MongoDBDatabase
 from test.base import ClientBaseCase
 
+from linode_api4 import MongoDBDatabase, PostgreSQLDatabase
 from linode_api4.objects import MySQLDatabase
 
 
 class DatabaseTest(ClientBaseCase):
     """
     Tests methods of the DatabaseGroup class
     """
@@ -12,51 +12,57 @@
     def test_get_types(self):
         """
         Test that database types are properly handled
         """
         types = self.client.database.types()
 
         self.assertEqual(len(types), 1)
-        self.assertEqual(types[0].type_class, 'nanode')
-        self.assertEqual(types[0].id, 'g6-nanode-1')
+        self.assertEqual(types[0].type_class, "nanode")
+        self.assertEqual(types[0].id, "g6-nanode-1")
         self.assertEqual(types[0].engines.mongodb[0].price.monthly, 20)
 
     def test_get_engines(self):
         """
         Test that database engines are properly handled
         """
         engines = self.client.database.engines()
 
         self.assertEqual(len(engines), 2)
 
-        self.assertEqual(engines[0].engine, 'mysql')
-        self.assertEqual(engines[0].id, 'mysql/8.0.26')
-        self.assertEqual(engines[0].version, '8.0.26')
-
-        self.assertEqual(engines[1].engine, 'postgresql')
-        self.assertEqual(engines[1].id, 'postgresql/10.14')
-        self.assertEqual(engines[1].version, '10.14')
+        self.assertEqual(engines[0].engine, "mysql")
+        self.assertEqual(engines[0].id, "mysql/8.0.26")
+        self.assertEqual(engines[0].version, "8.0.26")
+
+        self.assertEqual(engines[1].engine, "postgresql")
+        self.assertEqual(engines[1].id, "postgresql/10.14")
+        self.assertEqual(engines[1].version, "10.14")
 
     def test_get_databases(self):
         """
         Test that databases are properly handled
         """
         dbs = self.client.database.instances()
 
         self.assertEqual(len(dbs), 1)
-        self.assertEqual(dbs[0].allow_list[1], '192.0.1.0/24')
+        self.assertEqual(dbs[0].allow_list[1], "192.0.1.0/24")
         self.assertEqual(dbs[0].cluster_size, 3)
         self.assertEqual(dbs[0].encrypted, False)
-        self.assertEqual(dbs[0].engine, 'mysql')
-        self.assertEqual(dbs[0].hosts.primary, 'lin-123-456-mysql-mysql-primary.servers.linodedb.net')
-        self.assertEqual(dbs[0].hosts.secondary, 'lin-123-456-mysql-primary-private.servers.linodedb.net')
+        self.assertEqual(dbs[0].engine, "mysql")
+        self.assertEqual(
+            dbs[0].hosts.primary,
+            "lin-123-456-mysql-mysql-primary.servers.linodedb.net",
+        )
+        self.assertEqual(
+            dbs[0].hosts.secondary,
+            "lin-123-456-mysql-primary-private.servers.linodedb.net",
+        )
         self.assertEqual(dbs[0].id, 123)
-        self.assertEqual(dbs[0].region, 'us-east')
+        self.assertEqual(dbs[0].region, "us-east")
         self.assertEqual(dbs[0].updates.duration, 3)
-        self.assertEqual(dbs[0].version, '8.0.26')
+        self.assertEqual(dbs[0].version, "8.0.26")
 
     def test_database_instance(self):
         """
         Ensures that the .instance attribute properly translates database types
         """
 
         dbs = self.client.database.instances()
@@ -74,490 +80,547 @@
     def test_get_instances(self):
         """
         Test that database types are properly handled
         """
         dbs = self.client.database.mysql_instances()
 
         self.assertEqual(len(dbs), 1)
-        self.assertEqual(dbs[0].allow_list[1], '192.0.1.0/24')
+        self.assertEqual(dbs[0].allow_list[1], "192.0.1.0/24")
         self.assertEqual(dbs[0].cluster_size, 3)
         self.assertEqual(dbs[0].encrypted, False)
-        self.assertEqual(dbs[0].engine, 'mysql')
-        self.assertEqual(dbs[0].hosts.primary, 'lin-123-456-mysql-mysql-primary.servers.linodedb.net')
-        self.assertEqual(dbs[0].hosts.secondary, 'lin-123-456-mysql-primary-private.servers.linodedb.net')
+        self.assertEqual(dbs[0].engine, "mysql")
+        self.assertEqual(
+            dbs[0].hosts.primary,
+            "lin-123-456-mysql-mysql-primary.servers.linodedb.net",
+        )
+        self.assertEqual(
+            dbs[0].hosts.secondary,
+            "lin-123-456-mysql-primary-private.servers.linodedb.net",
+        )
         self.assertEqual(dbs[0].id, 123)
-        self.assertEqual(dbs[0].region, 'us-east')
+        self.assertEqual(dbs[0].region, "us-east")
         self.assertEqual(dbs[0].updates.duration, 3)
-        self.assertEqual(dbs[0].version, '8.0.26')
+        self.assertEqual(dbs[0].version, "8.0.26")
 
     def test_create(self):
         """
         Test that MySQL databases can be created
         """
 
-        with self.mock_post('/databases/mysql/instances') as m:
+        with self.mock_post("/databases/mysql/instances") as m:
             # We don't care about errors here; we just want to
             # validate the request.
             try:
                 self.client.database.mysql_create(
-                    'cool',
-                    'us-southeast',
-                    'mysql/8.0.26',
-                    'g6-standard-1',
-                    cluster_size=3
+                    "cool",
+                    "us-southeast",
+                    "mysql/8.0.26",
+                    "g6-standard-1",
+                    cluster_size=3,
                 )
             except Exception:
                 pass
 
-            self.assertEqual(m.method, 'post')
-            self.assertEqual(m.call_url, '/databases/mysql/instances')
-            self.assertEqual(m.call_data['label'], 'cool')
-            self.assertEqual(m.call_data['region'], 'us-southeast')
-            self.assertEqual(m.call_data['engine'], 'mysql/8.0.26')
-            self.assertEqual(m.call_data['type'], 'g6-standard-1')
-            self.assertEqual(m.call_data['cluster_size'], 3)
+            self.assertEqual(m.method, "post")
+            self.assertEqual(m.call_url, "/databases/mysql/instances")
+            self.assertEqual(m.call_data["label"], "cool")
+            self.assertEqual(m.call_data["region"], "us-southeast")
+            self.assertEqual(m.call_data["engine"], "mysql/8.0.26")
+            self.assertEqual(m.call_data["type"], "g6-standard-1")
+            self.assertEqual(m.call_data["cluster_size"], 3)
 
     def test_update(self):
         """
         Test that the MySQL database can be updated
         """
 
-        with self.mock_put('/databases/mysql/instances/123') as m:
-            new_allow_list = ['192.168.0.1/32']
+        with self.mock_put("/databases/mysql/instances/123") as m:
+            new_allow_list = ["192.168.0.1/32"]
 
             db = MySQLDatabase(self.client, 123)
 
             db.updates.day_of_week = 2
             db.allow_list = new_allow_list
-            db.label = 'cool'
+            db.label = "cool"
 
             db.save()
 
-            self.assertEqual(m.method, 'put')
-            self.assertEqual(m.call_url, '/databases/mysql/instances/123')
-            self.assertEqual(m.call_data['label'], 'cool')
-            self.assertEqual(m.call_data['updates']['day_of_week'], 2)
-            self.assertEqual(m.call_data['allow_list'], new_allow_list)
+            self.assertEqual(m.method, "put")
+            self.assertEqual(m.call_url, "/databases/mysql/instances/123")
+            self.assertEqual(m.call_data["label"], "cool")
+            self.assertEqual(m.call_data["updates"]["day_of_week"], 2)
+            self.assertEqual(m.call_data["allow_list"], new_allow_list)
 
     def test_list_backups(self):
         """
         Test that MySQL backups list properly
         """
 
         db = MySQLDatabase(self.client, 123)
         backups = db.backups
 
         self.assertEqual(len(backups), 1)
 
         self.assertEqual(backups[0].id, 456)
-        self.assertEqual(backups[0].label, 'Scheduled - 02/04/22 11:11 UTC-XcCRmI')
-        self.assertEqual(backups[0].type, 'auto')
+        self.assertEqual(
+            backups[0].label, "Scheduled - 02/04/22 11:11 UTC-XcCRmI"
+        )
+        self.assertEqual(backups[0].type, "auto")
 
     def test_create_backup(self):
         """
         Test that MySQL database backups can be updated
         """
 
-        with self.mock_post('/databases/mysql/instances/123/backups') as m:
+        with self.mock_post("/databases/mysql/instances/123/backups") as m:
             db = MySQLDatabase(self.client, 123)
 
             # We don't care about errors here; we just want to
             # validate the request.
             try:
-                db.backup_create('mybackup', target='secondary')
+                db.backup_create("mybackup", target="secondary")
             except Exception:
                 pass
 
-            self.assertEqual(m.method, 'post')
-            self.assertEqual(m.call_url, '/databases/mysql/instances/123/backups')
-            self.assertEqual(m.call_data['label'], 'mybackup')
-            self.assertEqual(m.call_data['target'], 'secondary')
+            self.assertEqual(m.method, "post")
+            self.assertEqual(
+                m.call_url, "/databases/mysql/instances/123/backups"
+            )
+            self.assertEqual(m.call_data["label"], "mybackup")
+            self.assertEqual(m.call_data["target"], "secondary")
 
     def test_backup_restore(self):
         """
         Test that MySQL database backups can be restored
         """
 
-        with self.mock_post('/databases/mysql/instances/123/backups/456/restore') as m:
+        with self.mock_post(
+            "/databases/mysql/instances/123/backups/456/restore"
+        ) as m:
             db = MySQLDatabase(self.client, 123)
 
             db.backups[0].restore()
 
-            self.assertEqual(m.method, 'post')
-            self.assertEqual(m.call_url, '/databases/mysql/instances/123/backups/456/restore')
+            self.assertEqual(m.method, "post")
+            self.assertEqual(
+                m.call_url, "/databases/mysql/instances/123/backups/456/restore"
+            )
 
     def test_patch(self):
         """
         Test MySQL Database patching logic.
         """
-        with self.mock_post('/databases/mysql/instances/123/patch') as m:
+        with self.mock_post("/databases/mysql/instances/123/patch") as m:
             db = MySQLDatabase(self.client, 123)
 
             db.patch()
 
-            self.assertEqual(m.method, 'post')
-            self.assertEqual(m.call_url, '/databases/mysql/instances/123/patch')
+            self.assertEqual(m.method, "post")
+            self.assertEqual(m.call_url, "/databases/mysql/instances/123/patch")
 
     def test_get_ssl(self):
         """
         Test MySQL SSL cert logic
         """
         db = MySQLDatabase(self.client, 123)
 
         ssl = db.ssl
 
-        self.assertEqual(ssl.ca_certificate, 'LS0tLS1CRUdJ...==')
+        self.assertEqual(ssl.ca_certificate, "LS0tLS1CRUdJ...==")
 
     def test_get_credentials(self):
         """
         Test MySQL credentials logic
         """
         db = MySQLDatabase(self.client, 123)
 
         creds = db.credentials
 
-        self.assertEqual(creds.password, 's3cur3P@ssw0rd')
-        self.assertEqual(creds.username, 'linroot')
+        self.assertEqual(creds.password, "s3cur3P@ssw0rd")
+        self.assertEqual(creds.username, "linroot")
 
     def test_reset_credentials(self):
         """
         Test resetting MySQL credentials
         """
-        with self.mock_post('/databases/mysql/instances/123/credentials/reset') as m:
+        with self.mock_post(
+            "/databases/mysql/instances/123/credentials/reset"
+        ) as m:
             db = MySQLDatabase(self.client, 123)
 
             db.credentials_reset()
 
-            self.assertEqual(m.method, 'post')
-            self.assertEqual(m.call_url, '/databases/mysql/instances/123/credentials/reset')
+            self.assertEqual(m.method, "post")
+            self.assertEqual(
+                m.call_url, "/databases/mysql/instances/123/credentials/reset"
+            )
 
 
 class PostgreSQLDatabaseTest(ClientBaseCase):
     """
     Tests methods of the PostgreSQLDatabase class
     """
 
     def test_get_instances(self):
         """
         Test that database types are properly handled
         """
         dbs = self.client.database.postgresql_instances()
 
         self.assertEqual(len(dbs), 1)
-        self.assertEqual(dbs[0].allow_list[1], '192.0.1.0/24')
+        self.assertEqual(dbs[0].allow_list[1], "192.0.1.0/24")
         self.assertEqual(dbs[0].cluster_size, 3)
         self.assertEqual(dbs[0].encrypted, False)
-        self.assertEqual(dbs[0].engine, 'postgresql')
-        self.assertEqual(dbs[0].hosts.primary, 'lin-0000-000-pgsql-primary.servers.linodedb.net')
-        self.assertEqual(dbs[0].hosts.secondary, 'lin-0000-000-pgsql-primary-private.servers.linodedb.net')
+        self.assertEqual(dbs[0].engine, "postgresql")
+        self.assertEqual(
+            dbs[0].hosts.primary,
+            "lin-0000-000-pgsql-primary.servers.linodedb.net",
+        )
+        self.assertEqual(
+            dbs[0].hosts.secondary,
+            "lin-0000-000-pgsql-primary-private.servers.linodedb.net",
+        )
         self.assertEqual(dbs[0].id, 123)
-        self.assertEqual(dbs[0].region, 'us-east')
+        self.assertEqual(dbs[0].region, "us-east")
         self.assertEqual(dbs[0].updates.duration, 3)
-        self.assertEqual(dbs[0].version, '13.2')
+        self.assertEqual(dbs[0].version, "13.2")
 
     def test_create(self):
         """
         Test that PostgreSQL databases can be created
         """
 
-        with self.mock_post('/databases/postgresql/instances') as m:
+        with self.mock_post("/databases/postgresql/instances") as m:
             # We don't care about errors here; we just want to
             # validate the request.
             try:
                 self.client.database.postgresql_create(
-                    'cool',
-                    'us-southeast',
-                    'postgresql/13.2',
-                    'g6-standard-1',
-                    cluster_size=3
+                    "cool",
+                    "us-southeast",
+                    "postgresql/13.2",
+                    "g6-standard-1",
+                    cluster_size=3,
                 )
             except Exception:
                 pass
 
-            self.assertEqual(m.method, 'post')
-            self.assertEqual(m.call_url, '/databases/postgresql/instances')
-            self.assertEqual(m.call_data['label'], 'cool')
-            self.assertEqual(m.call_data['region'], 'us-southeast')
-            self.assertEqual(m.call_data['engine'], 'postgresql/13.2')
-            self.assertEqual(m.call_data['type'], 'g6-standard-1')
-            self.assertEqual(m.call_data['cluster_size'], 3)
+            self.assertEqual(m.method, "post")
+            self.assertEqual(m.call_url, "/databases/postgresql/instances")
+            self.assertEqual(m.call_data["label"], "cool")
+            self.assertEqual(m.call_data["region"], "us-southeast")
+            self.assertEqual(m.call_data["engine"], "postgresql/13.2")
+            self.assertEqual(m.call_data["type"], "g6-standard-1")
+            self.assertEqual(m.call_data["cluster_size"], 3)
 
     def test_update(self):
         """
         Test that the PostgreSQL database can be updated
         """
 
-        with self.mock_put('/databases/postgresql/instances/123') as m:
-            new_allow_list = ['192.168.0.1/32']
+        with self.mock_put("/databases/postgresql/instances/123") as m:
+            new_allow_list = ["192.168.0.1/32"]
 
             db = PostgreSQLDatabase(self.client, 123)
 
             db.updates.day_of_week = 2
             db.allow_list = new_allow_list
-            db.label = 'cool'
+            db.label = "cool"
 
             db.save()
 
-            self.assertEqual(m.method, 'put')
-            self.assertEqual(m.call_url, '/databases/postgresql/instances/123')
-            self.assertEqual(m.call_data['label'], 'cool')
-            self.assertEqual(m.call_data['updates']['day_of_week'], 2)
-            self.assertEqual(m.call_data['allow_list'], new_allow_list)
+            self.assertEqual(m.method, "put")
+            self.assertEqual(m.call_url, "/databases/postgresql/instances/123")
+            self.assertEqual(m.call_data["label"], "cool")
+            self.assertEqual(m.call_data["updates"]["day_of_week"], 2)
+            self.assertEqual(m.call_data["allow_list"], new_allow_list)
 
     def test_list_backups(self):
         """
         Test that PostgreSQL backups list properly
         """
 
         db = PostgreSQLDatabase(self.client, 123)
         backups = db.backups
 
         self.assertEqual(len(backups), 1)
 
         self.assertEqual(backups[0].id, 456)
-        self.assertEqual(backups[0].label, 'Scheduled - 02/04/22 11:11 UTC-XcCRmI')
-        self.assertEqual(backups[0].type, 'auto')
+        self.assertEqual(
+            backups[0].label, "Scheduled - 02/04/22 11:11 UTC-XcCRmI"
+        )
+        self.assertEqual(backups[0].type, "auto")
 
     def test_create_backup(self):
         """
         Test that PostgreSQL database backups can be created
         """
 
-        with self.mock_post('/databases/postgresql/instances/123/backups') as m:
+        with self.mock_post("/databases/postgresql/instances/123/backups") as m:
             db = PostgreSQLDatabase(self.client, 123)
 
             # We don't care about errors here; we just want to
             # validate the request.
             try:
-                db.backup_create('mybackup', target='secondary')
+                db.backup_create("mybackup", target="secondary")
             except Exception:
                 pass
 
-            self.assertEqual(m.method, 'post')
-            self.assertEqual(m.call_url, '/databases/postgresql/instances/123/backups')
-            self.assertEqual(m.call_data['label'], 'mybackup')
-            self.assertEqual(m.call_data['target'], 'secondary')
+            self.assertEqual(m.method, "post")
+            self.assertEqual(
+                m.call_url, "/databases/postgresql/instances/123/backups"
+            )
+            self.assertEqual(m.call_data["label"], "mybackup")
+            self.assertEqual(m.call_data["target"], "secondary")
 
     def test_backup_restore(self):
         """
         Test that PostgreSQL database backups can be restored
         """
 
-        with self.mock_post('/databases/postgresql/instances/123/backups/456/restore') as m:
+        with self.mock_post(
+            "/databases/postgresql/instances/123/backups/456/restore"
+        ) as m:
             db = PostgreSQLDatabase(self.client, 123)
 
             db.backups[0].restore()
 
-            self.assertEqual(m.method, 'post')
-            self.assertEqual(m.call_url, '/databases/postgresql/instances/123/backups/456/restore')
+            self.assertEqual(m.method, "post")
+            self.assertEqual(
+                m.call_url,
+                "/databases/postgresql/instances/123/backups/456/restore",
+            )
 
     def test_patch(self):
         """
         Test PostgreSQL Database patching logic.
         """
-        with self.mock_post('/databases/postgresql/instances/123/patch') as m:
+        with self.mock_post("/databases/postgresql/instances/123/patch") as m:
             db = PostgreSQLDatabase(self.client, 123)
 
             db.patch()
 
-            self.assertEqual(m.method, 'post')
-            self.assertEqual(m.call_url, '/databases/postgresql/instances/123/patch')
+            self.assertEqual(m.method, "post")
+            self.assertEqual(
+                m.call_url, "/databases/postgresql/instances/123/patch"
+            )
 
     def test_get_ssl(self):
         """
         Test PostgreSQL SSL cert logic
         """
         db = PostgreSQLDatabase(self.client, 123)
 
         ssl = db.ssl
 
-        self.assertEqual(ssl.ca_certificate, 'LS0tLS1CRUdJ...==')
+        self.assertEqual(ssl.ca_certificate, "LS0tLS1CRUdJ...==")
 
     def test_get_credentials(self):
         """
         Test PostgreSQL credentials logic
         """
         db = PostgreSQLDatabase(self.client, 123)
 
         creds = db.credentials
 
-        self.assertEqual(creds.password, 's3cur3P@ssw0rd')
-        self.assertEqual(creds.username, 'linroot')
+        self.assertEqual(creds.password, "s3cur3P@ssw0rd")
+        self.assertEqual(creds.username, "linroot")
 
     def test_reset_credentials(self):
         """
         Test resetting PostgreSQL credentials
         """
-        with self.mock_post('/databases/postgresql/instances/123/credentials/reset') as m:
+        with self.mock_post(
+            "/databases/postgresql/instances/123/credentials/reset"
+        ) as m:
             db = PostgreSQLDatabase(self.client, 123)
 
             db.credentials_reset()
 
-            self.assertEqual(m.method, 'post')
-            self.assertEqual(m.call_url, '/databases/postgresql/instances/123/credentials/reset')
+            self.assertEqual(m.method, "post")
+            self.assertEqual(
+                m.call_url,
+                "/databases/postgresql/instances/123/credentials/reset",
+            )
 
 
 class MongoDBDatabaseTest(ClientBaseCase):
     """
     Tests methods of the MongoDBDatabase class
     """
 
     def test_get_instances(self):
         """
         Test that database types are properly handled
         """
         dbs = self.client.database.mongodb_instances()
 
         self.assertEqual(len(dbs), 1)
-        self.assertEqual(dbs[0].allow_list[1], '192.0.1.0/24')
+        self.assertEqual(dbs[0].allow_list[1], "192.0.1.0/24")
         self.assertEqual(dbs[0].cluster_size, 3)
-        self.assertEqual(dbs[0].compression_type, 'none')
+        self.assertEqual(dbs[0].compression_type, "none")
         self.assertEqual(dbs[0].encrypted, False)
-        self.assertEqual(dbs[0].engine, 'mongodb')
-        self.assertEqual(dbs[0].hosts.primary, 'lin-0000-0000.servers.linodedb.net')
+        self.assertEqual(dbs[0].engine, "mongodb")
+        self.assertEqual(
+            dbs[0].hosts.primary, "lin-0000-0000.servers.linodedb.net"
+        )
         self.assertEqual(dbs[0].hosts.secondary, None)
         self.assertEqual(len(dbs[0].peers), 3)
         self.assertEqual(dbs[0].id, 123)
-        self.assertEqual(dbs[0].region, 'us-east')
+        self.assertEqual(dbs[0].region, "us-east")
         self.assertEqual(dbs[0].updates.duration, 3)
-        self.assertEqual(dbs[0].version, '4.4.10')
+        self.assertEqual(dbs[0].version, "4.4.10")
 
     def test_create(self):
         """
         Test that MongoDB databases can be created
         """
 
-        with self.mock_post('/databases/mongodb/instances') as m:
+        with self.mock_post("/databases/mongodb/instances") as m:
             # We don't care about errors here; we just want to
             # validate the request.
             try:
                 self.client.database.mongodb_create(
-                    'cool',
-                    'us-southeast',
-                    'mongodb/4.4.10',
-                    'g6-standard-1',
-                    cluster_size=3
+                    "cool",
+                    "us-southeast",
+                    "mongodb/4.4.10",
+                    "g6-standard-1",
+                    cluster_size=3,
                 )
             except Exception:
                 pass
 
-            self.assertEqual(m.method, 'post')
-            self.assertEqual(m.call_url, '/databases/mongodb/instances')
-            self.assertEqual(m.call_data['label'], 'cool')
-            self.assertEqual(m.call_data['region'], 'us-southeast')
-            self.assertEqual(m.call_data['engine'], 'mongodb/4.4.10')
-            self.assertEqual(m.call_data['type'], 'g6-standard-1')
-            self.assertEqual(m.call_data['cluster_size'], 3)
+            self.assertEqual(m.method, "post")
+            self.assertEqual(m.call_url, "/databases/mongodb/instances")
+            self.assertEqual(m.call_data["label"], "cool")
+            self.assertEqual(m.call_data["region"], "us-southeast")
+            self.assertEqual(m.call_data["engine"], "mongodb/4.4.10")
+            self.assertEqual(m.call_data["type"], "g6-standard-1")
+            self.assertEqual(m.call_data["cluster_size"], 3)
 
     def test_update(self):
         """
         Test that the MongoDB database can be updated
         """
 
-        with self.mock_put('/databases/mongodb/instances/123') as m:
-            new_allow_list = ['192.168.0.1/32']
+        with self.mock_put("/databases/mongodb/instances/123") as m:
+            new_allow_list = ["192.168.0.1/32"]
 
             db = MongoDBDatabase(self.client, 123)
 
             db.updates.day_of_week = 2
             db.allow_list = new_allow_list
-            db.label = 'cool'
+            db.label = "cool"
 
             db.save()
 
-            self.assertEqual(m.method, 'put')
-            self.assertEqual(m.call_url, '/databases/mongodb/instances/123')
-            self.assertEqual(m.call_data['label'], 'cool')
-            self.assertEqual(m.call_data['updates']['day_of_week'], 2)
-            self.assertEqual(m.call_data['allow_list'], new_allow_list)
+            self.assertEqual(m.method, "put")
+            self.assertEqual(m.call_url, "/databases/mongodb/instances/123")
+            self.assertEqual(m.call_data["label"], "cool")
+            self.assertEqual(m.call_data["updates"]["day_of_week"], 2)
+            self.assertEqual(m.call_data["allow_list"], new_allow_list)
 
     def test_list_backups(self):
         """
         Test that MongoDB backups list properly
         """
 
         db = MongoDBDatabase(self.client, 123)
         backups = db.backups
 
         self.assertEqual(len(backups), 1)
 
         self.assertEqual(backups[0].id, 456)
-        self.assertEqual(backups[0].label, 'Scheduled - 02/04/22 11:11 UTC-XcCRmI')
-        self.assertEqual(backups[0].type, 'auto')
+        self.assertEqual(
+            backups[0].label, "Scheduled - 02/04/22 11:11 UTC-XcCRmI"
+        )
+        self.assertEqual(backups[0].type, "auto")
 
     def test_create_backup(self):
         """
         Test that MongoDB database backups can be created
         """
 
-        with self.mock_post('/databases/mongodb/instances/123/backups') as m:
+        with self.mock_post("/databases/mongodb/instances/123/backups") as m:
             db = MongoDBDatabase(self.client, 123)
 
             # We don't care about errors here; we just want to
             # validate the request.
             try:
-                db.backup_create('mybackup', target='secondary')
+                db.backup_create("mybackup", target="secondary")
             except Exception:
                 pass
 
-            self.assertEqual(m.method, 'post')
-            self.assertEqual(m.call_url, '/databases/mongodb/instances/123/backups')
-            self.assertEqual(m.call_data['label'], 'mybackup')
-            self.assertEqual(m.call_data['target'], 'secondary')
+            self.assertEqual(m.method, "post")
+            self.assertEqual(
+                m.call_url, "/databases/mongodb/instances/123/backups"
+            )
+            self.assertEqual(m.call_data["label"], "mybackup")
+            self.assertEqual(m.call_data["target"], "secondary")
 
     def test_backup_restore(self):
         """
         Test that MongoDB database backups can be restored
         """
 
-        with self.mock_post('/databases/mongodb/instances/123/backups/456/restore') as m:
+        with self.mock_post(
+            "/databases/mongodb/instances/123/backups/456/restore"
+        ) as m:
             db = MongoDBDatabase(self.client, 123)
 
             db.backups[0].restore()
 
-            self.assertEqual(m.method, 'post')
-            self.assertEqual(m.call_url, '/databases/mongodb/instances/123/backups/456/restore')
+            self.assertEqual(m.method, "post")
+            self.assertEqual(
+                m.call_url,
+                "/databases/mongodb/instances/123/backups/456/restore",
+            )
 
     def test_patch(self):
         """
         Test MongoDB Database patching logic.
         """
-        with self.mock_post('/databases/mongodb/instances/123/patch') as m:
+        with self.mock_post("/databases/mongodb/instances/123/patch") as m:
             db = MongoDBDatabase(self.client, 123)
 
             db.patch()
 
-            self.assertEqual(m.method, 'post')
-            self.assertEqual(m.call_url, '/databases/mongodb/instances/123/patch')
+            self.assertEqual(m.method, "post")
+            self.assertEqual(
+                m.call_url, "/databases/mongodb/instances/123/patch"
+            )
 
     def test_get_ssl(self):
         """
         Test MongoDB SSL cert logic
         """
         db = MongoDBDatabase(self.client, 123)
 
         ssl = db.ssl
 
-        self.assertEqual(ssl.ca_certificate, 'LS0tLS1CRUdJ...==')
+        self.assertEqual(ssl.ca_certificate, "LS0tLS1CRUdJ...==")
 
     def test_get_credentials(self):
         """
         Test MongoDB credentials logic
         """
         db = MongoDBDatabase(self.client, 123)
 
         creds = db.credentials
 
-        self.assertEqual(creds.password, 's3cur3P@ssw0rd')
-        self.assertEqual(creds.username, 'linroot')
+        self.assertEqual(creds.password, "s3cur3P@ssw0rd")
+        self.assertEqual(creds.username, "linroot")
 
     def test_reset_credentials(self):
         """
         Test resetting MongoDB credentials
         """
-        with self.mock_post('/databases/mongodb/instances/123/credentials/reset') as m:
+        with self.mock_post(
+            "/databases/mongodb/instances/123/credentials/reset"
+        ) as m:
             db = MongoDBDatabase(self.client, 123)
 
             db.credentials_reset()
 
-            self.assertEqual(m.method, 'post')
-            self.assertEqual(m.call_url, '/databases/mongodb/instances/123/credentials/reset')
+            self.assertEqual(m.method, "post")
+            self.assertEqual(
+                m.call_url, "/databases/mongodb/instances/123/credentials/reset"
+            )
```

### Comparing `linode_api4-5.3.0/test/objects/firewall_test.py` & `linode_api4-5.4.0/test/objects/firewall_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,69 @@
 from test.base import ClientBaseCase
 
 from linode_api4.objects import Firewall, FirewallDevice
 
+
 class FirewallTest(ClientBaseCase):
     """
     Tests methods of the Firewall class
     """
+
     def test_get_rules(self):
         """
         Test that the rules can be retrieved from a Firewall
         """
         firewall = Firewall(self.client, 123)
         rules = firewall.rules
 
         self.assertEqual(len(rules.inbound), 0)
-        self.assertEqual(rules.inbound_policy, 'DROP')
+        self.assertEqual(rules.inbound_policy, "DROP")
         self.assertEqual(len(rules.outbound), 0)
-        self.assertEqual(rules.outbound_policy, 'DROP')
+        self.assertEqual(rules.outbound_policy, "DROP")
 
     def test_update_rules(self):
         """
         Test that the rules can be updated for a Firewall
         """
 
         firewall = Firewall(self.client, 123)
 
-        with self.mock_put('networking/firewalls/123/rules') as m:
+        with self.mock_put("networking/firewalls/123/rules") as m:
             new_rules = {
-                'inbound': [
+                "inbound": [
                     {
-                        'action': 'ACCEPT',
-                        'addresses': {
-                            'ipv4': [
-                                '0.0.0.0/0'
-                            ],
-                            'ipv6': [
-                                "ff00::/8"
-                            ]
+                        "action": "ACCEPT",
+                        "addresses": {
+                            "ipv4": ["0.0.0.0/0"],
+                            "ipv6": ["ff00::/8"],
                         },
-                        'description': 'A really cool firewall rule.',
-                        'label': 'really-cool-firewall-rule',
-                        'ports': '80',
-                        'protocol': 'TCP'
+                        "description": "A really cool firewall rule.",
+                        "label": "really-cool-firewall-rule",
+                        "ports": "80",
+                        "protocol": "TCP",
                     }
                 ],
-                'inbound_policy': 'ALLOW',
-                'outbound': [],
-                'outbound_policy': 'ALLOW'
+                "inbound_policy": "ALLOW",
+                "outbound": [],
+                "outbound_policy": "ALLOW",
             }
 
             firewall.update_rules(new_rules)
 
-            self.assertEqual(m.method, 'put')
-            self.assertEqual(m.call_url, '/networking/firewalls/123/rules')
+            self.assertEqual(m.method, "put")
+            self.assertEqual(m.call_url, "/networking/firewalls/123/rules")
 
             self.assertEqual(m.call_data, new_rules)
 
 
 class FirewallDevicesTest(ClientBaseCase):
     """
     Tests methods of Firewall devices
     """
+
     def test_get_devices(self):
         """
         Tests that devices can be pulled from a firewall
         """
         firewall = Firewall(self.client, 123)
         self.assertEqual(len(firewall.devices), 1)
 
@@ -73,12 +72,12 @@
         Tests that a device is loaded correctly by ID
         """
         device = FirewallDevice(self.client, 123, 123)
         self.assertEqual(device._populated, False)
 
         self.assertEqual(device.id, 123)
         self.assertEqual(device.entity.id, 123)
-        self.assertEqual(device.entity.label, 'my-linode')
-        self.assertEqual(device.entity.type, 'linode')
-        self.assertEqual(device.entity.url, '/v4/linode/instances/123')
+        self.assertEqual(device.entity.label, "my-linode")
+        self.assertEqual(device.entity.type, "linode")
+        self.assertEqual(device.entity.url, "/v4/linode/instances/123")
 
         self.assertEqual(device._populated, True)
```

### Comparing `linode_api4-5.3.0/test/objects/longview_test.py` & `linode_api4-5.4.0/test/objects/longview_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,99 @@
 from datetime import datetime
 from test.base import ClientBaseCase
 
-from linode_api4.objects import LongviewClient, LongviewSubscription
+from linode_api4.objects import (
+    LongviewClient,
+    LongviewPlan,
+    LongviewSubscription,
+)
 from linode_api4.objects.base import MappedObject
 
 
+class LongviewPlanTest(ClientBaseCase):
+    """
+    Tests methods of the LongviewPlan class
+    """
+
+    def test_get_plan(self):
+        """
+        Tests that a plan is loaded correctly
+        """
+        plan = LongviewPlan(self.client, "longview-10")
+
+        self.assertEqual(plan.id, "longview-10")
+        self.assertEqual(plan.clients_included, 10)
+        self.assertEqual(plan.label, "Longview Pro 10 pack")
+        self.assertIsNotNone(plan.price)
+
+
 class LongviewClientTest(ClientBaseCase):
     """
     Tests methods of the LongviewClient class
     """
+
     def test_get_client(self):
         """
         Tests that a client is loaded correctly by ID
         """
         client = LongviewClient(self.client, 1234)
         self.assertEqual(client._populated, False)
 
-        self.assertEqual(client.label, 'test_client_1')
+        self.assertEqual(client.label, "test_client_1")
         self.assertEqual(client._populated, True)
 
         self.assertIsInstance(client.created, datetime)
         self.assertIsInstance(client.updated, datetime)
 
         self.assertIsInstance(client.apps, MappedObject)
         self.assertFalse(client.apps.nginx)
         self.assertFalse(client.apps.mysql)
         self.assertFalse(client.apps.apache)
 
-        self.assertEqual(client.install_code, '12345678-ABCD-EF01-23456789ABCDEF12')
-        self.assertEqual(client.api_key, '12345678-ABCD-EF01-23456789ABCDEF12')
+        self.assertEqual(
+            client.install_code, "12345678-ABCD-EF01-23456789ABCDEF12"
+        )
+        self.assertEqual(client.api_key, "12345678-ABCD-EF01-23456789ABCDEF12")
 
     def test_update_label(self):
         """
         Tests that updating a client's label contacts the api correctly.
         """
-        with self.mock_put('longview/clients/1234') as m:
+        with self.mock_put("longview/clients/1234") as m:
             client = LongviewClient(self.client, 1234)
             client.label = "updated"
             client.save()
 
-            self.assertEqual(m.call_url, '/longview/clients/1234')
-            self.assertEqual(m.call_data, {
-                "label": "updated"
-            })
+            self.assertEqual(m.call_url, "/longview/clients/1234")
+            self.assertEqual(m.call_data, {"label": "updated"})
 
     def test_delete_client(self):
         """
         Tests that deleting a client creates the correct api request.
         """
         with self.mock_delete() as m:
             client = LongviewClient(self.client, 1234)
             client.delete()
 
-            self.assertEqual(m.call_url, '/longview/clients/1234')
+            self.assertEqual(m.call_url, "/longview/clients/1234")
 
 
 class LongviewSubscriptionTest(ClientBaseCase):
     """
     Tests methods of the LongviewSubscription class
     """
+
     def test_get_subscription(self):
         """
         Tests that a subscription is loaded correctly by ID
         """
         sub = LongviewSubscription(self.client, "longview-40")
         self.assertEqual(sub._populated, False)
 
-        self.assertEqual(sub.label, 'Longview Pro 40 pack')
+        self.assertEqual(sub.label, "Longview Pro 40 pack")
         self.assertEqual(sub._populated, True)
 
         self.assertEqual(sub.clients_included, 40)
 
         self.assertIsInstance(sub.price, MappedObject)
-        self.assertEqual(sub.price.hourly, .15)
+        self.assertEqual(sub.price.hourly, 0.15)
         self.assertEqual(sub.price.monthly, 100)
```

### Comparing `linode_api4-5.3.0/test/objects/nodebalancers_test.py` & `linode_api4-5.4.0/test/objects/nodebalancers_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from datetime import datetime
 from test.base import ClientBaseCase
 
 from linode_api4.objects import NodeBalancerConfig, NodeBalancerNode
 from linode_api4.objects.base import MappedObject
 
 
 class NodeBalancerConfigTest(ClientBaseCase):
     """
     Tests methods of the NodeBalancerConfig class
     """
+
     def test_get_config(self):
         """
         Tests that a config is loaded correctly by ID
         """
         config = NodeBalancerConfig(self.client, 65432, 123456)
         self.assertEqual(config._populated, False)
 
@@ -40,14 +40,15 @@
         self.assertEqual(config.proxy_protocol, "none")
 
 
 class NodeBalancerNodeTest(ClientBaseCase):
     """
     Tests methods of the NodeBalancerNode class
     """
+
     def test_get_node(self):
         """
         Tests that a node is loaded correctly by ID
         """
         node = NodeBalancerNode(self.client, 54321, (65432, 123456))
         self.assertEqual(node._populated, False)
 
@@ -62,51 +63,68 @@
         self.assertEqual(node.config_id, 65432)
         self.assertEqual(node.nodebalancer_id, 123456)
 
     def test_create_node(self):
         """
         Tests that a node can be created
         """
-        with self.mock_post('nodebalancers/123456/configs/65432/nodes/54321') as m:
+        with self.mock_post(
+            "nodebalancers/123456/configs/65432/nodes/54321"
+        ) as m:
             config = NodeBalancerConfig(self.client, 65432, 123456)
-            node = config.node_create('node54321', '192.168.210.120',
-                weight=50, mode='accept')
+            node = config.node_create(
+                "node54321", "192.168.210.120", weight=50, mode="accept"
+            )
 
             self.assertIsNotNone(node)
             self.assertEqual(node.id, 54321)
-            self.assertEqual(m.call_url, '/nodebalancers/123456/configs/65432/nodes')
-            self.assertEqual(m.call_data, {
-                "label": "node54321",
-                "address": "192.168.210.120",
-                "weight": 50,
-                "mode": "accept"
-            })
+            self.assertEqual(
+                m.call_url, "/nodebalancers/123456/configs/65432/nodes"
+            )
+            self.assertEqual(
+                m.call_data,
+                {
+                    "label": "node54321",
+                    "address": "192.168.210.120",
+                    "weight": 50,
+                    "mode": "accept",
+                },
+            )
 
     def test_update_node(self):
         """
         Tests that a node can be updated
         """
-        with self.mock_put('nodebalancers/123456/configs/65432/nodes/54321') as m:
+        with self.mock_put(
+            "nodebalancers/123456/configs/65432/nodes/54321"
+        ) as m:
             node = self.client.load(NodeBalancerNode, 54321, (65432, 123456))
             node.label = "ThisNewLabel"
             node.weight = 60
             node.mode = "drain"
             node.address = "192.168.210.121"
             node.save()
 
-            self.assertEqual(m.call_url, '/nodebalancers/123456/configs/65432/nodes/54321')
-            self.assertEqual(m.call_data, {
-                "label": "ThisNewLabel",
-                "address": "192.168.210.121",
-                "mode": "drain",
-                "weight": 60
-            })
+            self.assertEqual(
+                m.call_url, "/nodebalancers/123456/configs/65432/nodes/54321"
+            )
+            self.assertEqual(
+                m.call_data,
+                {
+                    "label": "ThisNewLabel",
+                    "address": "192.168.210.121",
+                    "mode": "drain",
+                    "weight": 60,
+                },
+            )
 
     def test_delete_node(self):
         """
         Tests that deleting a node creates the correct api request.
         """
         with self.mock_delete() as m:
             node = NodeBalancerNode(self.client, 54321, (65432, 123456))
             node.delete()
 
-            self.assertEqual(m.call_url, '/nodebalancers/123456/configs/65432/nodes/54321')
+            self.assertEqual(
+                m.call_url, "/nodebalancers/123456/configs/65432/nodes/54321"
+            )
```

### Comparing `linode_api4-5.3.0/test/objects/tag_test.py` & `linode_api4-5.4.0/test/objects/tag_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from datetime import datetime
 from test.base import ClientBaseCase
 
 from linode_api4.objects import Instance, Tag
 
 
 class TagTest(ClientBaseCase):
     """
     Tests methods of the Tag class
     """
+
     def test_get_tag(self):
         """
         Tests that Tag is loaded correctly by label
         """
-        tag = Tag(self.client, 'something')
+        tag = Tag(self.client, "something")
 
         self.assertEqual(tag.label, "something")
-        self.assertFalse(hasattr(tag, '_raw_objects'))
+        self.assertFalse(hasattr(tag, "_raw_objects"))
 
     def test_load_tag(self):
         """
         Tests that the LinodeClient can load a tag
         """
-        tag = self.client.load(Tag, 'something')
+        tag = self.client.load(Tag, "something")
 
-        self.assertEqual(tag.label, 'something')
-        self.assertTrue(hasattr(tag, '_raw_objects')) # got the raw objects
+        self.assertEqual(tag.label, "something")
+        self.assertTrue(hasattr(tag, "_raw_objects"))  # got the raw objects
         print(tag._raw_objects)
 
         # objects loaded up right
         self.assertEqual(len(tag.objects), 1)
         self.assertEqual(tag.objects[0].id, 123)
-        self.assertEqual(tag.objects[0].label, 'linode123')
-        self.assertEqual(tag.objects[0].tags, ['something'])
+        self.assertEqual(tag.objects[0].label, "linode123")
+        self.assertEqual(tag.objects[0].tags, ["something"])
 
     def test_delete_tag(self):
         """
         Tests that you can delete a tag
         """
         with self.mock_delete() as m:
-            tag = Tag(self.client, 'nothing')
+            tag = Tag(self.client, "nothing")
             result = tag.delete()
 
             self.assertEqual(result, True)
 
-            self.assertEqual(m.call_url, '/tags/nothing')
+            self.assertEqual(m.call_url, "/tags/nothing")
```

### Comparing `linode_api4-5.3.0/test/objects/volume_test.py` & `linode_api4-5.4.0/test/objects/volume_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,77 +12,85 @@
     def test_get_volume(self):
         """
         Tests that a volume is loaded correctly by ID
         """
         volume = Volume(self.client, 1)
         self.assertEqual(volume._populated, False)
 
-        self.assertEqual(volume.label, 'block1')
+        self.assertEqual(volume.label, "block1")
         self.assertEqual(volume._populated, True)
 
         self.assertEqual(volume.size, 40)
         self.assertEqual(volume.linode, None)
-        self.assertEqual(volume.status, 'active')
+        self.assertEqual(volume.status, "active")
         self.assertIsInstance(volume.updated, datetime)
-        self.assertEqual(volume.region.id, 'us-east-1a')
+        self.assertEqual(volume.region.id, "us-east-1a")
 
         assert volume.tags == ["something"]
 
+        self.assertEqual(volume.filesystem_path, "this/is/a/file/path")
+        self.assertEqual(volume.hardware_type, "hdd")
+        self.assertEqual(volume.linode_label, None)
+
     def test_update_volume_tags(self):
         """
         Tests that updating tags on an entity send the correct request
         """
         volume = self.client.volumes().first()
 
-        with self.mock_put('volumes/1') as m:
-            volume.tags = ['test1', 'test2']
+        with self.mock_put("volumes/1") as m:
+            volume.tags = ["test1", "test2"]
             volume.save()
 
-            assert m.call_url == '/volumes/{}'.format(volume.id)
-            assert m.call_data['tags'] == ['test1', 'test2']
+            assert m.call_url == "/volumes/{}".format(volume.id)
+            assert m.call_data["tags"] == ["test1", "test2"]
 
     def test_clone_volume(self):
         """
         Tests that cloning a volume returns new volume object with
         same region and the given label
         """
         volume_to_clone = self.client.volumes().first()
 
-        with self.mock_post(f'volumes/{volume_to_clone.id}') as mock:
-            new_volume = volume_to_clone.clone('new-volume')
-            assert mock.call_url == f'/volumes/{volume_to_clone.id}/clone'
-            self.assertEqual(str(new_volume.region), str(volume_to_clone.region), 'the regions should be the same')
+        with self.mock_post(f"volumes/{volume_to_clone.id}") as mock:
+            new_volume = volume_to_clone.clone("new-volume")
+            assert mock.call_url == f"/volumes/{volume_to_clone.id}/clone"
+            self.assertEqual(
+                str(new_volume.region),
+                str(volume_to_clone.region),
+                "the regions should be the same",
+            )
             assert new_volume.id != str(volume_to_clone.id)
 
     def test_resize_volume(self):
         """
         Tests that resizing a given volume volume works
         """
         volume = self.client.volumes().first()
 
-        with self.mock_post(f'volumes/{volume.id}') as mock:
+        with self.mock_post(f"volumes/{volume.id}") as mock:
             volume.resize(3048)
-            assert mock.call_url == f'/volumes/{volume.id}/resize'
-            assert str(mock.call_data['size']) == '3048'
+            assert mock.call_url == f"/volumes/{volume.id}/resize"
+            assert str(mock.call_data["size"]) == "3048"
 
     def test_detach_volume(self):
         """
         Tests that detaching the volume succeeds
         """
         volume = self.client.volumes()[2]
 
-        with self.mock_post(f'volumes/{volume.id}') as mock:
+        with self.mock_post(f"volumes/{volume.id}") as mock:
             result = volume.detach()
-            assert mock.call_url == f'/volumes/{volume.id}/detach'
+            assert mock.call_url == f"/volumes/{volume.id}/detach"
             assert result is True
 
     def test_attach_volume_to_linode(self):
         """
         Tests that the given volume attaches to the Linode via id
         """
         volume = self.client.volumes().first()
 
-        with self.mock_post(f'volumes/{volume.id}') as mock:
+        with self.mock_post(f"volumes/{volume.id}") as mock:
             result = volume.attach(1)
-            assert mock.call_url == f'/volumes/{volume.id}/attach'
+            assert mock.call_url == f"/volumes/{volume.id}/attach"
             assert result is True
-            assert str(mock.call_data['linode_id']) == '1'
+            assert str(mock.call_data["linode_id"]) == "1"
```

### Comparing `linode_api4-5.3.0/test/paginated_list_test.py` & `linode_api4-5.4.0/test/paginated_list_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,36 +6,39 @@
 
 class PaginationSlicingTest(TestCase):
     def setUp(self):
         """
         Creates sample mocked lists for use in the test cases
         """
         self.normal_list = list(range(25))
-        self.paginated_list = PaginatedList(None, None, page=self.normal_list,
-                total_items=25)
+        self.paginated_list = PaginatedList(
+            None, None, page=self.normal_list, total_items=25
+        )
 
     def test_slice_normal(self):
         """
         Tests that bounded, forward slices work as expected
         """
-        slices = ( (1, 10), (10, 20), (5, 25), (0, 10) )
+        slices = ((1, 10), (10, 20), (5, 25), (0, 10))
 
-        for (start, stop) in slices:
-            self.assertEqual(self.normal_list[start:stop],
-                    self.paginated_list[start:stop])
+        for start, stop in slices:
+            self.assertEqual(
+                self.normal_list[start:stop], self.paginated_list[start:stop]
+            )
 
     def test_slice_negative(self):
         """
         Tests that negative indexing works in slices
         """
-        slices = ( (-10,-5), (-20, 20), (3, -10) )
+        slices = ((-10, -5), (-20, 20), (3, -10))
 
-        for (start, stop) in slices:
-            self.assertEqual(self.normal_list[start:stop],
-                    self.paginated_list[start:stop])
+        for start, stop in slices:
+            self.assertEqual(
+                self.normal_list[start:stop], self.paginated_list[start:stop]
+            )
 
     def test_slice_no_lower_bound(self):
         """
         Tests that slices without lower bounds work
         """
         self.assertEqual(self.normal_list[:5], self.paginated_list[:5])
 
@@ -64,65 +67,70 @@
         """
         self.assertEqual(self.normal_list[30:], self.paginated_list[30:])
 
     def test_slice_unsupported_step(self):
         """
         Tests that steps outside of 1 raise a NotImplementedError
         """
-        for step in ( -1, 0, 2, 3 ):
+        for step in (-1, 0, 2, 3):
             with self.assertRaises(NotImplementedError):
                 self.paginated_list[::step]
 
     def test_slice_backward_indexing(self):
         """
         Tests that backwards indexing works as expected
         """
         self.assertEqual(self.normal_list[10:5], self.paginated_list[10:5])
 
 
-class TestModel():
+class TestModel:
     """
     This is a test model class used to simulate an actual model that would be
     returned by the API
     """
+
     @classmethod
     def make_instance(*args, **kwargs):
         return TestModel()
 
 
 class PageLoadingTest(TestCase):
     def test_page_size_in_request(self):
         """
         Tests that the correct page_size is added to requests when loading subsequent pages
         """
 
         for i in (25, 100, 500):
             # these are the pages we're sending in to the mocked list
-            first_page = [ TestModel()  for x in range(i) ]
+            first_page = [TestModel() for x in range(i)]
             second_page = {
                 "data": [{"id": 1}],
                 "pages": 2,
                 "page": 2,
                 "results": i + 1,
             }
 
             # our mock client to intercept the requests and return the mocked info
             client = MagicMock()
             client.get = MagicMock(return_value=second_page)
 
             # let's do it!
-            p = PaginatedList(client, "/test", page=first_page, max_pages=2, total_items=i+1)
-            p[i] # load second page
+            p = PaginatedList(
+                client, "/test", page=first_page, max_pages=2, total_items=i + 1
+            )
+            p[i]  # load second page
 
             # and we called the next page URL with the correct page_size
-            assert client.get.call_args == call("//test?page=2&page_size={}".format(i), filters=None)
+            assert client.get.call_args == call(
+                "//test?page=2&page_size={}".format(i), filters=None
+            )
 
     def test_no_pages(self):
         """
         Tests that this library correctly handles paginated lists with no data, such
         as if a paginated endpoint is given a filter that matches nothing.
         """
         client = MagicMock()
 
         p = PaginatedList(client, "/test", page=[], max_pages=0, total_items=0)
 
-        assert(len(p) == 0)
+        assert len(p) == 0
```

