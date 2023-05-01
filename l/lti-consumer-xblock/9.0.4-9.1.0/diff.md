# Comparing `tmp/lti-consumer-xblock-9.0.4.tar.gz` & `tmp/lti-consumer-xblock-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lti-consumer-xblock-9.0.4.tar", last modified: Tue Apr 25 18:30:45 2023, max compression
+gzip compressed data, was "lti-consumer-xblock-9.1.0.tar", last modified: Mon May  1 14:39:31 2023, max compression
```

## Comparing `lti-consumer-xblock-9.0.4.tar` & `lti-consumer-xblock-9.1.0.tar`

### file list

```diff
@@ -1,245 +1,245 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13412 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      672 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14958 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/django.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.476392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13817 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/tests/test_oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.476392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/ags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    32648 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.476392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.476392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      388 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      554 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3298 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10557 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/nprs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.476392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.476392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.476392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     9039 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    39510 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    71037 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0002_ltiagslineitem.py
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0003_ltiagsscore.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0005_migrate_keyset_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0007_ltidlcontentitem.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0008_fix_uuid_backfill.py
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0013_auto_20210712_1352.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0014_adds_external_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0015_add_additional_1p3_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/outcomes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11681 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/plugin/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/public/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/public/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ar/
--rw-r--r--   0 runner    (1001) docker     (122)    22730 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ar/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/en/
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/en/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/es_419/
--rw-r--r--   0 runner    (1001) docker     (122)    23422 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/es_419/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/fr/
--rw-r--r--   0 runner    (1001) docker     (122)    21751 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/fr/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/he/
--rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/he/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/hi/
--rw-r--r--   0 runner    (1001) docker     (122)     3735 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/hi/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/it/
--rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/it/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ja/
--rw-r--r--   0 runner    (1001) docker     (122)    17362 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ja/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ko/
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ko/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/pt_BR/
--rw-r--r--   0 runner    (1001) docker     (122)     4601 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/pt_BR/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/pt_PT/
--rw-r--r--   0 runner    (1001) docker     (122)    13621 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/pt_PT/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ru/
--rw-r--r--   0 runner    (1001) docker     (122)     3772 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ru/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/zh_CN/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/signals/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/static/css/student.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)    11301 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/static/js/xblock_lti_consumer.js
--rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/static/js/xblock_studio_view.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/static/sass/
--rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/static/sass/student.scss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/dl_response_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/dl_response_saved.html
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_dl_content.html
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_html.html
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_image.html
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_1p3_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_1p3_permission_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_1p3_studio.html
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_iframe.html
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_launch_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_proctoring_start_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/student.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/templates/xml/
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/xml/outcome_service_response.xml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templatetags/get_dl_lti_launch_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templatetags/lti_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2807 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11288 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_proctoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    82946 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_lti_xblock.py
--rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/track.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10252 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ar/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/en/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    20799 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26467 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    18761 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25340 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9608 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/he/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/he/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/hi/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16407 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/hi/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16884 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ru/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16547 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ru/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16458 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-25 18:30:45.000000 lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7590 2023-04-25 18:30:45.000000 lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-25 18:30:45.000000 lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-04-25 18:30:45.000000 lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-04-25 18:30:45.000000 lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-25 18:30:45.000000 lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-25 18:30:45.496393 lti-consumer-xblock-9.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.984879 lti-consumer-xblock-9.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-05-01 14:39:31.984879 lti-consumer-xblock-9.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13412 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.964879 lti-consumer-xblock-9.1.0/lti_consumer/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5921 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.964879 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15199 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.964879 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/contrib/django.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.964879 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/contrib/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/contrib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/contrib/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.968879 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13965 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/tests/test_oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.968879 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32649 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.968879 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.968879 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      388 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      554 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3298 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10557 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/nprs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.968879 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.968879 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.972879 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9039 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/test_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39510 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/test_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/test_key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/test_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    72133 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/lti_xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.972879 lti-consumer-xblock-9.1.0/lti_consumer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0002_ltiagslineitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0003_ltiagsscore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0005_migrate_keyset_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0007_ltidlcontentitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0008_fix_uuid_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0013_auto_20210712_1352.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0014_adds_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0015_add_additional_1p3_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/outcomes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.972879 lti-consumer-xblock-9.1.0/lti_consumer/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11681 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/plugin/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35176 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.960879 lti-consumer-xblock-9.1.0/lti_consumer/public/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.960879 lti-consumer-xblock-9.1.0/lti_consumer/public/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.960879 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.972879 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/ar/
+-rw-r--r--   0 runner    (1001) docker     (122)    22730 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/ar/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.972879 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/en/
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/en/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.972879 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/es_419/
+-rw-r--r--   0 runner    (1001) docker     (122)    23422 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/es_419/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.972879 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/fr/
+-rw-r--r--   0 runner    (1001) docker     (122)    21751 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/fr/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.972879 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/he/
+-rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/he/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.972879 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/hi/
+-rw-r--r--   0 runner    (1001) docker     (122)     3735 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/hi/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.976879 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/it/
+-rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/it/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.976879 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/ja/
+-rw-r--r--   0 runner    (1001) docker     (122)    17362 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/ja/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.976879 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/ko/
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/ko/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.976879 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/pt_BR/
+-rw-r--r--   0 runner    (1001) docker     (122)     4601 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/pt_BR/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.976879 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/pt_PT/
+-rw-r--r--   0 runner    (1001) docker     (122)    13621 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/pt_PT/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.976879 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/ru/
+-rw-r--r--   0 runner    (1001) docker     (122)     3772 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/ru/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.976879 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/zh_CN/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.976879 lti-consumer-xblock-9.1.0/lti_consumer/signals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.960879 lti-consumer-xblock-9.1.0/lti_consumer/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.976879 lti-consumer-xblock-9.1.0/lti_consumer/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/static/css/student.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.976879 lti-consumer-xblock-9.1.0/lti_consumer/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    12186 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/static/js/xblock_lti_consumer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/static/js/xblock_studio_view.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.976879 lti-consumer-xblock-9.1.0/lti_consumer/static/sass/
+-rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/static/sass/student.scss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.960879 lti-consumer-xblock-9.1.0/lti_consumer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.976879 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.976879 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti-dl/
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti-dl/dl_response_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti-dl/dl_response_saved.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti-dl/render_dl_content.html
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti-dl/render_html.html
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti-dl/render_image.html
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti-dl/render_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti_1p3_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti_1p3_permission_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti_1p3_studio.html
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti_iframe.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti_launch_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti_proctoring_start_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/html/student.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.976879 lti-consumer-xblock-9.1.0/lti_consumer/templates/xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templates/xml/outcome_service_response.xml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.976879 lti-consumer-xblock-9.1.0/lti_consumer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templatetags/get_dl_lti_launch_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/templatetags/lti_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.980879 lti-consumer-xblock-9.1.0/lti_consumer/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.980879 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.980879 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11288 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/plugin/test_proctoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/plugin/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    84733 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/test_lti_xblock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/test_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/track.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.980879 lti-consumer-xblock-9.1.0/lti_consumer/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.960879 lti-consumer-xblock-9.1.0/lti_consumer/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.980879 lti-consumer-xblock-9.1.0/lti_consumer/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10252 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/ar/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/ar/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.960879 lti-consumer-xblock-9.1.0/lti_consumer/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.980879 lti-consumer-xblock-9.1.0/lti_consumer/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/en/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/en/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.960879 lti-consumer-xblock-9.1.0/lti_consumer/translations/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.980879 lti-consumer-xblock-9.1.0/lti_consumer/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    20799 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26467 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/es_419/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.960879 lti-consumer-xblock-9.1.0/lti_consumer/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.980879 lti-consumer-xblock-9.1.0/lti_consumer/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    18761 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/fr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25340 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/fr/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.960879 lti-consumer-xblock-9.1.0/lti_consumer/translations/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.984879 lti-consumer-xblock-9.1.0/lti_consumer/translations/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.960879 lti-consumer-xblock-9.1.0/lti_consumer/translations/he/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.984879 lti-consumer-xblock-9.1.0/lti_consumer/translations/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9608 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/he/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/he/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.960879 lti-consumer-xblock-9.1.0/lti_consumer/translations/hi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.984879 lti-consumer-xblock-9.1.0/lti_consumer/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/hi/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16407 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/hi/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.960879 lti-consumer-xblock-9.1.0/lti_consumer/translations/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.984879 lti-consumer-xblock-9.1.0/lti_consumer/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.960879 lti-consumer-xblock-9.1.0/lti_consumer/translations/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.984879 lti-consumer-xblock-9.1.0/lti_consumer/translations/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.960879 lti-consumer-xblock-9.1.0/lti_consumer/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.984879 lti-consumer-xblock-9.1.0/lti_consumer/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16884 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.964879 lti-consumer-xblock-9.1.0/lti_consumer/translations/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.984879 lti-consumer-xblock-9.1.0/lti_consumer/translations/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.964879 lti-consumer-xblock-9.1.0/lti_consumer/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.984879 lti-consumer-xblock-9.1.0/lti_consumer/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/ru/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16547 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/ru/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.964879 lti-consumer-xblock-9.1.0/lti_consumer/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.984879 lti-consumer-xblock-9.1.0/lti_consumer/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16458 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/lti_consumer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.984879 lti-consumer-xblock-9.1.0/lti_consumer_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-05-01 14:39:31.000000 lti-consumer-xblock-9.1.0/lti_consumer_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7590 2023-05-01 14:39:31.000000 lti-consumer-xblock-9.1.0/lti_consumer_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-01 14:39:31.000000 lti-consumer-xblock-9.1.0/lti_consumer_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-05-01 14:39:31.000000 lti-consumer-xblock-9.1.0/lti_consumer_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-01 14:39:31.000000 lti-consumer-xblock-9.1.0/lti_consumer_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-01 14:39:31.000000 lti-consumer-xblock-9.1.0/lti_consumer_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-01 14:39:31.984879 lti-consumer-xblock-9.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-01 14:39:31.984879 lti-consumer-xblock-9.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-05-01 14:39:25.000000 lti-consumer-xblock-9.1.0/setup.py
```

### Comparing `lti-consumer-xblock-9.0.4/LICENSE` & `lti-consumer-xblock-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/NOTICE` & `lti-consumer-xblock-9.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/PKG-INFO` & `lti-consumer-xblock-9.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.0.4
+Version: 9.1.0
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `lti-consumer-xblock-9.0.4/README.rst` & `lti-consumer-xblock-9.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/admin.py` & `lti-consumer-xblock-9.1.0/lti_consumer/admin.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/api.py` & `lti-consumer-xblock-9.1.0/lti_consumer/api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/apps.py` & `lti-consumer-xblock-9.1.0/lti_consumer/apps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/data.py` & `lti-consumer-xblock-9.1.0/lti_consumer/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         issuer.
     * user_role (required): The user's role as one of the keys in LTI_1P3_ROLE_MAP: staff, instructor, student, or
         guest. It can also be None if the empty list should be sent in the LTI launch message.
     * config_id (required): The config_id field of an LtiConfiguration to use for the launch.
     * resource_link_id (required): A unique identifier that is guaranteed to be unique for each placement of the LTI
         link.
     * preferred_username (optional): The user's username.
+    * name (optional): The user's full name.
     * email (optional): The user's email.
     * external_user_id (optional): A unique identifier for the user that is requesting the LTI 1.3 launch that can be
         shared externally. The identifier must be stable to the issuer. This value will be sent to the the Tool in the
         form of both the login_hint in the login initiation request and the sub claim in the ID token of the LTI 1.3
         launch message. Use this attribute to specify what value to send as this claim. Otherwise, the value of the
         required user_id attribute will be used.
     * launch_presentation_document_target (optional): The document_target property of the launch_presentation claim. It
@@ -72,14 +73,15 @@
         "LtiStartProctoring" or "LtiEndAssessment".
     """
     user_id = field()
     user_role = field()
     config_id = field()
     resource_link_id = field()
     preferred_username = field(default=None)
+    name = field(default=None)
     email = field(default=None)
     external_user_id = field(default=None)
     launch_presentation_document_target = field(default=None)
     launch_presentation_return_url = field(default=None)
     message_type = field(default="LtiResourceLinkRequest")
     context_id = field(default=None)
     context_type = field(default=None)
```

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/filters.py` & `lti-consumer-xblock-9.1.0/lti_consumer/filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/forms.py` & `lti-consumer-xblock-9.1.0/lti_consumer/forms.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/consumer.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/consumer.py`

 * *Files 5% similar despite different names*

```diff
@@ -151,45 +151,52 @@
 
     def set_user_data(
             self,
             user_id,
             roles,
             result_sourcedid,
             person_sourcedid=None,
-            person_contact_email_primary=None
+            person_contact_email_primary=None,
+            person_name_full=None,
     ):
         """
         Set user data/roles
 
         Arguments:
             user_id (string):  Unique value identifying the user
             roles (string):  A comma separated list of role values
             result_sourcedid (string):  Indicates the LIS Result Identifier (if any)
                 and uniquely identifies a row and column within the Tool Consumer gradebook
             person_sourcedid (string):  LIS identifier for the user account performing the launch
             person_contact_email_primary (string):  Primary contact email address of the user
+            person_name_full (string): Full name of the user
         """
         self.lti_user_data = {
             'user_id': user_id,
             'roles': roles,
             'lis_result_sourcedid': result_sourcedid,
         }
 
-        # Additonal user identity data
+        # Additional user identity data
         # Optional user data that can be sent to the tool, if the block is configured to do so
         if person_sourcedid:
             self.lti_user_data.update({
                 'lis_person_sourcedid': person_sourcedid,
             })
 
         if person_contact_email_primary:
             self.lti_user_data.update({
                 'lis_person_contact_email_primary': person_contact_email_primary,
             })
 
+        if person_name_full:
+            self.lti_user_data.update({
+                'lis_person_name_full': person_name_full,
+            })
+
     def set_context_data(self, context_id, context_title, context_label):
         """
         Set LTI context data
 
         Arguments:
             context_id (string):  Opaque identifier used to uniquely identify the
                 context that contains the link being launched
```

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/django.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/contrib/django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/tests/test_django.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/contrib/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/oauth.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/tests/test_consumer.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/tests/test_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,15 @@
         ))
     )
     def test_generate_launch_request_with_all_optional_parameters_set_succeeds(self):
         user_id = 'user_id'
         roles = 'roles'
         result_sourcedid = 'result_sourcedid'
         person_sourcedid = 'person_sourcedid'
+        person_name_full = 'person_name_full'
         person_contact_email_primary = 'person_contact_email_primary'
         context_id = 'context_id'
         context_title = 'context_title'
         context_label = 'context_label'
         outcome_service_url = 'outcome_service_url'
         launch_presentation_locale = 'launch_presentation_locale'
         custom_parameters = {
@@ -206,15 +207,16 @@
         resource_link_id = 'resource_link_id'
 
         self.lti_consumer.set_user_data(
             user_id,
             roles,
             result_sourcedid,
             person_sourcedid=person_sourcedid,
-            person_contact_email_primary=person_contact_email_primary
+            person_contact_email_primary=person_contact_email_primary,
+            person_name_full=person_name_full,
         )
         self.lti_consumer.set_context_data(context_id, context_title, context_label)
         self.lti_consumer.set_outcome_service_url(outcome_service_url)
         self.lti_consumer.set_launch_presentation_locale(launch_presentation_locale)
         self.lti_consumer.set_custom_parameters(custom_parameters)
 
         lti_parameters = self.lti_consumer.generate_launch_request(resource_link_id)
@@ -225,14 +227,15 @@
             'lti_message_type': 'basic-lti-launch-request',
             'lti_version': 'LTI-1p0',
             'user_id': user_id,
             'roles': roles,
             'lis_result_sourcedid': result_sourcedid,
             'lis_person_sourcedid': person_sourcedid,
             'lis_person_contact_email_primary': person_contact_email_primary,
+            'lis_person_name_full': person_name_full,
             'context_id': context_id,
             'context_label': context_label,
             'context_title': context_title,
             'lis_outcome_service_url': outcome_service_url,
             'launch_presentation_locale': launch_presentation_locale,
             'custom_parameter_1': custom_parameters['custom_parameter_1'],
             'custom_parameter_2': custom_parameters['custom_parameter_2'],
```

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/tests/test_oauth.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p1/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/ags.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/constants.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/constants.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/consumer.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
             "sub": user_id,
 
             # Roles claim
             # Array of URI values for roles that the user has within the message's context
             "https://purl.imsglobal.org/spec/lti/claim/roles": self._get_user_roles(role)
         }
 
-        # Additonal user identity claims
+        # Additional user identity claims
         # Optional user data that can be sent to the tool, if the block is configured to do so
         if full_name:
             self.lti_claim_user_data.update({
                 "name": full_name,
             })
 
         if email_address:
```

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/deep_linking.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/exceptions.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/exceptions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/utils.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/extensions/rest_framework/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/key_handlers.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/nprs.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/nprs.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_ags.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/test_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_consumer.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_deep_linking.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/test_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_key_handlers.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/test_key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_nrps.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_1p3/tests/test_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/lti_xblock.py` & `lti-consumer-xblock-9.1.0/lti_consumer/lti_xblock.py`

 * *Files 2% similar despite different names*

```diff
@@ -574,21 +574,29 @@
     ask_to_send_username = Boolean(
         display_name=_("Request user's username"),
         # Translators: This is used to request the user's username for a third party service.
         help=_("Select True to request the user's username."),
         default=False,
         scope=Scope.settings
     )
+    ask_to_send_full_name = Boolean(
+        display_name=_("Request user's full name"),
+        # Translators: This is used to request the user's full name for a third party service.
+        help=_("Select True to request the user's full name."),
+        default=False,
+        scope=Scope.settings
+    )
     ask_to_send_email = Boolean(
         display_name=_("Request user's email"),
         # Translators: This is used to request the user's email for a third party service.
         help=_("Select True to request the user's email address."),
         default=False,
         scope=Scope.settings
     )
+
     enable_processors = Boolean(
         display_name=_("Send extra parameters"),
         help=_("Select True to send the extra parameters, which might contain Personally Identifiable Information. "
                "The processors are site-wide, please consult the site administrator if you have any questions."),
         default=False,
         scope=Scope.settings
     )
@@ -604,15 +612,15 @@
         'lti_advantage_deep_linking_enabled', 'lti_advantage_deep_linking_launch_url',
         'lti_advantage_ags_mode',
         # LTI 1.1 variables
         'lti_id', 'launch_url',
         # Other parameters
         'custom_parameters', 'launch_target', 'button_text', 'inline_height', 'modal_height',
         'modal_width', 'has_score', 'weight', 'hide_launch', 'accept_grades_past_due',
-        'ask_to_send_username', 'ask_to_send_email', 'enable_processors',
+        'ask_to_send_username', 'ask_to_send_full_name', 'ask_to_send_email', 'enable_processors',
     )
 
     # Author view
     has_author_view = True
 
     @staticmethod
     def workbench_scenarios():
@@ -700,21 +708,24 @@
         except Exception:
             log.exception('Something went wrong in reading the LTI XBlock configuration.')
             raise
 
     def get_pii_sharing_enabled(self):
         """
         Returns whether PII can be transmitted via this XBlock. This controls both whether the PII sharing XBlock
-        fields ask_to_send_username and ask_to_send_email are displayed in Studio and whether these data are shared
-        in LTI launches, regardless of the values of the settings on the XBlock.
+        fields ask_to_send_username, ask_to_send_full_name, and ask_to_send_email are displayed in Studio and whether
+        these data are shared in LTI launches, regardless of the values of the settings on the XBlock.
         """
         config_service = self.runtime.service(self, 'lti-configuration')
         if config_service:
-            is_already_sharing_learner_info = self.ask_to_send_email or self.ask_to_send_username
-
+            is_already_sharing_learner_info = (
+                self.ask_to_send_username or
+                self.ask_to_send_full_name or
+                self.ask_to_send_email
+            )
             return config_service.configuration.lti_access_to_learners_editable(
                 self.scope_ids.usage_id.context_key,
                 is_already_sharing_learner_info,
             )
 
         # TODO: The LTI configuration service is currently only available from the studio_view. This means that
         #       the CourseAllowPIISharingInLTIFlag does not control PII sharing in the author_view or student_view,
@@ -734,16 +745,16 @@
         environment. For example, if the external_config_filter_enabled flag is not enabled, the external_config field
         should not be a part of editable_fields, because no user can edit this field in this case. On the other hand, if
         the currently selected config_type is 'database', the fields that are otherwise stored in the database should
         still be a part of editable_fields, because a user may select a different config_type from the menu, and we want
         those fields to become editable at that time. The Javascript will determine when to show or to hide a given
         field.
 
-        Fields that are potentially filtered out include "config_type", "external_config", "ask_to_send_username", and
-        "ask_to_send_email".
+        Fields that are potentially filtered out include "config_type", "external_config", "ask_to_send_username",
+        "ask_to_send_full_name", and "ask_to_send_email".
         """
         editable_fields = self.editable_field_names
         noneditable_fields = []
 
         is_database_config_enabled = database_config_enabled(self.scope_ids.usage_id.context_key)
         is_external_config_filter_enabled = external_config_filter_enabled(self.scope_ids.usage_id.context_key)
 
@@ -753,18 +764,18 @@
             noneditable_fields.append('config_type')
 
         # If the enable_external_config_filter is not enabled, do not display the "external_config" field to users.
         if not is_external_config_filter_enabled:
             noneditable_fields.append('external_config')
 
         # update the editable fields if this XBlock is configured to not to allow the
-        # editing of 'ask_to_send_username' and 'ask_to_send_email'.
+        # editing of 'ask_to_send_username', 'ask_to_send_full_name', and 'ask_to_send_email'.
         pii_sharing_enabled = self.get_pii_sharing_enabled()
         if not pii_sharing_enabled:
-            noneditable_fields.extend(['ask_to_send_username', 'ask_to_send_email'])
+            noneditable_fields.extend(['ask_to_send_username', 'ask_to_send_full_name', 'ask_to_send_email'])
 
         editable_fields = tuple(
             field
             for field in editable_fields
             if field not in noneditable_fields
         )
 
@@ -1077,14 +1088,15 @@
 
         if not user.opt_attrs["edx-platform.is_authenticated"]:
             raise LtiError(self.ugettext("Could not get user data for current request"))
 
         user_data = {
             'user_email': None,
             'user_username': None,
+            'user_full_name': user.full_name,
             'user_language': None,
         }
 
         try:
             user_data['user_email'] = user.emails[0]
         except IndexError:
             user_data['user_email'] = None
@@ -1207,29 +1219,34 @@
             result_sourcedid = self.lis_result_sourcedid
         except LtiError:
             loader = ResourceLoader(__name__)
             template = loader.render_django_template('/templates/html/lti_launch_error.html')
             return Response(template, status=400, content_type='text/html')
 
         username = None
+        full_name = None
         email = None
+
         # Send PII fields only if this XBlock is configured to allow the sending PII.
         pii_sharing_enabled = self.get_pii_sharing_enabled()
         if pii_sharing_enabled:
             if self.ask_to_send_username and real_user_data['user_username']:
                 username = real_user_data['user_username']
+            if self.ask_to_send_full_name and real_user_data['user_full_name']:
+                full_name = real_user_data['user_full_name']
             if self.ask_to_send_email and real_user_data['user_email']:
                 email = real_user_data['user_email']
 
         lti_consumer.set_user_data(
             user_id,
             role,
             result_sourcedid=result_sourcedid,
             person_sourcedid=username,
-            person_contact_email_primary=email
+            person_contact_email_primary=email,
+            person_name_full=full_name,
         )
 
         lti_consumer.set_context_data(
             self.context_id,
             self.course.display_name_with_default,
             self.course.display_org_with_default
         )
@@ -1526,32 +1543,36 @@
         from lti_consumer.api import config_id_for_block
         config_id = config_id_for_block(self)
 
         location = self.scope_ids.usage_id
         course_key = str(location.context_key)
 
         username = None
+        full_name = None
         email = None
 
         pii_sharing_enabled = self.get_pii_sharing_enabled()
         if pii_sharing_enabled:
             user_data = self.extract_real_user_data()
 
             if self.ask_to_send_username and user_data['user_username']:
                 username = user_data['user_username']
+            if self.ask_to_send_full_name and user_data['user_full_name']:
+                full_name = user_data['user_full_name']
             if self.ask_to_send_email and user_data['user_email']:
                 email = user_data['user_email']
 
         launch_data = Lti1p3LaunchData(
             user_id=self.lms_user_id,
             user_role=self.role,
             config_id=config_id,
             resource_link_id=str(location),
             external_user_id=self.external_user_id,
             preferred_username=username,
+            name=full_name,
             email=email,
             launch_presentation_document_target="iframe",
             context_id=course_key,
             context_type=["course_offering"],
             context_title=self.get_context_title(),
             context_label=course_key,
         )
@@ -1629,15 +1650,16 @@
         if self.config_type in ("database", "external"):
             lti_consumer = self._get_lti_consumer()
 
         launch_url = self._get_lti_launch_url(lti_consumer)
         lti_block_launch_handler = self._get_lti_block_launch_handler()
         lti_1p3_launch_url = self._get_lti_1p3_launch_url(lti_consumer)
 
-        # The values of ask_to_send_username and ask_to_send_email should only apply if PII sharing is enabled.
+        # The values of ask_to_send_username, ask_to_send_full_name, and ask_to_send_email should only apply if PII
+        # sharing is enabled.
         pii_sharing_enabled = self.get_pii_sharing_enabled()
 
         return {
             'launch_url': launch_url.strip(),
             'lti_1p3_launch_url': lti_1p3_launch_url,
             'element_id': self.scope_ids.usage_id.html_id(),
             'element_class': self.category,
@@ -1647,14 +1669,15 @@
             'hide_launch': self.hide_launch,
             'has_score': self.has_score,
             'weight': self.weight,
             'module_score': self.module_score,
             'comment': sanitized_comment,
             'description': self.description,
             'ask_to_send_username': self.ask_to_send_username if pii_sharing_enabled else False,
+            'ask_to_send_full_name': self.ask_to_send_full_name if pii_sharing_enabled else False,
             'ask_to_send_email': self.ask_to_send_email if pii_sharing_enabled else False,
             'button_text': self.button_text,
             'inline_height': self.inline_height,
             'modal_vertical_offset': self._get_modal_position_offset(self.modal_height),
             'modal_horizontal_offset': self._get_modal_position_offset(self.modal_width),
             'modal_width': self.modal_width,
             'accept_grades_past_due': self.accept_grades_past_due,
```

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0001_initial.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0002_ltiagslineitem.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0002_ltiagslineitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0003_ltiagsscore.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0003_ltiagsscore.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0004_keyset_mgmt_to_model.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0004_keyset_mgmt_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0005_migrate_keyset_to_model.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0005_migrate_keyset_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0007_ltidlcontentitem.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0007_ltidlcontentitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0008_fix_uuid_backfill.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0008_fix_uuid_backfill.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0009_backfill-empty-string-config-id.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0009_backfill-empty-string-config-id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0013_auto_20210712_1352.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0013_auto_20210712_1352.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0014_adds_external_id.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0014_adds_external_id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0015_add_additional_1p3_fields.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0015_add_additional_1p3_fields.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py` & `lti-consumer-xblock-9.1.0/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/models.py` & `lti-consumer-xblock-9.1.0/lti_consumer/models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/outcomes.py` & `lti-consumer-xblock-9.1.0/lti_consumer/outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/plugin/compat.py` & `lti-consumer-xblock-9.1.0/lti_consumer/plugin/compat.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/plugin/urls.py` & `lti-consumer-xblock-9.1.0/lti_consumer/plugin/urls.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/plugin/views.py` & `lti-consumer-xblock-9.1.0/lti_consumer/plugin/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,14 +183,15 @@
 
         # Set sub and roles claims.
         user_id = launch_data.external_user_id if launch_data.external_user_id else launch_data.user_id
         user_role = launch_data.user_role
         lti_consumer.set_user_data(
             user_id=user_id,
             role=user_role,
+            full_name=launch_data.name,
             email_address=launch_data.email,
             preferred_username=launch_data.preferred_username,
         )
 
         # Set resource_link claim.
         lti_consumer.set_resource_link_claim(launch_data.resource_link_id)
```

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ar/text.js` & `lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/ar/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/en/text.js` & `lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/en/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/es_419/text.js` & `lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/es_419/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/fr/text.js` & `lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/fr/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/he/text.js` & `lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/he/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/hi/text.js` & `lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/hi/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/it/text.js` & `lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/it/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ja/text.js` & `lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/ja/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ko/text.js` & `lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/ko/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/pt_BR/text.js` & `lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/pt_BR/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/pt_PT/text.js` & `lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/pt_PT/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ru/text.js` & `lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/ru/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/zh_CN/text.js` & `lti-consumer-xblock-9.1.0/lti_consumer/public/js/translations/zh_CN/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/signals/signals.py` & `lti-consumer-xblock-9.1.0/lti_consumer/signals/signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/static/css/student.css` & `lti-consumer-xblock-9.1.0/lti_consumer/static/css/student.css`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/static/js/xblock_lti_consumer.js` & `lti-consumer-xblock-9.1.0/lti_consumer/static/js/xblock_lti_consumer.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -171,22 +171,33 @@
             })
             return def.promise();
         };
 
         var $element = $(element);
         var $ltiContainer = $element.find('.lti-consumer-container');
         var askToSendUsername = $ltiContainer.data('ask-to-send-username') == 'True';
+        var askToSendFullName = $ltiContainer.data('ask-to-send-full-name') == 'True';
         var askToSendEmail = $ltiContainer.data('ask-to-send-email') == 'True';
         var ltiVersion = $ltiContainer.data('lti-version');
 
         function renderPIIConsentPromptIfRequired(onSuccess, showCancelButton = true) {
-            if (askToSendUsername && askToSendEmail) {
+            if (askToSendUsername && askToSendFullName && askToSendEmail) {
+                msg = gettext(
+                    'Click OK to have your username, full name, and e-mail address sent to a 3rd party application.'
+                );
+            } else if (askToSendUsername && askToSendEmail) {
                 msg = gettext('Click OK to have your username and e-mail address sent to a 3rd party application.');
+            } else if (askToSendUsername && askToSendFullName) {
+                msg = gettext('Click OK to have your username and full name sent to a 3rd party application.');
+            } else if (askToSendFullName && askToSendEmail) {
+                msg = gettext('Click OK to have your full name and e-mail address sent to a 3rd party application.');
             } else if (askToSendUsername) {
                 msg = gettext('Click OK to have your username sent to a 3rd party application.');
+            } else if (askToSendFullName) {
+                msg = gettext('Click OK to have your full name sent to a 3rd party application.');
             } else if (askToSendEmail) {
                 msg = gettext('Click OK to have your e-mail address sent to a 3rd party application.');
             } else {
                 onSuccess('OK');
                 return;
             }
```

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/static/js/xblock_studio_view.js` & `lti-consumer-xblock-9.1.0/lti_consumer/static/js/xblock_studio_view.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/static/sass/student.scss` & `lti-consumer-xblock-9.1.0/lti_consumer/static/sass/student.scss`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_dl_content.html` & `lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti-dl/render_dl_content.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_image.html` & `lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti-dl/render_image.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_link.html` & `lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti-dl/render_link.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_1p3_launch.html` & `lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti_1p3_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_1p3_studio.html` & `lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti_1p3_studio.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_launch.html` & `lti-consumer-xblock-9.1.0/lti_consumer/templates/html/lti_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/templates/html/student.html` & `lti-consumer-xblock-9.1.0/lti_consumer/templates/html/student.html`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     </div>
 % endif
 
 <div
     id="${element_id}"
     class="${element_class} lti-consumer-container"
     data-ask-to-send-username="${ask_to_send_username}"
+    data-ask-to-send-full-name="${ask_to_send_full_name}"
     data-ask-to-send-email="${ask_to_send_email}"
     data-lti-version="${lti_version}"
 >
 
 % if (launch_url or lti_1p3_launch_url) and not hide_launch:
     % if launch_target in ['modal', 'new_window']:
         <section class="wrapper-lti-link">
```

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/templates/xml/outcome_service_response.xml` & `lti-consumer-xblock-9.1.0/lti_consumer/templates/xml/outcome_service_response.xml`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/templatetags/get_dl_lti_launch_url.py` & `lti-consumer-xblock-9.1.0/lti_consumer/templatetags/get_dl_lti_launch_url.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/templatetags/lti_sanitize.py` & `lti-consumer-xblock-9.1.0/lti_consumer/templatetags/lti_sanitize.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/tests/test_utils.py` & `lti-consumer-xblock-9.1.0/lti_consumer/tests/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,16 +95,16 @@
 
 
 def get_mock_lti_configuration(editable):
     """
     Returns a mock object of lti-configuration service
 
     Arguments:
-        editable (bool): This indicates whether the LTI fields (i.e. 'ask_to_send_username' and
-        'ask_to_send_email') are editable.
+        editable (bool): This indicates whether the LTI fields (i.e. 'ask_to_send_username', 'ask_to_send_full_name',
+        and 'ask_to_send_email') are editable.
     """
     lti_configuration = Mock()
     lti_configuration.configuration = Mock()
     lti_configuration.configuration.lti_access_to_learners_editable = Mock(
         return_value=editable
     )
     return lti_configuration
```

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_proctoring.py` & `lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/plugin/test_proctoring.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views.py` & `lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/plugin/test_views.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views_lti_ags.py` & `lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/plugin/test_views_lti_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py` & `lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py` & `lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_api.py` & `lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_filters.py` & `lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_lti_xblock.py` & `lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/test_lti_xblock.py`

 * *Files 2% similar despite different names*

```diff
@@ -473,40 +473,46 @@
         Arguments:
             fields (list): list containing LTI Consumer XBlock's field names.
         """
         return all(field in self.xblock.editable_fields for field in fields)
 
     def test_editable_fields_with_no_config(self):
         """
-        Test that LTI XBlock's fields (i.e. 'ask_to_send_username' and 'ask_to_send_email')
+        Test that LTI XBlock's fields (i.e. 'ask_to_send_username', 'ask_to_send_full_name', and 'ask_to_send_email')
         are editable when lti-configuration service is not provided.
         """
         self.xblock.runtime.service.return_value = None
-        # Assert that 'ask_to_send_username' and 'ask_to_send_email' are editable.
-        self.assertTrue(self.are_fields_editable(fields=['ask_to_send_username', 'ask_to_send_email']))
+        # Assert that 'ask_to_send_username', 'ask_to_send_full_name', and 'ask_to_send_email' are editable.
+        self.assertTrue(
+            self.are_fields_editable(fields=['ask_to_send_username', 'ask_to_send_full_name', 'ask_to_send_email'])
+        )
 
     def test_editable_fields_when_editing_allowed(self):
         """
-        Test that LTI XBlock's fields (i.e. 'ask_to_send_username' and 'ask_to_send_email')
+        Test that LTI XBlock's fields (i.e. 'ask_to_send_username', 'ask_to_send_full_name', and 'ask_to_send_email')
         are editable when this XBlock is configured to allow it.
         """
         # this XBlock is configured to allow editing of LTI fields
         self.xblock.runtime.service.return_value = get_mock_lti_configuration(editable=True)
-        # Assert that 'ask_to_send_username' and 'ask_to_send_email' are editable.
-        self.assertTrue(self.are_fields_editable(fields=['ask_to_send_username', 'ask_to_send_email']))
+        # Assert that 'ask_to_send_username', 'ask_to_send_full_name', and 'ask_to_send_email' are editable.
+        self.assertTrue(
+            self.are_fields_editable(fields=['ask_to_send_username', 'ask_to_send_full_name', 'ask_to_send_email'])
+        )
 
     def test_editable_fields_when_editing_not_allowed(self):
         """
-        Test that LTI XBlock's fields (i.e. 'ask_to_send_username' and 'ask_to_send_email')
+        Test that LTI XBlock's fields (i.e. 'ask_to_send_username', 'ask_to_send_full_name', and 'ask_to_send_email')
         are not editable when this XBlock is configured to not to allow it.
         """
         # this XBlock is configured to not to allow editing of LTI fields
         self.xblock.runtime.service.return_value = get_mock_lti_configuration(editable=False)
-        # Assert that 'ask_to_send_username' and 'ask_to_send_email' are not editable.
-        self.assertFalse(self.are_fields_editable(fields=['ask_to_send_username', 'ask_to_send_email']))
+        # Assert that 'ask_to_send_username', 'ask_to_send_full_name', and 'ask_to_send_email' are not editable.
+        self.assertFalse(
+            self.are_fields_editable(fields=['ask_to_send_username', 'ask_to_send_full_name', 'ask_to_send_email'])
+        )
 
     def test_lti_1p3_fields_appear(self):
         """
         Test that LTI 1.3 XBlock's fields appear when `lti_1p3_enabled` returns True.
         """
         self.assertTrue(
             self.are_fields_editable(
@@ -827,14 +833,18 @@
         self.xblock._get_lti_consumer = Mock(return_value=self.mock_lti_consumer)  # pylint: disable=protected-access
         self.xblock.due = timezone.now()
         self.xblock.graceperiod = timedelta(days=1)
 
         fake_user = Mock()
         fake_user_email = 'abc@example.com'
         fake_user.emails = [fake_user_email]
+
+        full_name_mock = PropertyMock(return_value='fake_full_name')
+        type(fake_user).full_name = full_name_mock
+
         fake_username = 'fake'
         fake_user.opt_attrs = {
             "edx-platform.username": fake_username,
             "edx-platform.is_authenticated": True,
         }
 
         self.xblock.runtime.service(self, 'user').get_current_user = Mock(return_value=fake_user)
@@ -872,14 +882,18 @@
         key = 'test'
         secret = 'secret'
         type(mock_course).lti_passports = PropertyMock(return_value=[f"{provider}:{key}:{secret}"])
 
         fake_user = Mock()
         fake_user_email = 'abc@example.com'
         fake_user.emails = [fake_user_email]
+
+        full_name_mock = PropertyMock(return_value='fake_full_name')
+        type(fake_user).full_name = full_name_mock
+
         fake_username = 'fake'
         fake_user.opt_attrs = {
             "edx-platform.username": fake_username,
             "edx-platform.is_authenticated": True,
         }
         self.xblock.runtime.service(self, 'user').get_current_user = Mock(return_value=fake_user)
 
@@ -911,35 +925,45 @@
                 'lti_version': 'LTI_1p3',
                 'user_roles': 'Student',
                 'launch_url': 'https://test.co',
             }
         )
 
     @patch('lti_consumer.lti_xblock.LtiConsumerXBlock.anonymous_user_id', PropertyMock(return_value=FAKE_USER_ID))
-    @ddt.idata(product([True, False], [True, False], [True, False]))
+    @ddt.idata(product([True, False], [True, False], [True, False], [True, False]))
     @ddt.unpack
-    def test_lti_launch_pii_sharing(self, pii_sharing_enabled, ask_to_send_username, ask_to_send_email):
+    def test_lti_launch_pii_sharing(
+        self,
+        pii_sharing_enabled,
+        ask_to_send_username,
+        ask_to_send_email,
+        ask_to_send_full_name
+    ):
         """
         Test that the values of the LTI 1.1 PII fields person_sourcedid and person_contact_email_primary that are set
         on the LTI consumer are actual values for those fields only when PII sharing is enabled. If PII sharing is not
         enabled, then the values should be None.
         """
         self.xblock.get_pii_sharing_enabled = Mock(return_value=pii_sharing_enabled)
 
         self.xblock.ask_to_send_username = ask_to_send_username
+        self.xblock.ask_to_send_full_name = ask_to_send_full_name
         self.xblock.ask_to_send_email = ask_to_send_email
 
         request = make_request('', 'GET')
         self.xblock.lti_launch_handler(request)
 
         set_user_data_kwargs = {
             'result_sourcedid': self.xblock.lis_result_sourcedid,
         }
 
         set_user_data_kwargs['person_sourcedid'] = 'fake' if pii_sharing_enabled and ask_to_send_username else None
+        set_user_data_kwargs['person_name_full'] = (
+            'fake_full_name' if pii_sharing_enabled and ask_to_send_full_name else None
+        )
         set_user_data_kwargs['person_contact_email_primary'] = (
             'abc@example.com' if pii_sharing_enabled and ask_to_send_email else None
         )
 
         self.mock_lti_consumer.set_user_data.assert_called_with(FAKE_USER_ID, 'Student,Learner', **set_user_data_kwargs)
 
 
@@ -1404,16 +1428,16 @@
         """
         Test `_get_context_for_template` returns dict with correct keys
         """
         self.xblock.lti_version = lti_version
         context_keys = (
             'launch_url', 'lti_1p3_launch_url', 'element_id', 'element_class', 'launch_target',
             'display_name', 'form_url', 'hide_launch', 'has_score', 'weight', 'module_score',
-            'comment', 'description', 'ask_to_send_username', 'ask_to_send_email', 'button_text',
-            'modal_vertical_offset', 'modal_horizontal_offset', 'modal_width',
+            'comment', 'description', 'ask_to_send_username', 'ask_to_send_full_name', 'ask_to_send_email',
+            'button_text', 'modal_vertical_offset', 'modal_horizontal_offset', 'modal_width',
             'accept_grades_past_due', 'lti_version',
         )
 
         # This test isn't testing the value of any of the above keys. Calling _get_lti_block_launch_handler raises an
         # error because the mocked XBlock location attribute does not act like a UsageKey, so mock out
         # get_lti_1p3_launch_data to avoid accessing it.
         mock_get_lti_1p3_launch_data.return_value = None
@@ -1482,32 +1506,42 @@
         # Calling _get_lti_block_launch_handler raises an error because the mocked XBlock location attribute does not
         # act like a UsageKey, so mock out get_lti_1p3_launch_data to avoid accessing it.
         mock_get_lti_1p3_launch_data.return_value = None
 
         context = self.xblock._get_context_for_template()  # pylint: disable=protected-access
         self.assertEqual(context['lti_1p3_launch_url'], lti_1p3_launch_url)
 
-    @ddt.idata(product([True, False], [True, False], [True, False]))
+    @ddt.idata(product([True, False], [True, False], [True, False], [True, False]))
     @ddt.unpack
-    def test_context_pii_sharing(self, pii_sharing_enabled, ask_to_send_username, ask_to_send_email):
-        """
-        Test that the values for context keys ask_to_send_username and ask_to_send_email are the values of the
-        corresponding XBlock fields only when PII sharing is enabled. Otherwise, they should always be False.
+    def test_context_pii_sharing(
+        self,
+        pii_sharing_enabled,
+        ask_to_send_username,
+        ask_to_send_full_name,
+        ask_to_send_email
+    ):
+        """
+        Test that the values for context keys ask_to_send_username, 'ask_to_send_full_name', and ask_to_send_email
+        are the values of thecorresponding XBlock fields only when PII sharing is enabled.
+        Otherwise, they should always be False.
         """
         self.xblock.get_pii_sharing_enabled = Mock(return_value=pii_sharing_enabled)
         self.xblock.ask_to_send_username = ask_to_send_username
+        self.xblock.ask_to_send_full_name = ask_to_send_full_name
         self.xblock.ask_to_send_email = ask_to_send_email
 
         context = self.xblock._get_context_for_template()  # pylint: disable=protected-access
 
         if pii_sharing_enabled:
             self.assertEqual(context['ask_to_send_username'], self.xblock.ask_to_send_username)
+            self.assertEqual(context['ask_to_send_full_name'], self.xblock.ask_to_send_full_name)
             self.assertEqual(context['ask_to_send_email'], self.xblock.ask_to_send_email)
         else:
             self.assertEqual(context['ask_to_send_username'], False)
+            self.assertEqual(context['ask_to_send_full_name'], False)
             self.assertEqual(context['ask_to_send_email'], False)
 
 
 @ddt.ddt
 class TestProcessorSettings(TestLtiConsumerXBlock):
     """
     Unit tests for the adding custom LTI parameters.
@@ -1590,35 +1624,48 @@
         self.mock_filter_enabled_patcher = patch("lti_consumer.lti_xblock.external_config_filter_enabled")
         self.mock_database_config_enabled_patcher = patch("lti_consumer.lti_xblock.database_config_enabled")
         self.mock_filter_enabled = self.mock_filter_enabled_patcher.start()
         self.mock_database_config_enabled = self.mock_database_config_enabled_patcher.start()
         self.addCleanup(self.mock_filter_enabled_patcher.stop)
         self.addCleanup(self.mock_database_config_enabled_patcher.stop)
 
-    @ddt.idata(product([True, False], [True, False], [True, False]))
+    @ddt.idata(product([True, False], [True, False], [True, False], [True, False]))
     @ddt.unpack
-    def test_get_lti_1p3_launch_data(self, pii_sharing_enabled, ask_to_send_username, ask_to_send_email):
+    def test_get_lti_1p3_launch_data(
+        self,
+        pii_sharing_enabled,
+        ask_to_send_username,
+        ask_to_send_full_name,
+        ask_to_send_email
+    ):
         """
         Test that get_lti_1p3_launch_data returns an instance of Lti1p3LaunchData with the correct data.
         """
         # Mock out the user role and external_user_id properties.
         fake_user = Mock()
         fake_user_email = 'fake_email@example.com'
         fake_username = 'fake_username'
+
+        fake_name = 'fake_full_name'
+        full_name_mock = PropertyMock(return_value=fake_name)
+        type(fake_user).full_name = full_name_mock
+
         fake_user.emails = [fake_user_email]
+        fake_user.name = fake_name
         fake_user.opt_attrs = {
             'edx-platform.user_id': 1,
             'edx-platform.user_role': 'instructor',
             'edx-platform.is_authenticated': True,
             'edx-platform.username': fake_username,
         }
 
         self.xblock.runtime.service(self, 'user').get_current_user = Mock(return_value=fake_user)
         self.xblock.runtime.service(self, 'user').get_external_user_id = Mock(return_value="external_user_id")
         self.xblock.ask_to_send_username = ask_to_send_username
+        self.xblock.ask_to_send_full_name = ask_to_send_full_name
         self.xblock.ask_to_send_email = ask_to_send_email
 
         # Mock out get_context_title to avoid calling into the compatability layer.
         self.xblock.get_context_title = Mock(return_value="context_title")
 
         # Mock out get_pii_sharing_enabled to reduce the amount of mocking we have to do.
         self.xblock.get_pii_sharing_enabled = Mock(return_value=pii_sharing_enabled)
@@ -1641,14 +1688,17 @@
             "context_label": course_key,
         }
 
         if pii_sharing_enabled:
             if ask_to_send_username:
                 expected_launch_data_kwargs["preferred_username"] = fake_username
 
+            if ask_to_send_full_name:
+                expected_launch_data_kwargs["name"] = fake_name
+
             if ask_to_send_email:
                 expected_launch_data_kwargs["email"] = fake_user_email
 
         expected_launch_data = Lti1p3LaunchData(
             **expected_launch_data_kwargs
         )
 
@@ -2009,29 +2059,30 @@
         method of the LTI configuration service, so long as as the configuration service is available and defined.
         """
         self.xblock.runtime.service.return_value = get_mock_lti_configuration(
             editable=lti_access_to_learners_editable
         )
         self.assertEqual(self.xblock.get_pii_sharing_enabled(), lti_access_to_learners_editable)
 
-    @ddt.idata(product([True, False], [True, False]))
+    @ddt.idata(product([True, False], [True, False], [True, False]))
     @ddt.unpack
-    def test_lti_access_to_learners_editable_args(self, ask_to_send_username, ask_to_send_email):
+    def test_lti_access_to_learners_editable_args(self, ask_to_send_username, ask_to_send_full_name, ask_to_send_email):
         """
         Test that the lti_access_to_learners_editable_mock method of the LTI configuration service is called with the
         the correct arguments.
         """
         lti_configuration = Mock()
         lti_configuration.configuration = Mock()
         lti_access_to_learners_editable_mock = Mock()
         lti_configuration.configuration.lti_access_to_learners_editable = lti_access_to_learners_editable_mock
         self.xblock.runtime.service.return_value = lti_configuration
 
         self.xblock.ask_to_send_username = ask_to_send_username
+        self.xblock.ask_to_send_full_name = ask_to_send_full_name
         self.xblock.ask_to_send_email = ask_to_send_email
 
         self.xblock.get_pii_sharing_enabled()
 
         lti_access_to_learners_editable_mock.assert_called_once_with(
             self.xblock.scope_ids.usage_id.context_key,
-            ask_to_send_username or ask_to_send_email,
+            ask_to_send_username or ask_to_send_full_name or ask_to_send_email,
         )
```

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_models.py` & `lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_outcomes.py` & `lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_signals.py` & `lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/test_signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_utils.py` & `lti-consumer-xblock-9.1.0/lti_consumer/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/ar/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/ar/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/ar/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/ar/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/en/LC_MESSAGES/django.po` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/en/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/en/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/es_419/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/es_419/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/es_419/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/es_419/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/fr/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/fr/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/fr/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/fr/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/he/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/he/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/he/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/he/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/hi/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/hi/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/ru/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/ru/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/ru/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/ru/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/settings.py` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/settings.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.1.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer/utils.py` & `lti-consumer-xblock-9.1.0/lti_consumer/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/PKG-INFO` & `lti-consumer-xblock-9.1.0/lti_consumer_xblock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.0.4
+Version: 9.1.0
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/SOURCES.txt` & `lti-consumer-xblock-9.1.0/lti_consumer_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.4/setup.py` & `lti-consumer-xblock-9.1.0/setup.py`

 * *Files identical despite different names*

