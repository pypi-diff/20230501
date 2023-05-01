# Comparing `tmp/duo_client-4.7.1.tar.gz` & `tmp/duo_client-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duo_client-4.7.1.tar", last modified: Wed Apr  5 19:05:03 2023, max compression
+gzip compressed data, was "duo_client-5.0.0.tar", last modified: Mon May  1 19:09:58 2023, max compression
```

## Comparing `duo_client-4.7.1.tar` & `duo_client-5.0.0.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:05:03.020024 duo_client-4.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-05 19:04:51.000000 duo_client-4.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-05 19:04:51.000000 duo_client-4.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-05 19:05:03.020024 duo_client-4.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-05 19:04:51.000000 duo_client-4.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-05 19:04:51.000000 duo_client-4.7.1/apache-license-2.0.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:05:03.016024 duo_client-4.7.1/duo_client/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-05 19:04:51.000000 duo_client-4.7.1/duo_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-05 19:04:51.000000 duo_client-4.7.1/duo_client/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)   119340 2023-04-05 19:04:51.000000 duo_client-4.7.1/duo_client/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-05 19:04:51.000000 duo_client-4.7.1/duo_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-05 19:04:51.000000 duo_client-4.7.1/duo_client/auth_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-04-05 19:04:51.000000 duo_client-4.7.1/duo_client/ca_certs.pem
--rw-r--r--   0 runner    (1001) docker     (123)    24101 2023-04-05 19:04:51.000000 duo_client-4.7.1/duo_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-04-05 19:04:51.000000 duo_client-4.7.1/duo_client/https_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:05:03.016024 duo_client-4.7.1/duo_client/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-05 19:04:51.000000 duo_client-4.7.1/duo_client/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-05 19:04:51.000000 duo_client-4.7.1/duo_client/logs/telephony.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-05 19:04:51.000000 duo_client-4.7.1/duo_client/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:05:03.016024 duo_client-4.7.1/duo_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-05 19:05:02.000000 duo_client-4.7.1/duo_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-05 19:05:02.000000 duo_client-4.7.1/duo_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 19:05:02.000000 duo_client-4.7.1/duo_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-05 19:05:02.000000 duo_client-4.7.1/duo_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-05 19:05:02.000000 duo_client-4.7.1/duo_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:05:03.020024 duo_client-4.7.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-05 19:04:51.000000 duo_client-4.7.1/examples/create_integration_sso_generic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1857 2023-04-05 19:04:51.000000 duo_client-4.7.1/examples/create_user_and_phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-05 19:04:51.000000 duo_client-4.7.1/examples/get_billing_and_telephony_credits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-05 19:04:51.000000 duo_client-4.7.1/examples/log_examples.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1176 2023-04-05 19:04:51.000000 duo_client-4.7.1/examples/report_auths_by_country.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1203 2023-04-05 19:04:51.000000 duo_client-4.7.1/examples/report_users_and_phones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:05:03.020024 duo_client-4.7.1/examples/splunk/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-05 19:04:51.000000 duo_client-4.7.1/examples/splunk/duo.conf
--rwxr-xr-x   0 runner    (1001) docker     (123)     7179 2023-04-05 19:04:51.000000 duo_client-4.7.1/examples/splunk/splunk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1371 2023-04-05 19:04:51.000000 duo_client-4.7.1/examples/trust_monitor_events.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-05 19:04:51.000000 duo_client-4.7.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-05 19:04:51.000000 duo_client-4.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-05 19:05:03.020024 duo_client-4.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-05 19:04:51.000000 duo_client-4.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:05:03.020024 duo_client-4.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 19:05:03.020024 duo_client-4.7.1/tests/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_administrative_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_authlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_bypass_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_desktop_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_phones.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_telephony.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_trust_monitor_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_u2f.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_user_bypass_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_user_phones.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_user_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_user_u2f.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_user_webauthn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/admin/test_webauthn.py
--rw-r--r--   0 runner    (1001) docker     (123)    30728 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/test_https_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-04-05 19:04:51.000000 duo_client-4.7.1/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.275415 duo_client-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-01 19:09:41.000000 duo_client-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-01 19:09:41.000000 duo_client-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-01 19:09:58.275415 duo_client-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-01 19:09:41.000000 duo_client-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-01 19:09:41.000000 duo_client-5.0.0/apache-license-2.0.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.267415 duo_client-5.0.0/duo_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122004 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/auth_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/ca_certs.pem
+-rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/https_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.271415 duo_client-5.0.0/duo_client/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/logs/telephony.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-01 19:09:41.000000 duo_client-5.0.0/duo_client/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.271415 duo_client-5.0.0/duo_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-01 19:09:58.000000 duo_client-5.0.0/duo_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-01 19:09:58.000000 duo_client-5.0.0/duo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:09:58.000000 duo_client-5.0.0/duo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 19:09:58.000000 duo_client-5.0.0/duo_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 19:09:58.000000 duo_client-5.0.0/duo_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.271415 duo_client-5.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/create_integration_sso_generic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1857 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/create_user_and_phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/get_billing_and_telephony_credits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/log_examples.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3856 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/policies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1176 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/report_auths_by_country.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1203 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/report_users_and_phones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.271415 duo_client-5.0.0/examples/splunk/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/splunk/duo.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7179 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/splunk/splunk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1371 2023-05-01 19:09:41.000000 duo_client-5.0.0/examples/trust_monitor_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-01 19:09:41.000000 duo_client-5.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 19:09:41.000000 duo_client-5.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 19:09:58.275415 duo_client-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-01 19:09:41.000000 duo_client-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.271415 duo_client-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:58.275415 duo_client-5.0.0/tests/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_administrative_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_authlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_bypass_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_desktop_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_phones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_telephony.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_trust_monitor_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_u2f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_user_bypass_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_user_phones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_user_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_user_u2f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_user_webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/admin/test_webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32499 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/test_https_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-05-01 19:09:41.000000 duo_client-5.0.0/tests/util.py
```

### Comparing `duo_client-4.7.1/LICENSE` & `duo_client-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/PKG-INFO` & `duo_client-5.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duo_client
-Version: 4.7.1
+Version: 5.0.0
 Summary: Reference client for Duo Security APIs
 Home-page: https://github.com/duosecurity/duo_client_python
 Author: Duo Security, Inc.
 Author-email: support@duosecurity.com
 License: BSD
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -31,17 +31,20 @@
 ## Tested Against Python Versions
 * 3.7
 * 3.8
 * 3.9
 * 3.10
 * 3.11
 
+## Requirements
+Duo_client_python supports Python 3.7 and higher
+
 ## TLS 1.2 and 1.3 Support
 
-Duo_client_python uses Python's ssl module and OpenSSL for TLS operations.  Python versions 2.7 (and higher) and 3.5 (and higher) have both TLS 1.2 and TLS 1.3 support.
+Duo_client_python uses Python's ssl module and OpenSSL for TLS operations.  Python versions 3.7 (and higher) have both TLS 1.2 and TLS 1.3 support.
 
 # Installing
 
 Development:
 
 ```
 $ git clone https://github.com/duosecurity/duo_client_python.git
```

### Comparing `duo_client-4.7.1/README.md` & `duo_client-5.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,20 @@
 ## Tested Against Python Versions
 * 3.7
 * 3.8
 * 3.9
 * 3.10
 * 3.11
 
+## Requirements
+Duo_client_python supports Python 3.7 and higher
+
 ## TLS 1.2 and 1.3 Support
 
-Duo_client_python uses Python's ssl module and OpenSSL for TLS operations.  Python versions 2.7 (and higher) and 3.5 (and higher) have both TLS 1.2 and TLS 1.3 support.
+Duo_client_python uses Python's ssl module and OpenSSL for TLS operations.  Python versions 3.7 (and higher) have both TLS 1.2 and TLS 1.3 support.
 
 # Installing
 
 Development:
 
 ```
 $ git clone https://github.com/duosecurity/duo_client_python.git
```

### Comparing `duo_client-4.7.1/apache-license-2.0.txt` & `duo_client-5.0.0/apache-license-2.0.txt`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/duo_client/accounts.py` & `duo_client-5.0.0/duo_client/accounts.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/duo_client/admin.py` & `duo_client-5.0.0/duo_client/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -3262,14 +3262,96 @@
 
         return self.json_api_call(
             "GET",
             "/admin/v1/trust_monitor/events",
             params,
         )
 
+    def _quote_policy_id(self, policy_key):
+        return six.moves.urllib.parse.quote_plus("{}".format(policy_key))
+
+    def get_policies_v2_iterator(self):
+        """
+        Obtain an iterator for retrieving all the policies. The order isn't defined.
+        Returns: Iterator of dict elements. Each element contains the policy content.
+        """
+
+        return self.json_paging_api_call(
+            "GET",
+            "/admin/v2/policies",
+            {},
+        )
+
+    def get_policies_v2(self, limit=None, offset=0):
+        """
+        Retrieves a list of policies. The order isn't defined.
+        Args:
+            limit (int, optional): The max number of policies to fetch at once.
+            offset (int, optional): If a limit is passed, the offset to start retrieval.
+                Default 0
+        Raises RuntimeError on error.
+        """
+
+        (limit, offset) = self.normalize_paging_args(limit, offset)
+        if limit:
+            return self.json_api_call(
+                "GET",
+                "/admin/v2/policies",
+                {"limit": limit, "offset": offset},
+            )
+        return list(self.get_policies_v2_iterator())
+
+    def delete_policy_v2(self, policy_key):
+        """
+        Deletes a policy.
+        Params:
+            policy_key (str) - Unique id of the policy
+        Notes:
+            Raises RuntimeError on error.
+        """
+
+        path = "/admin/v2/policies/" + self._quote_policy_id(policy_key)
+        return self.json_api_call("DELETE", path, {})
+
+    def update_policy_v2(self, policy_key, json_request):
+        """
+        Update the content of a single policy
+        Args:
+            policy_key (str) - Unique id of the policy
+            json_request (dict) - policy content to update.
+        Returns (dict) - policy after updates have been made.
+        """
+
+        path = "/admin/v2/policies/" + self._quote_policy_id(policy_key)
+        response = self.json_api_call("PUT", path, json_request)
+        return response
+
+    def create_policy_v2(self, json_request):
+        """
+        Args:
+            json_request (dict) - policy content to create.
+        Returns (dict) - newly created policy
+        """
+
+        path = "/admin/v2/policies"
+        response = self.json_api_call("POST", path, json_request)
+        return response
+
+    def get_policy_v2(self, policy_key):
+        """
+        Args:
+            policy_key: policy_key (str) - Unique id of the policy
+        Returns (dict) - policy content
+        """
+
+        path = "/admin/v2/policies/" + self._quote_policy_id(policy_key)
+        response = self.json_api_call("GET", path, {})
+        return response
+
+
 class AccountAdmin(Admin):
     """AccountAdmin manages a child account using an Accounts API integration."""
 
     def __init__(self, account_id, **kwargs):
         """Initializes an AccountAdmin for administering a child account.
            account_id is the account id of the child account.
            See the Client base class for other parameters."""
```

### Comparing `duo_client-4.7.1/duo_client/auth.py` & `duo_client-5.0.0/duo_client/auth.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/duo_client/auth_v1.py` & `duo_client-5.0.0/duo_client/auth_v1.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/duo_client/ca_certs.pem` & `duo_client-5.0.0/duo_client/ca_certs.pem`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/duo_client/client.py` & `duo_client-5.0.0/duo_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Low level functions for generating Duo Web API calls and parsing results.
 """
 from __future__ import absolute_import
 from __future__ import print_function
 import six
 
-__version__ = '4.7.1'
+__version__ = '5.0.0'
 
 import base64
 import collections
 import datetime
 import email.utils
 import hashlib
 import hmac
@@ -579,15 +579,20 @@
                     response.status,
                     response.reason,
             ))
         try:
             data = json.loads(data)
             if data['stat'] != 'OK':
                 raise_error('Received error response: %s' % data)
-            return (data['response'], data.get('metadata', {}))
+            response = data['response']
+            metadata = data.get('metadata', {})
+            if not metadata and not isinstance(response, list):
+                metadata = response.get('metadata', {})
+
+            return (response, metadata)
         except (ValueError, KeyError, TypeError):
             raise_error('Received bad response: %s' % data)
 
     @classmethod
     def canon_json(cls, params):
         if not isinstance(params, dict):
             raise ValueError('JSON request must be an object.')
```

### Comparing `duo_client-4.7.1/duo_client/https_wrapper.py` & `duo_client-5.0.0/duo_client/https_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,16 @@
 
     def connect(self):
         "Connect to a host on a given (SSL) port."
         self.sock = socket.create_connection((self.host, self.port),
                                              self.timeout)
         if self._tunnel_host:
             self._tunnel()
-        self.sock = self.default_ssl_context.wrap_socket(self.sock)
+        self.sock = self.default_ssl_context.wrap_socket(self.sock,
+                                                         server_hostname=self.host)
         if self.default_ssl_context.verify_mode == ssl.CERT_REQUIRED:
             cert = self.sock.getpeercert()
             cert_validation_host = self._tunnel_host or self.host
             hostname = cert_validation_host.split(':', 0)[0]
             if not self._ValidateCertificateHostname(cert, hostname):
                 raise InvalidCertificateException(hostname, cert, 'hostname mismatch')
```

### Comparing `duo_client-4.7.1/duo_client/logs/telephony.py` & `duo_client-5.0.0/duo_client/logs/telephony.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/duo_client/util.py` & `duo_client-5.0.0/duo_client/util.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/duo_client.egg-info/PKG-INFO` & `duo_client-5.0.0/duo_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duo-client
-Version: 4.7.1
+Version: 5.0.0
 Summary: Reference client for Duo Security APIs
 Home-page: https://github.com/duosecurity/duo_client_python
 Author: Duo Security, Inc.
 Author-email: support@duosecurity.com
 License: BSD
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -31,17 +31,20 @@
 ## Tested Against Python Versions
 * 3.7
 * 3.8
 * 3.9
 * 3.10
 * 3.11
 
+## Requirements
+Duo_client_python supports Python 3.7 and higher
+
 ## TLS 1.2 and 1.3 Support
 
-Duo_client_python uses Python's ssl module and OpenSSL for TLS operations.  Python versions 2.7 (and higher) and 3.5 (and higher) have both TLS 1.2 and TLS 1.3 support.
+Duo_client_python uses Python's ssl module and OpenSSL for TLS operations.  Python versions 3.7 (and higher) have both TLS 1.2 and TLS 1.3 support.
 
 # Installing
 
 Development:
 
 ```
 $ git clone https://github.com/duosecurity/duo_client_python.git
```

### Comparing `duo_client-4.7.1/duo_client.egg-info/SOURCES.txt` & `duo_client-5.0.0/duo_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 duo_client.egg-info/top_level.txt
 duo_client/logs/__init__.py
 duo_client/logs/telephony.py
 examples/create_integration_sso_generic.py
 examples/create_user_and_phone.py
 examples/get_billing_and_telephony_credits.py
 examples/log_examples.py
+examples/policies.py
 examples/report_auths_by_country.py
 examples/report_users_and_phones.py
 examples/trust_monitor_events.py
 examples/splunk/duo.conf
 examples/splunk/splunk.py
 tests/__init__.py
 tests/test_client.py
@@ -45,14 +46,15 @@
 tests/admin/test_desktop_tokens.py
 tests/admin/test_endpoints.py
 tests/admin/test_groups.py
 tests/admin/test_integration.py
 tests/admin/test_integrations.py
 tests/admin/test_logo.py
 tests/admin/test_phones.py
+tests/admin/test_policies.py
 tests/admin/test_settings.py
 tests/admin/test_telephony.py
 tests/admin/test_tokens.py
 tests/admin/test_trust_monitor_events.py
 tests/admin/test_u2f.py
 tests/admin/test_user_bypass_codes.py
 tests/admin/test_user_groups.py
```

### Comparing `duo_client-4.7.1/examples/create_integration_sso_generic.py` & `duo_client-5.0.0/examples/create_integration_sso_generic.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/examples/create_user_and_phone.py` & `duo_client-5.0.0/examples/create_user_and_phone.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/examples/get_billing_and_telephony_credits.py` & `duo_client-5.0.0/examples/get_billing_and_telephony_credits.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/examples/log_examples.py` & `duo_client-5.0.0/examples/log_examples.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/examples/report_auths_by_country.py` & `duo_client-5.0.0/examples/report_auths_by_country.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/examples/report_users_and_phones.py` & `duo_client-5.0.0/examples/report_users_and_phones.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/examples/splunk/splunk.py` & `duo_client-5.0.0/examples/splunk/splunk.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/examples/trust_monitor_events.py` & `duo_client-5.0.0/examples/trust_monitor_events.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/setup.py` & `duo_client-5.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/base.py` & `duo_client-5.0.0/tests/admin/base.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_activity.py` & `duo_client-5.0.0/tests/admin/test_activity.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_administrative_units.py` & `duo_client-5.0.0/tests/admin/test_administrative_units.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_admins.py` & `duo_client-5.0.0/tests/admin/test_admins.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_authlog.py` & `duo_client-5.0.0/tests/admin/test_authlog.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_bypass_codes.py` & `duo_client-5.0.0/tests/admin/test_bypass_codes.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_desktop_tokens.py` & `duo_client-5.0.0/tests/admin/test_desktop_tokens.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_endpoints.py` & `duo_client-5.0.0/tests/admin/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_groups.py` & `duo_client-5.0.0/tests/admin/test_groups.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_integration.py` & `duo_client-5.0.0/tests/admin/test_integration.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_integrations.py` & `duo_client-5.0.0/tests/admin/test_integrations.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_logo.py` & `duo_client-5.0.0/tests/admin/test_logo.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_phones.py` & `duo_client-5.0.0/tests/admin/test_phones.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_settings.py` & `duo_client-5.0.0/tests/admin/test_settings.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_telephony.py` & `duo_client-5.0.0/tests/admin/test_telephony.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_tokens.py` & `duo_client-5.0.0/tests/admin/test_tokens.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_trust_monitor_events.py` & `duo_client-5.0.0/tests/admin/test_trust_monitor_events.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_u2f.py` & `duo_client-5.0.0/tests/admin/test_u2f.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_user_bypass_codes.py` & `duo_client-5.0.0/tests/admin/test_user_bypass_codes.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_user_groups.py` & `duo_client-5.0.0/tests/admin/test_user_groups.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_user_phones.py` & `duo_client-5.0.0/tests/admin/test_user_phones.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_user_tokens.py` & `duo_client-5.0.0/tests/admin/test_user_tokens.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_user_u2f.py` & `duo_client-5.0.0/tests/admin/test_user_u2f.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_user_webauthn.py` & `duo_client-5.0.0/tests/admin/test_user_webauthn.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_users.py` & `duo_client-5.0.0/tests/admin/test_users.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/admin/test_webauthn.py` & `duo_client-5.0.0/tests/admin/test_webauthn.py`

 * *Files identical despite different names*

### Comparing `duo_client-4.7.1/tests/test_client.py` & `duo_client-5.0.0/tests/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -410,14 +410,56 @@
     def test_get_all_objects(self):
         response = self.client.json_paging_api_call(
             'GET', '/admin/v1/objects', {'limit':'1000'})
         expected = [obj.to_json() for obj in self.objects]
         self.assertListEqual(expected, list(response))
         self.assertEqual(1, self.client.counter)
 
+class TestAlternatePaging(unittest.TestCase):
+    def setUp(self):
+        self.client = util.CountingClient(
+            'test_ikey', 'test_akey', 'example.com', paging_limit=100)
+        self.objects = [util.MockJsonObject() for i in range(1000)]
+        self.client._connect = lambda: util.MockAlternatePagingHTTPConnection(self.objects)
+
+    def test_get_objects_paging(self):
+        response = self.client.json_cursor_api_call(
+            'GET', '/admin/v1/objects', {},
+            lambda response: response['data']
+        )
+        self.assertEqual(len(self.objects), len(list(response)))
+        self.assertEqual(10, self.client.counter)
+
+    def test_get_no_objects_paging(self):
+        self.objects = []
+        self.client._connect = lambda: util.MockAlternatePagingHTTPConnection(self.objects)
+        response = self.client.json_cursor_api_call(
+            'GET', '/admin/v1/objects', {},
+            lambda response: response['data']
+        )
+        self.assertEqual(len(self.objects), len(list(response)))
+        self.assertEqual(1, self.client.counter)
+
+    def test_get_objects_paging_limit(self):
+        response = self.client.json_cursor_api_call(
+            'GET', '/admin/v1/objects', {'limit':'250'},
+            lambda response: response['data']
+        )
+        self.assertEqual(len(self.objects), len(list(response)))
+        self.assertEqual(4, self.client.counter)
+
+    def test_get_all_objects(self):
+        response = self.client.json_cursor_api_call(
+            'GET', '/admin/v1/objects', {'limit':'1000'},
+            lambda response: response['data']
+        )
+        expected = [obj.to_json() for obj in self.objects]
+        self.assertListEqual(expected, list(response))
+        self.assertEqual(1, self.client.counter)
+
 class TestRequestsV4(unittest.TestCase):
     # usful args for testing GETs
     args_in = {
         'foo':['bar'],
         'baz':['qux', 'quux=quuux', 'foobar=foobar&barbaz=barbaz']}
     args_out = dict(
         (key, [v for v in val])
```

### Comparing `duo_client-4.7.1/tests/util.py` & `duo_client-5.0.0/tests/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,15 +119,36 @@
         self.uri = uri
         self.body = body
         self.headers = headers
         parsed = six.moves.urllib.parse.urlparse(uri)
         params = six.moves.urllib.parse.parse_qs(parsed.query)
 
         self.limit = int(params['limit'][0])
-        self.offset = int(params['offset'][0])
+
+        # offset is always present with list-based paging but cannot be
+        # present on the initial request with cursor-based paging
+        self.offset = int(params.get('offset', [0])[0])
+
+class MockAlternatePagingHTTPConnection(MockPagingHTTPConnection):
+    def read(self):
+        metadata = {}
+        metadata['total_objects'] = len(self.objects)
+        if self.offset + self.limit < len(self.objects):
+            metadata['next_offset'] = self.offset + self.limit
+        if self.offset > 0:
+            metadata['prev_offset'] = max(self.offset-self.limit, 0)
+
+        return json.dumps(
+                {"stat":"OK",
+                 "response": {
+                    "data" : self.objects[self.offset: self.offset+self.limit],
+                    "metadata": metadata
+                  },
+                },
+                cls=MockObjectJsonEncoder)
 
 
 class MockMultipleRequestHTTPConnection(MockHTTPConnection):
     def __init__(self, statuses):
         super(MockMultipleRequestHTTPConnection, self).__init__()
         self.statuses = statuses
         self.status_iterator = iter(statuses)
```

