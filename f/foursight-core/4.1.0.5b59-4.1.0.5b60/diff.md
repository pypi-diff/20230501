# Comparing `tmp/foursight_core-4.1.0.5b59.tar.gz` & `tmp/foursight_core-4.1.0.5b60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_core-4.1.0.5b59.tar", max compression
+gzip compressed data, was "foursight_core-4.1.0.5b60.tar", max compression
```

## Comparing `foursight_core-4.1.0.5b59.tar` & `foursight_core-4.1.0.5b60.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1083 2023-04-28 12:50:35.590272 foursight_core-4.1.0.5b59/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/__init__.py
--rw-r--r--   0        0        0     1901 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/abstract_connection.py
--rw-r--r--   0        0        0       69 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/app.py
--rw-r--r--   0        0        0   105729 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/app_utils.py
--rw-r--r--   0        0        0     2571 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/buckets.py
--rw-r--r--   0        0        0      638 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/check_schema.py
--rw-r--r--   0        0        0        3 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/check_setup.json
--rw-r--r--   0        0        0    22858 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/check_utils.py
--rw-r--r--   0        0        0      270 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/checks/__init__.py
--rw-r--r--   0        0        0     4452 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/checks/access_key_expiration_detection.py
--rw-r--r--   0        0        0     2899 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/checks/codebuild_checks.py
--rw-r--r--   0        0        0     3305 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/checks/ecs_checks.py
--rw-r--r--   0        0        0     4683 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/checks/ecs_recovery_check.py
--rw-r--r--   0        0        0        0 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/checks/helpers/__init__.py
--rw-r--r--   0        0        0      348 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/checks/helpers/confchecks.py
--rw-r--r--   0        0        0     3519 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/checks/helpers/sys_utils.py
--rw-r--r--   0        0        0     2055 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0     8375 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/checks/scaling_checks.py
--rw-r--r--   0        0        0     2658 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/checks/test_checks.py
--rw-r--r--   0        0        0    11929 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/decorators.py
--rw-r--r--   0        0        0    15050 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/deploy.py
--rw-r--r--   0        0        0     8302 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/environment.py
--rw-r--r--   0        0        0    11792 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/es_connection.py
--rw-r--r--   0        0        0     1176 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/exceptions.py
--rw-r--r--   0        0        0     5146 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/fs_connection.py
--rw-r--r--   0        0        0     8423 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/identity.py
--rw-r--r--   0        0        0     3082 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/mapping.json
--rw-r--r--   0        0        0     1014 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/package.py
--rw-r--r--   0        0        0    17191 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/react/api/auth.py
--rw-r--r--   0        0        0     7608 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/react/api/auth0_config.py
--rw-r--r--   0        0        0    23203 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/react/api/aws_network.py
--rw-r--r--   0        0        0     3038 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/react/api/aws_s3.py
--rw-r--r--   0        0        0     6315 2023-04-28 12:50:35.598272 foursight_core-4.1.0.5b59/foursight_core/react/api/aws_stacks.py
--rw-r--r--   0        0        0    28316 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/checks.py
--rw-r--r--   0        0        0    20652 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/cognito.py
--rw-r--r--   0        0        0     3952 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/cookie_utils.py
--rw-r--r--   0        0        0     6189 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/datetime_utils.py
--rw-r--r--   0        0        0     1841 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/encoding_utils.py
--rw-r--r--   0        0        0     3649 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/encryption.py
--rw-r--r--   0        0        0     4876 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/envs.py
--rw-r--r--   0        0        0     3257 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/gac.py
--rw-r--r--   0        0        0     3516 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/jwt_utils.py
--rw-r--r--   0        0        0     9524 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/misc_utils.py
--rw-r--r--   0        0        0     5164 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/portal_access_key_utils.py
--rw-r--r--   0        0        0    81003 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/react_api.py
--rw-r--r--   0        0        0    11353 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/react_api_base.py
--rw-r--r--   0        0        0     8025 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/react_route_decorator.py
--rw-r--r--   0        0        0    33393 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/react_routes.py
--rw-r--r--   0        0        0     4861 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/react_ui.py
--rw-r--r--   0        0        0      806 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/api/yaml_utils.py
--rw-r--r--   0        0        0      234 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/ui/asset-manifest.json
--rw-r--r--   0        0        0     1681 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/ui/index.html
--rw-r--r--   0        0        0        3 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/ui/manifest.json
--rw-r--r--   0        0        0    11735 2023-04-28 12:50:35.602272 foursight_core-4.1.0.5b59/foursight_core/react/ui/static/css/main.css
--rw-r--r--   0        0        0  1930742 2023-04-28 12:50:35.610273 foursight_core-4.1.0.5b59/foursight_core/react/ui/static/js/main.js
--rw-r--r--   0        0        0      597 2023-04-28 12:50:35.610273 foursight_core-4.1.0.5b59/foursight_core/route_prefixes.py
--rw-r--r--   0        0        0    10496 2023-04-28 12:50:35.610273 foursight_core-4.1.0.5b59/foursight_core/routes.py
--rw-r--r--   0        0        0    22442 2023-04-28 12:50:35.610273 foursight_core-4.1.0.5b59/foursight_core/run_result.py
--rw-r--r--   0        0        0     6330 2023-04-28 12:50:35.610273 foursight_core-4.1.0.5b59/foursight_core/s3_connection.py
--rw-r--r--   0        0        0     5282 2023-04-28 12:50:35.610273 foursight_core-4.1.0.5b59/foursight_core/schedule_decorator.py
--rw-r--r--   0        0        0     1402 2023-04-28 12:50:35.610273 foursight_core-4.1.0.5b59/foursight_core/scripts/decrypt_accounts_file.py
--rw-r--r--   0        0        0     1406 2023-04-28 12:50:35.610273 foursight_core-4.1.0.5b59/foursight_core/scripts/encrypt_accounts_file.py
--rw-r--r--   0        0        0     5370 2023-04-28 12:50:35.610273 foursight_core-4.1.0.5b59/foursight_core/sqs_utils.py
--rw-r--r--   0        0        0     1715 2023-04-28 12:50:35.610273 foursight_core-4.1.0.5b59/foursight_core/stage.py
--rw-r--r--   0        0        0     7763 2023-04-28 12:50:35.614272 foursight_core-4.1.0.5b59/foursight_core/templates/base.html
--rw-r--r--   0        0        0    20532 2023-04-28 12:50:35.614272 foursight_core-4.1.0.5b59/foursight_core/templates/header.html
--rw-r--r--   0        0        0     4090 2023-04-28 12:50:35.614272 foursight_core-4.1.0.5b59/foursight_core/templates/history.html
--rw-r--r--   0        0        0    19634 2023-04-28 12:50:35.614272 foursight_core-4.1.0.5b59/foursight_core/templates/info.html
--rw-r--r--   0        0        0     1297 2023-04-28 12:50:35.614272 foursight_core-4.1.0.5b59/foursight_core/templates/unused.html
--rw-r--r--   0        0        0     2259 2023-04-28 12:50:35.614272 foursight_core-4.1.0.5b59/foursight_core/templates/user.html
--rw-r--r--   0        0        0     1669 2023-04-28 12:50:35.614272 foursight_core-4.1.0.5b59/foursight_core/templates/users.html
--rw-r--r--   0        0        0      572 2023-04-28 12:50:35.614272 foursight_core-4.1.0.5b59/foursight_core/templates/view_checks.html
--rw-r--r--   0        0        0     2248 2023-04-28 12:50:35.614272 foursight_core-4.1.0.5b59/foursight_core/templates/view_groups.html
--rw-r--r--   0        0        0     1612 2023-04-28 12:50:35.614272 foursight_core-4.1.0.5b59/pyproject.toml
--rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 foursight_core-4.1.0.5b59/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-01 15:32:47.500104 foursight_core-4.1.0.5b60/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-05-01 15:32:47.504104 foursight_core-4.1.0.5b60/foursight_core/__init__.py
+-rw-r--r--   0        0        0     1901 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/abstract_connection.py
+-rw-r--r--   0        0        0       69 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/app.py
+-rw-r--r--   0        0        0   105101 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/app_utils.py
+-rw-r--r--   0        0        0     2571 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/buckets.py
+-rw-r--r--   0        0        0      638 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/check_schema.py
+-rw-r--r--   0        0        0        3 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/check_setup.json
+-rw-r--r--   0        0        0    22858 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/check_utils.py
+-rw-r--r--   0        0        0      270 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/checks/__init__.py
+-rw-r--r--   0        0        0     4452 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/checks/access_key_expiration_detection.py
+-rw-r--r--   0        0        0     2899 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/checks/codebuild_checks.py
+-rw-r--r--   0        0        0     3305 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/checks/ecs_checks.py
+-rw-r--r--   0        0        0     4683 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/checks/ecs_recovery_check.py
+-rw-r--r--   0        0        0        0 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/checks/helpers/__init__.py
+-rw-r--r--   0        0        0      348 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0     3519 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/checks/helpers/sys_utils.py
+-rw-r--r--   0        0        0     2055 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0     8375 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/checks/scaling_checks.py
+-rw-r--r--   0        0        0     2658 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/checks/test_checks.py
+-rw-r--r--   0        0        0    11929 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/decorators.py
+-rw-r--r--   0        0        0    15050 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/deploy.py
+-rw-r--r--   0        0        0     8302 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/environment.py
+-rw-r--r--   0        0        0    11792 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/es_connection.py
+-rw-r--r--   0        0        0     1176 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/exceptions.py
+-rw-r--r--   0        0        0     5146 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/fs_connection.py
+-rw-r--r--   0        0        0     8423 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/identity.py
+-rw-r--r--   0        0        0     3082 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/mapping.json
+-rw-r--r--   0        0        0     1014 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/package.py
+-rw-r--r--   0        0        0    16912 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/auth.py
+-rw-r--r--   0        0        0     6629 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/auth0_config.py
+-rw-r--r--   0        0        0    22994 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/aws_network.py
+-rw-r--r--   0        0        0     3038 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/aws_s3.py
+-rw-r--r--   0        0        0     6116 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/aws_stacks.py
+-rw-r--r--   0        0        0    28009 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/checks.py
+-rw-r--r--   0        0        0    20464 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/cognito.py
+-rw-r--r--   0        0        0     3952 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/cookie_utils.py
+-rw-r--r--   0        0        0     6189 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/datetime_utils.py
+-rw-r--r--   0        0        0     1841 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/encoding_utils.py
+-rw-r--r--   0        0        0     3649 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/encryption.py
+-rw-r--r--   0        0        0     4720 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/envs.py
+-rw-r--r--   0        0        0     3196 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/gac.py
+-rw-r--r--   0        0        0     3516 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/jwt_utils.py
+-rw-r--r--   0        0        0     9466 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/misc_utils.py
+-rw-r--r--   0        0        0     5164 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/portal_access_key_utils.py
+-rw-r--r--   0        0        0    78714 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/react_api.py
+-rw-r--r--   0        0        0    11210 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/react_api_base.py
+-rw-r--r--   0        0        0     8025 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/react_route_decorator.py
+-rw-r--r--   0        0        0    33872 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/react_routes.py
+-rw-r--r--   0        0        0     4805 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/react_ui.py
+-rw-r--r--   0        0        0      806 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/api/yaml_utils.py
+-rw-r--r--   0        0        0      234 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/ui/asset-manifest.json
+-rw-r--r--   0        0        0     1681 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/ui/index.html
+-rw-r--r--   0        0        0        3 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/ui/manifest.json
+-rw-r--r--   0        0        0    11735 2023-05-01 15:32:47.508104 foursight_core-4.1.0.5b60/foursight_core/react/ui/static/css/main.css
+-rw-r--r--   0        0        0  1931686 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/react/ui/static/js/main.js
+-rw-r--r--   0        0        0      597 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/route_prefixes.py
+-rw-r--r--   0        0        0    10496 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/routes.py
+-rw-r--r--   0        0        0    22442 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/run_result.py
+-rw-r--r--   0        0        0     6330 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/s3_connection.py
+-rw-r--r--   0        0        0     5282 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/schedule_decorator.py
+-rw-r--r--   0        0        0     1402 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/scripts/decrypt_accounts_file.py
+-rw-r--r--   0        0        0     1406 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/scripts/encrypt_accounts_file.py
+-rw-r--r--   0        0        0     5370 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/sqs_utils.py
+-rw-r--r--   0        0        0     1715 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/stage.py
+-rw-r--r--   0        0        0     7763 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/templates/base.html
+-rw-r--r--   0        0        0    20532 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/templates/header.html
+-rw-r--r--   0        0        0     4090 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/templates/history.html
+-rw-r--r--   0        0        0    19634 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/templates/info.html
+-rw-r--r--   0        0        0     1297 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/templates/unused.html
+-rw-r--r--   0        0        0     2259 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/templates/user.html
+-rw-r--r--   0        0        0     1669 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/templates/users.html
+-rw-r--r--   0        0        0      572 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/templates/view_checks.html
+-rw-r--r--   0        0        0     2248 2023-05-01 15:32:47.520105 foursight_core-4.1.0.5b60/foursight_core/templates/view_groups.html
+-rw-r--r--   0        0        0     1608 2023-05-01 15:32:47.524105 foursight_core-4.1.0.5b60/pyproject.toml
+-rw-r--r--   0        0        0     1194 1970-01-01 00:00:00.000000 foursight_core-4.1.0.5b60/PKG-INFO
```

### Comparing `foursight_core-4.1.0.5b59/LICENSE.txt` & `foursight_core-4.1.0.5b60/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/abstract_connection.py` & `foursight_core-4.1.0.5b60/foursight_core/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/app_utils.py` & `foursight_core-4.1.0.5b60/foursight_core/app_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,17 @@
     full_env_name,
     get_foursight_bucket,
     get_foursight_bucket_prefix,
     infer_foursight_from_env,
     short_env_name,
     public_env_name
 )
-from dcicutils import ff_utils
 from dcicutils.exceptions import InvalidParameterError
+from dcicutils import ff_utils
+from dcicutils.function_cache_decorator import function_cache
 from dcicutils.lang_utils import disjoined_list
 from dcicutils.misc_utils import get_error_message, ignored
 from dcicutils.obfuscation_utils import obfuscate_dict
 from dcicutils.secrets_utils import (get_identity_name, get_identity_secrets)
 from dcicutils.redis_tools import RedisSessionToken, RedisException, SESSION_TOKEN_COOKIE
 from .app import app
 from .check_utils import CheckHandler
@@ -134,16 +135,14 @@
         )
         self.auth0_domain = None
         self.auth0_client_id = None
         self.user_records = {}
         # self.user_record = None
         # self.user_record_error = None
         # self.user_record_error_email = None
-        self._cached_lambda_last_modified = None
-        self._cached_portal_url = {}
         super(AppUtilsCore, self).__init__()
 
     @classmethod
     def get_default_env(cls) -> str:
         return os.environ.get("ENV_NAME", cls.DEFAULT_ENV)
 
     @staticmethod
@@ -269,29 +268,26 @@
         if not email:
             return
         self.user_records[email] = user_record = self.user_records.get(email) or {"email": email}
         user_record["record"] = record
         user_record["error"] = error
         user_record["exception"] = exception
 
+    @function_cache(key=lambda self, env_name, raise_exception = False: env_name, nocache=None)
     def get_portal_url(self, env_name: str, raise_exception: bool = False) -> Optional[str]:
-        portal_url = self._cached_portal_url.get(env_name)
-        if not portal_url:
-            try:
-                environment_and_bucket_info = (
-                    self.environment.get_environment_and_bucket_info(env_name, self.stage.get_stage()))
-                portal_url = environment_and_bucket_info.get("fourfront")
-                self._cached_portal_url[env_name] = portal_url
-            except Exception as e:
-                if raise_exception:
-                    raise
-                message = f"Error getting portal URL: {get_error_message(e)}"
-                logger.error(message)
-                return None
-        return self._cached_portal_url[env_name]
+        try:
+            environment_and_bucket_info = (
+                self.environment.get_environment_and_bucket_info(env_name, self.stage.get_stage()))
+            return environment_and_bucket_info.get("fourfront")
+        except Exception as e:
+            if raise_exception:
+                raise
+            message = f"Error getting portal URL: {get_error_message(e)}"
+            logger.error(message)
+            return None
 
     def get_auth0_client_id(self, env_name: str) -> str:
         auth0_client_id = os.environ.get("CLIENT_ID")
         if not auth0_client_id:
             # TODO: Confirm that we do not actually need to do this.
             # Just in case. We should already have this value from the GAC.
             # But Will said get it from the portal (was hardcoded in the template),
@@ -796,48 +792,41 @@
                     if lambda_description.endswith("."):
                         lambda_description = lambda_description[:-1]
                     else:
                         lambda_description = lambda_description + "."
                 logger.warning(f"Reloading lambda: {lambda_name}")
                 boto_lambda.update_function_configuration(FunctionName=lambda_name, Description=lambda_description)
                 logger.warning(f"Reloaded lambda: {lambda_name}")
-                self._cached_lambda_last_modified = None
                 return True
         except Exception as e:
             logger.warning(f"Error reloading lambda ({lambda_name}): {e}")
         return False
 
+    @function_cache(nocache=None)
     def get_lambda_last_modified(self, lambda_name: str = None) -> Optional[str]:
         """
         Returns the last modified time for the given lambda name.
         See comments in reload_lambda on this.
         """
-        lambda_current = False
         if not lambda_name or lambda_name.lower() == "current" or lambda_name.lower() == "current":
             lambda_name = os.environ.get("AWS_LAMBDA_FUNCTION_NAME")
             if not lambda_name:
                 return None
-            lambda_current = True
-        if lambda_current:
-            if self._cached_lambda_last_modified:
-                return self._cached_lambda_last_modified
         try:
             boto_lambda = boto3.client("lambda")
             lambda_info = boto_lambda.get_function(FunctionName=lambda_name)
             if lambda_info:
                 lambda_arn = lambda_info["Configuration"]["FunctionArn"]
                 lambda_tags = boto_lambda.list_tags(Resource=lambda_arn)["Tags"]
                 lambda_last_modified_tag = lambda_tags.get("last_modified")
                 if lambda_last_modified_tag:
                     lambda_last_modified = self.convert_utc_datetime_to_useastern_datetime(lambda_last_modified_tag)
                 else:
                     lambda_last_modified = lambda_info["Configuration"]["LastModified"]
                     lambda_last_modified = self.convert_utc_datetime_to_useastern_datetime(lambda_last_modified)
-                if lambda_current:
-                    self._cached_lambda_last_modified = lambda_last_modified
                 return lambda_last_modified
         except Exception as e:
             logger.warning(f"Error getting lambda ({lambda_name}) last modified time: {e}")
         return None
 
     # ===== ROUTE RUNNING FUNCTIONS =====
 
@@ -2133,18 +2122,14 @@
         # was in 4dn-cloud-infra/app-{cgap,fourfront}.py; and we know the only place we create
         # this is from there and also from foursight-cgap/chalicelib/app.py and foursight/app.py
         # with the appropriate locally derived (from this AppUtilsCore) AppUtils.
         if not AppUtilsCore._singleton:
             AppUtilsCore._singleton = specific_class() if specific_class else AppUtilsCore()
         return AppUtilsCore._singleton
 
-    def cache_clear(self) -> None:
-        self._cached_lambda_last_modified = None
-        self._cached_portal_url = {}
-
 
 class AppUtils(AppUtilsCore):  # for compatibility with older imports
     """
     Class AppUtils is the most high-level class that's used directy by Chalice object app.
     This class mostly contains the functionality defined in app_utils in original foursight,
     but the details are now inherited from AppUtilsCore, which is the recommended class to
     import if you're making an AppUtils in some other library.
```

### Comparing `foursight_core-4.1.0.5b59/foursight_core/buckets.py` & `foursight_core-4.1.0.5b60/foursight_core/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/check_schema.py` & `foursight_core-4.1.0.5b60/foursight_core/check_schema.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/check_utils.py` & `foursight_core-4.1.0.5b60/foursight_core/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/checks/access_key_expiration_detection.py` & `foursight_core-4.1.0.5b60/foursight_core/checks/access_key_expiration_detection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/checks/codebuild_checks.py` & `foursight_core-4.1.0.5b60/foursight_core/checks/codebuild_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/checks/ecs_checks.py` & `foursight_core-4.1.0.5b60/foursight_core/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/checks/ecs_recovery_check.py` & `foursight_core-4.1.0.5b60/foursight_core/checks/ecs_recovery_check.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/checks/helpers/sys_utils.py` & `foursight_core-4.1.0.5b60/foursight_core/checks/helpers/sys_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/checks/helpers/wrangler_utils.py` & `foursight_core-4.1.0.5b60/foursight_core/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/checks/scaling_checks.py` & `foursight_core-4.1.0.5b60/foursight_core/checks/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/checks/test_checks.py` & `foursight_core-4.1.0.5b60/foursight_core/checks/test_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/decorators.py` & `foursight_core-4.1.0.5b60/foursight_core/decorators.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/deploy.py` & `foursight_core-4.1.0.5b60/foursight_core/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/environment.py` & `foursight_core-4.1.0.5b60/foursight_core/environment.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/es_connection.py` & `foursight_core-4.1.0.5b60/foursight_core/es_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/exceptions.py` & `foursight_core-4.1.0.5b60/foursight_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/fs_connection.py` & `foursight_core-4.1.0.5b60/foursight_core/fs_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/identity.py` & `foursight_core-4.1.0.5b60/foursight_core/identity.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/mapping.json` & `foursight_core-4.1.0.5b60/foursight_core/mapping.json`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/package.py` & `foursight_core-4.1.0.5b60/foursight_core/package.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/auth.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 import boto3
 import logging
 import time
 import redis
 from typing import Optional
-from dcicutils.redis_utils import create_redis_client
-from dcicutils.redis_tools import RedisBase, RedisSessionToken, SESSION_TOKEN_COOKIE
 from dcicutils.env_utils import full_env_name
+from dcicutils.function_cache_decorator import function_cache
 from dcicutils.misc_utils import ignored, PRINT
+from dcicutils.redis_tools import RedisBase, RedisSessionToken, SESSION_TOKEN_COOKIE
+from dcicutils.redis_utils import create_redis_client
 from ...app import app
 from .cookie_utils import read_cookie, read_cookie_bool
 from .envs import Envs
 from .jwt_utils import JWT_AUDIENCE_PROPERTY_NAME, JWT_SUBJECT_PROPERTY_NAME, jwt_decode, jwt_encode
 from .misc_utils import get_request_domain
 
 logging.basicConfig()
@@ -35,16 +36,14 @@
                 url=os.environ['REDIS_HOST'])
             ) if 'REDIS_HOST' in os.environ else None
         except redis.exceptions.ConnectionError:
             PRINT('Cannot connect to Redis')
             PRINT('This error is expected when deploying with remote (ElastiCache) Redis')
             self._redis = None
 
-    _cached_aws_credentials = {}
-
     def get_redis_handler(self):
         """
         Returns a handler to Redis or None if not in use
         """
         return self._redis
 
     @classmethod
@@ -261,54 +260,50 @@
 
     def _create_unauthenticated_response(self, request: dict, status: str, authtoken_decoded: dict = None) -> dict:
         """
         Creates a response suitable for a request which is NOT authenticated.
         """
         return self._create_unauthorized_response(request, status, authtoken_decoded, is_authenticated=False)
 
+    @function_cache(nocache=None)
     def get_aws_credentials(self, env: str) -> dict:
         """
         Returns basic AWS credentials info (NOT the secret).
         This is just for informational/display purposes in the UI.
         This has nothing to do with the rest of the authentication
         and authorization stuff here but vaguely related so here seems fine.
         """
-        aws_credentials = Auth._cached_aws_credentials.get(env)
-        if not aws_credentials:
+        aws_credentials = None
+        try:
+            session = boto3.session.Session()
+            credentials = session.get_credentials()
+            access_key_id = credentials.access_key
+            region_name = session.region_name
+            caller_identity = boto3.client("sts").get_caller_identity()
+            user_arn = caller_identity["Arn"]
+            account_number = caller_identity["Account"]
+            aws_credentials = {
+                "aws_account_number": account_number,
+                "aws_user_arn": user_arn,
+                "aws_access_key_id": access_key_id,
+                "aws_region": region_name,
+                "auth0_client_id": self._auth0_client
+            }
+            # Try getting the account name though probably no permission at the moment.
+            aws_account_name = None
             try:
-                session = boto3.session.Session()
-                credentials = session.get_credentials()
-                access_key_id = credentials.access_key
-                region_name = session.region_name
-                caller_identity = boto3.client("sts").get_caller_identity()
-                user_arn = caller_identity["Arn"]
-                account_number = caller_identity["Account"]
-                aws_credentials = {
-                    "aws_account_number": account_number,
-                    "aws_user_arn": user_arn,
-                    "aws_access_key_id": access_key_id,
-                    "aws_region": region_name,
-                    "auth0_client_id": self._auth0_client
-                }
-                # Try getting the account name though probably no permission at the moment.
-                aws_account_name = None
+                aws_credentials["aws_account_name"] = (
+                    boto3.client('iam').list_account_aliases()['AccountAliases'][0])
+            except Exception as e:
+                logger.warning(f"Exception (not fatal) getting AWS account alias: {e}")
+            if not aws_account_name:
                 try:
                     aws_credentials["aws_account_name"] = (
-                        boto3.client('iam').list_account_aliases()['AccountAliases'][0])
+                        boto3.client('organizations').
+                        describe_account(AccountId=account_number).get('Account').get('Name')
+                    )
                 except Exception as e:
-                    logger.warning(f"Exception (not fatal) getting AWS account alias: {e}")
-                if not aws_account_name:
-                    try:
-                        aws_credentials["aws_account_name"] = (
-                            boto3.client('organizations').
-                            describe_account(AccountId=account_number).get('Account').get('Name')
-                        )
-                    except Exception as e:
-                        logger.warning(f"Exception (not fatal) getting AWS account name: {e}")
-                Auth._cached_aws_credentials[env] = aws_credentials
-            except Exception as e:
-                logger.warning(f"Exception (not fatal) getting AWS account info: {e}")
-                return {}
+                    logger.warning(f"Exception (not fatal) getting AWS account name: {e}")
+        except Exception as e:
+            logger.warning(f"Exception (not fatal) getting AWS account info: {e}")
+            return None
         return aws_credentials
-
-    def cache_clear(self) -> None:
-        self._cached_aws_credentials = {}
```

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/auth0_config.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/auth0_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import os
 import requests
+from dcicutils.function_cache_decorator import function_cache
 from dcicutils.misc_utils import get_error_message
 from .misc_utils import get_request_domain, is_running_locally
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
@@ -58,38 +59,26 @@
     }
 
     def __init__(self, portal_url: str) -> None:
         if not portal_url:
             raise ValueError("Portal URL required for Auth0Config usage.")
         self._portal_url = portal_url
         self._config_url = f"{portal_url}{'/' if not portal_url.endswith('/') else ''}auth0_config?format=json"
-        self._config_data = {}
-        self._config_raw_data = {}
 
     def get_portal_url(self) -> str:
         return self._portal_url
 
     def get_config_url(self) -> str:
         return self._config_url
 
+    @function_cache(nocache={})
     def get_config_data(self) -> dict:
         """
         Returns relevant info (dictionary) from the Auth0 config URL in canonical form.
         It contains these properties: domain, client, sso, scope, prompt, connections.
-        This caches its data.
-        """
-        if not self._config_data:
-            self._config_data = self._get_config_data_nocache() or {}
-        return self._config_data
-
-    def _get_config_data_nocache(self) -> dict:
-        """
-        Returns relevant info (dictionary) from the Auth0 config URL in canonical form.
-        It contains these properties: domain, client, sso, scope, prompt, connections.
-        This does NOT cache its data.
         """
         config_raw_data = self.get_config_raw_data()
         domain = config_raw_data.get("auth0Domain") if config_raw_data else None
         # 2023-04-24: Change to get the Auth0 client ID from the GAC rather
         # that from the Portal /auth0_config endpoint; we still et the other
         # non-credential info (e.g. domain, scope) from that endpoint though.
         # This just makes it more consistent, having both those pieces of info
@@ -115,27 +104,18 @@
             "domain": domain or Auth0Config.FALLBACK_VALUES["domain"],
             "sso": sso or Auth0Config.FALLBACK_VALUES["sso"],
             "scope": scope or Auth0Config.FALLBACK_VALUES["scope"],
             "prompt": prompt or Auth0Config.FALLBACK_VALUES["prompt"],
             "connections": connections or Auth0Config.FALLBACK_VALUES["connections"]
         }
 
+    @function_cache(nocache={})
     def get_config_raw_data(self) -> dict:
         """
         Returns raw data (dictionary) from the Auth0 config URL.
-        This caches its data.
-        """
-        if not self._config_raw_data:
-            self._config_raw_data = self._get_config_raw_data_nocache() or {}
-        return self._config_raw_data
-
-    def _get_config_raw_data_nocache(self) -> dict:
-        """
-        Returns raw data (dictionary) from the Auth0 config URL.
-        This does NOT caches its data.
         """
         try:
             return requests.get(self.get_config_url()).json() or {}
         except Exception as e:
             logger.error(f"Exception fetching Auth0 config ({self.get_config_url()}): {get_error_message(e)}")
             return {}
 
@@ -162,13 +142,7 @@
         domain = get_request_domain(request)
         # The context (route prefix) for the Auth0 callback is effectively hardcoded at Auth0.
         # but note different for running locally (localhost) and normal server operation.
         context = "/api/" if not is_running_locally(request) else "/"
         headers = request.get("headers", {})
         scheme = headers.get("x-forwarded-proto", "http")
         return f"{scheme}://{domain}{context}callback/?react"
-
-    def cache_clear(self) -> None:
-        """
-        Clears out the caches, so next call to get_config_data() and get_config_raw_data() get fresh data.
-        """
-        self._config_data = self._config_raw_data = {}
```

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/aws_network.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/aws_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import boto3
 import copy
 import re
 from typing import Callable, Optional, Union
 # TODO: Included here until we get utils PR-236 approved/merged/pushed
 # from dcicutils.misc_utils import keys_and_values_to_dict
 from .misc_utils import keys_and_values_to_dict
+from dcicutils.function_cache_decorator import function_cache
 from dcicutils.obfuscation_utils import obfuscate_dict
-from .misc_utils import memoize, sort_dictionary_by_case_insensitive_keys
+from .misc_utils import sort_dictionary_by_case_insensitive_keys
 
 
 def _filter_boto_description_list(description: dict,
                                   name: str,
                                   predicate: Optional[Union[str, re.Pattern, Callable]] = None,
                                   create_record: Optional[Callable] = None) -> list:
     """
@@ -121,15 +122,15 @@
 
     :param tags: Dictionary of tags as described above.
     :returns: List from given dictionary of tags as described above.
     """
     return sort_dictionary_by_case_insensitive_keys(obfuscate_dict(keys_and_values_to_dict(tags)))
 
 
-@memoize
+@function_cache
 def aws_get_vpcs(predicate: Optional[Union[str, re.Pattern, Callable]] = None, raw: bool = False) -> list:
     """
     Returns the list of AWS VPCs which have tags names matching the given tag predicate.
     This predicate may be (1) a string in which case it is used to match (case-sensitive) the
     tag name exactly, or as a prefix if it ends with an asterisk; or (2) a regular expression
     against which the tag name will be matched, or (3) a function which will be called with
     each tag name and which should return True iff the tag name should be considered a match.
@@ -210,15 +211,15 @@
         }
     ec2 = boto3.client("ec2")
     vpcs = ec2.describe_vpcs()
     vpcs = _filter_boto_description_list(vpcs, "Vpcs", predicate, create_record if not raw else None)
     return vpcs
 
 
-@memoize
+@function_cache
 def aws_get_subnets(predicate: Optional[Union[str, re.Pattern, Callable]] = None,
                     vpc_id: Optional[str] = None, raw: bool = False) -> list:
     """
     Returns the list of AWS Subnets which have tags names matching the given tag predicate.
     This predicate may be (1) a string in which case it is used to match (case-sensitive) the
     tag name exactly, or as a prefix if it ends with an asterisk; or (2) a regular expression
     against which the tag name will be matched, or (3) a function which will be called with
@@ -315,15 +316,15 @@
     subnets = _filter_boto_description_list(subnets, "Subnets", predicate, create_record if not raw else None)
     if vpc_id:
         vpc_property = "vpc" if not raw else "VpcId"
         subnets = [subnet for subnet in subnets if subnet.get(vpc_property) == vpc_id]
     return subnets
 
 
-@memoize
+@function_cache
 def aws_get_security_groups(predicate: Optional[Union[str, re.Pattern, Callable]] = None,
                             vpc_id: Optional[str] = None, raw: bool = False) -> list:
     """
     Returns the list of AWS Security Groups which have tags names matching the given tag predicate.
     This predicate may be (1) a string in which case it is used to match (case-sensitive) the
     tag name exactly, or as a prefix if it ends with an asterisk; or (2) a regular expression
     against which the tag name will be matched, or (3) a function which will be called with
@@ -432,15 +433,15 @@
     if vpc_id:
         vpc_property = "vpc" if not raw else "VpcId"
         security_groups = [security_group for security_group in security_groups
                            if security_group.get(vpc_property) == vpc_id]
     return security_groups
 
 
-@memoize
+@function_cache
 def aws_get_security_group_rules(security_group_id: str, direction: Optional[str] = None, raw: bool = False) -> list:
     """
     Returns list of AWS Security Group Rules for the given Security Group ID in our own canonical form.
 
     :param security_group_id: AWS Security Group ID of Rules to return,
     :param direction: If "inbound" or "outbound" then returns only inbound/outbound rules; otherwise all.
     :param raw: Returns raw objects iff True otherwise returns our own canonical form.
@@ -482,41 +483,30 @@
         security_group_rules = [security_group_rule for security_group_rule in security_group_rules
                                 if security_group_rule.get("IsEgress") is True]
     if not raw:
         security_group_rules = [create_record(security_group_rule) for security_group_rule in security_group_rules]
     return security_group_rules
 
 
-@memoize
+@function_cache
 def aws_get_network(predicate: Optional[Union[str, re.Pattern, Callable]] = None, raw: bool = False) -> list:
     """
     Returns AWS network info, i.e. WRT VPCs, Subnets, and Security Groups, whose tags match the given predicate
 
     :param predicate: Predicate choosing which items in to return based on it matching "Value" of tag in "Tags" array,
                       within each item, whose "Key" value is "Name". Case-sensitive string matching tag name value
                       exactly or its prefix if ending in asterisk; or regular expression matching tag name; or function
                       returning True on match of given tag name.
     :param raw: Returns raw (matched) objects iff True otherwise returns our own canonical form.
     :returns: List of matching (based on predicate) AWS VPC, Subnet, and Security Group objects.
     :raises Exception: On any error.
     """
     vpcs = aws_get_vpcs(predicate, raw)
-    vpcs = copy.deepcopy(vpcs)  # Copy because we're going to modify and it's memoized.
+    vpcs = copy.deepcopy(vpcs)  # Copy because we're going to modify and it's cached.
     subnets = aws_get_subnets(predicate, None, raw)
     sgs = aws_get_security_groups(predicate, None, raw)
     vpc_property = "vpc" if not raw else "VpcId"
     id_property = "id" if not raw else "VpcId"
     for vpc in vpcs:
         vpc["subnets"] = [subnet for subnet in subnets if subnet[vpc_property] == vpc[id_property]]
         vpc["security_groups"] = [sg for sg in sgs if sg[vpc_property] == vpc[id_property]]
     return vpcs
-
-
-def aws_network_cache_clear():
-    """
-    Clears any cached info herein, i.e. based on memoize.
-    """
-    aws_get_vpcs.cache_clear()
-    aws_get_subnets.cache_clear()
-    aws_get_security_groups.cache_clear()
-    aws_get_security_group_rules.cache_clear()
-    aws_get_network.cache_clear()
```

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/aws_s3.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/aws_s3.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/aws_stacks.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/aws_stacks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import boto3
 from .datetime_utils import convert_utc_datetime_to_useastern_datetime_string
-from .misc_utils import memoize
 from .yaml_utils import load_yaml
 from collections import OrderedDict
+from dcicutils.function_cache_decorator import function_cache
 from dcicutils.obfuscation_utils import obfuscate_dict
 from typing import Optional, Union
 
 
 _STACK_NAME_PREFIX = "c4-"
 
 
-@memoize
+@function_cache
 def aws_get_stacks() -> list:
     """
     Returns the list of all known AWS CloudFormation stacks with various metadata.
     """
     def stack_id(element):
         return element.name
     stacks_info = []
@@ -36,15 +36,15 @@
         "role_arn": stack.role_arn,
         "status": stack.stack_status,
         "updated": convert_utc_datetime_to_useastern_datetime_string(stack.last_updated_time),
         "created": convert_utc_datetime_to_useastern_datetime_string(stack.creation_time)
     }
 
 
-@memoize
+@function_cache
 def aws_get_stack(stack_name_or_object: Union[str, object]) -> dict:
     """
     Returns all detailed info for the given AWS CloudFormation stack name,
     including various metadata, outputs, parameters, and resources.
     Output and parameter values are obfuscated if their names represents a sensitive value.
     """
     result = {}
@@ -56,15 +56,15 @@
         resources = aws_get_stack_resources(stack)
         result["outputs"] = outputs
         result["parameters"] = parameters
         result["resources"] = resources
     return result
 
 
-@memoize
+@function_cache
 def aws_get_stack_outputs(stack_name_or_object: Union[str, object]) -> dict:
     """
     Returns the name/value outputs for the given AWS CloudFormation stack name.
     Output values are obfuscated if the output name represents a sensitive value.
     """
     def output_id(element):
         return element["OutputKey"]
@@ -72,15 +72,15 @@
     stack = _get_aws_stack_object(stack_name_or_object)
     if stack and stack.outputs:
         for stack_output in sorted(stack.outputs, key=output_id):
             result[stack_output.get("OutputKey")] = stack_output.get("OutputValue")
     return _obfuscate(result)
 
 
-@memoize
+@function_cache
 def aws_get_stack_parameters(stack_name_or_object: Union[str, object]) -> dict:
     """
     Returns a name/value dictionary of the parameters for the given AWS CloudFormation stack name.
     Parameter values are obfuscated if the parameter name represents a sensitive value.
     """
     def parameter_id(element):
         return element["ParameterKey"]
@@ -88,15 +88,15 @@
     stack = _get_aws_stack_object(stack_name_or_object)
     if stack and stack.parameters:
         for stack_parameter in sorted(stack.parameters, key=parameter_id):
             result[stack_parameter.get("ParameterKey")] = stack_parameter.get("ParameterValue")
     return _obfuscate(result)
 
 
-@memoize
+@function_cache
 def aws_get_stack_resources(stack_name_or_object: Union[str, object]) -> dict:
     """
     Returns a name/value dictionary of the resources for the given AWS CloudFormation stack name.
     """
     def resource_id(element):
         return element.logical_resource_id
     result = {}
@@ -126,15 +126,15 @@
 
 def get_single_item_list_value(any_list: list) -> object:
     if len(any_list) != 1:
         raise Exception(f"Single item list expected but contains {len(any_list)}")
     return any_list[0]
 
 
-@memoize
+@function_cache
 def aws_get_stack_template(stack_name: str) -> dict:
     """
     Returns the AWS Cloudformation template as a dictionary for the given stack name.
     The entire template will be obfuscated according to the obfuscate_dict function.
     """
     cf = boto3.client("cloudformation")
     stack_template = cf.get_template(StackName=stack_name)
@@ -150,18 +150,9 @@
         # For other AWS stacks like c4-datastore-cgap-supertest-stack,
         # we get a simple string containing the YAML for the template.
         #
         stack_template_dict = load_yaml(stack_template_body)
     return _obfuscate(stack_template_dict)
 
 
-def aws_stacks_cache_clear() -> None:
-    aws_get_stacks.cache_clear()
-    aws_get_stack.cache_clear()
-    aws_get_stack_outputs.cache_clear()
-    aws_get_stack_parameters.cache_clear()
-    aws_get_stack_resources.cache_clear()
-    aws_get_stack_template.cache_clear()
-
-
 def _obfuscate(value: dict) -> dict:
     return obfuscate_dict(value, obfuscated="********")
```

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/checks.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import boto3
 from chalice import Cron
 import copy
 import cron_descriptor
 import logging
 import os
 from typing import Callable, Optional
+from dcicutils.function_cache_decorator import function_cache
 from ...decorators import Decorators
 from .envs import Envs
-from .misc_utils import memoize
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
 class Checks:
 
@@ -22,37 +22,37 @@
 
     def get_checks_raw(self) -> dict:
         """
         Returns a dictionary containing the pristine, original check_setup.json file contents.
         """
         return self._check_setup_raw
 
-    @memoize
+    @function_cache
     def _get_checks(self) -> dict:
         checks = self._check_setup
         for check_key in checks.keys():
             checks[check_key]["name"] = check_key
             checks[check_key]["group"] = checks[check_key]["group"]
         lambdas = self.get_annotated_lambdas()
         self._annotate_checks_for_dependencies(checks)
         self._annotate_checks_with_schedules_from_lambdas(checks, lambdas)
         self._annotate_checks_with_kwargs_from_decorators(checks)
         return checks
 
-    @memoize
+    @function_cache
     def get_checks(self, env: str) -> dict:
         """
         Returns a dictionary containing all checks, annotated with various info,
         e.g. the (cron) schedule from the associated lambdas, check kwargs, and
         associated actions, from the check function decorators; filtered by the
         given env name. Cached on the first call, except for the filtering part.
         """
         return self._filter_checks_by_env(self._get_checks(), env)
 
-    @memoize
+    @function_cache
     def get_checks_grouped(self, env: str) -> list:
         """
         Like get_checks but returns the checks grouped by their group names.
         """
         grouped_checks = []
         checks = self.get_checks(env)
         for check_name in checks:
@@ -64,15 +64,15 @@
                     grouped_check["checks"].append(check_item)
                     found = True
                     break
             if not found:
                 grouped_checks.append({"group": check_item_group, "checks": [check_item]})
         return grouped_checks
 
-    @memoize
+    @function_cache
     def get_checks_grouped_by_schedule(self, env: str) -> list:
         """
         Like get_checks_grouped but groups by schedule (i.e. by scheduling lambdas).
         """
         def create_schedule_group_title(name: str):
             """
             Pretty lame title-ifying the groiup name for display purposes, based
@@ -109,15 +109,15 @@
                             }
                             grouped_checks.append(group)
                         else:
                             group = group[0]
                         group["checks"].append(check)
         return grouped_checks
 
-    @memoize
+    @function_cache
     def get_check(self, env: str, check: str) -> Optional[dict]:
         """
         Returns the check for the given check name; filtered by the given env name.
         If it turns out the check name is really an action then return its info;
         there is a 'type' property set to 'check' or 'action indicating which it is.
         """
         checks = self.get_checks(env)
@@ -377,25 +377,25 @@
                                 "check_group": check_item.get("group")
                             })
         for lambda_item in lambdas:
             if lambda_item.get("lambda_checks"):
                 lambda_item["lambda_checks"].sort(key=lambda item: f"{item['check_group']}.{item['check_name']}")
         return lambdas
 
-    @memoize
+    @function_cache
     def _get_annotated_lambdas(self) -> dict:
         stack_name = self._get_stack_name()
         stack_template = self._get_stack_template(stack_name)
         lambdas = self._get_lambdas_from_template(stack_template)
         lambdas = self._annotate_lambdas_with_schedules_from_template(lambdas, stack_template)
         lambdas = self._annotate_lambdas_with_function_metadata(lambdas)
         lambdas = self._annotate_lambdas_with_check_setup(lambdas, self._check_setup)
         return lambdas
 
-    @memoize
+    @function_cache
     def get_annotated_lambdas(self, env: Optional[str] = None) -> dict:
         """
         Returns the dictionary of all AWS lambdas for our defined stack.
         """
         return self._filter_lambdas_by_env(self._get_annotated_lambdas(), env)
 
     def _filter_lambdas_by_env(self, lambdas: list, env: Optional[str] = None) -> list:
@@ -432,15 +432,15 @@
                 for check_schedule_name in check_schedule.keys():
                     for la in lambdas:
                         if (la["lambda_handler"] == check_schedule_name
                                 or la["lambda_handler"] == "app." + check_schedule_name):
                             check_schedule[check_schedule_name]["cron"] = la["lambda_schedule"]
                             check_schedule[check_schedule_name]["cron_description"] = la["lambda_schedule_description"]
 
-    @memoize
+    @function_cache
     def get_registry(self) -> dict:
         """
         Returns the checks registry dictionary which was set up by the @check_function
         and @action_function decoratros (deifned in decorators.py).
         """
         registry = Decorators.get_registry()
         registered_checks = [check for check in registry if registry[check]["kind"] == "check"]
@@ -536,17 +536,7 @@
             for lambda_function in lambda_functions["Functions"]:
                 if lambda_filter(lambda_function):
                     results.append(lambda_function)
             marker = lambda_functions.get("NextMarker")
             if not marker:
                 break
         return results
-
-    def cache_clear(self) -> None:
-        self._get_checks.cache_clear()
-        self.get_checks.cache_clear()
-        self.get_checks_grouped.cache_clear()
-        self.get_checks_grouped_by_schedule.cache_clear()
-        self.get_check.cache_clear()
-        self._get_annotated_lambdas.cache_clear()
-        self.get_annotated_lambdas.cache_clear()
-        self.get_registry.cache_clear()
```

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/cognito.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/cognito.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 import jwt as jwtlib
 from jwt import PyJWKClient
 import requests
 import os
 from typing import Tuple
 from typing_extensions import TypedDict
 from dcicutils.common import REGION as AWS_REGION
+from dcicutils.function_cache_decorator import function_cache
 from foursight_core.react.api.encoding_utils import base64_encode
 from foursight_core.react.api.envs import Envs
 from foursight_core.react.api.gac import Gac
 from foursight_core.react.api.jwt_utils import jwt_encode
-from foursight_core.react.api.misc_utils import get_request_domain, get_request_origin, memoize
+from foursight_core.react.api.misc_utils import get_request_domain, get_request_origin
 
 
 AWS_COGNITO_SERVICE_BASE_URL = f"https://cognito-idp.{AWS_REGION}.amazonaws.com"
 
 KEY_REGION = "region"
 KEY_DOMAIN = "domain"
 KEY_USER_POOL_ID = "userpool"
@@ -54,25 +55,22 @@
     # to localhost:3000, rather than to what the default would have been, localhost:8000.
     #
     config[KEY_CALLBACK_URL] = os.environ.get("FOURSIGHT_COGNITO_CALLBACK",
                                               f"{get_request_origin(request)}/api/react/cognito/callback")
     return config
 
 
-@memoize
+@function_cache
 def _get_cognito_oauth_config_basic() -> CognitoConfig:
     """
     Returns basic configuration info for our AWS Cognito authentication server.
     Retrieved via either environment variables of AWS Secrets Manager.
     :returns: Dictionary with basic AWS Cognito configuration info.
     """
-    #
-    # This is separated from get_cognito_oauth_config just so we can memoize these most commonly used
-    # configuration values (as the dictionary argument required for that function is not memoize-able).
-    #
+    # This is separated from get_cognito_oauth_config just so we can cache these most commonly used
     domain = os.environ.get("FOURSIGHT_COGNITO_DOMAIN")
     if not domain:
         domain = Gac.get_secret_value("COGNITO_DOMAIN")
     user_pool_id = os.environ.get("FOURSIGHT_COGNITO_USER_POOL_ID")
     if not user_pool_id:
         user_pool_id = Gac.get_secret_value("COGNITO_USER_POOL_ID")
     client_id = os.environ.get("FOURSIGHT_COGNITO_CLIENT_ID")
@@ -86,15 +84,15 @@
         KEY_SCOPES: ["openid", "email", "profile"],
         KEY_CONNECTIONS: ["Google"],
         KEY_CONFIG_URL: f"{AWS_COGNITO_SERVICE_BASE_URL}/{user_pool_id}/.well-known/openid-configuration",
         KEY_CALLBACK_URL: ""
     }
 
 
-@memoize
+@function_cache
 def _get_cognito_oauth_config_client_secret() -> str:
     """
     Returns the Cognito user pool client secret value.
     Note not returned by get_cognito_oauth_config and used only internally to this module.
     :returns: Cognito user pool client secret value.
     """
     client_secret = os.environ.get("FOURSIGHT_COGNITO_CLIENT_SECRET")
@@ -407,12 +405,7 @@
         "allowed_envs": allowed_envs,
         "known_envs": known_envs,
         "default_env": default_env,
         "domain": domain,
         "site": site
     }
     return authtoken, expires
-
-
-def clear_cognito_cache():
-    _get_cognito_oauth_config_basic.cache_clear()
-    _get_cognito_oauth_config_client_secret.cache_clear()
```

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/cookie_utils.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/cookie_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/datetime_utils.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/encoding_utils.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/encoding_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/encryption.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/encryption.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/envs.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/envs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import copy
 import logging
 import os
 from typing import Optional, Tuple
 from dcicutils import ff_utils
 from dcicutils.env_utils import foursight_env_name
+from dcicutils.function_cache_decorator import function_cache
 from dcicutils.misc_utils import find_association
 from .gac import Gac
-from .misc_utils import memoize
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
 # TODO
 # Rationalize this with dcicutil.utils env_utils functions for name versions, normalizations, comparisons.
@@ -29,45 +29,45 @@
 
     def get_known_envs(self) -> list:
         return self._known_envs
 
     def get_known_envs_count(self) -> int:
         return len(self._known_envs)
 
-    @memoize
+    @function_cache
     def get_known_envs_with_gac_names(self) -> list:
         known_envs = copy.deepcopy(self._known_envs)
         for known_env in known_envs:
             gac_name = Gac.get_gac_name(known_env["full_name"])
             if gac_name:
                 known_env["gac_name"] = gac_name
         return known_envs
 
     @staticmethod
     def get_default_env() -> str:
         return os.environ.get("ENV_NAME", Envs._DEFAULT_ENV_PLACHOLDER)
 
-    @memoize
+    @function_cache
     def is_known_env(self, env: str) -> bool:
         return self.find_known_env(env) is not None
 
-    @memoize
+    @function_cache
     def find_known_env(self, env: str) -> Optional[dict]:
         known_envs = self.get_known_envs_with_gac_names()
         return find_association(known_envs, foursight_name=foursight_env_name(env))
 
     def is_allowed_env(self, env: str, allowed_envs: list) -> bool:
         if not env or not allowed_envs:
             return False
         for allowed_env in allowed_envs:
             if self.is_same_env(env, allowed_env):
                 return True
         return False
 
-    @memoize
+    @function_cache
     def is_same_env(self, env_a: str, env_b: str) -> bool:
         return foursight_env_name(env_a) == foursight_env_name(env_b)
 
     def get_user_auth_info(self, email: str, raise_exception: bool = False) -> Tuple[list, str, str]:
         """
         Returns a tuple containing (in left-right order): the list of known environments,
         i.e the list of annotated environment name objects; the list of allowed environment
@@ -100,13 +100,7 @@
     def _is_user_allowed_access(user: Optional[dict]) -> bool:
         return user and Envs._is_user_in_one_or_more_groups(user, ["admin", "foursight"])
 
     @staticmethod
     def _is_user_in_one_or_more_groups(user: Optional[dict], allowed_groups: list) -> bool:
         user_groups = user.get("groups") if user else None
         return user_groups and any(allowed_group in user_groups for allowed_group in allowed_groups or [])
-
-    def cache_clear(self) -> None:
-        self.get_known_envs_with_gac_names.cache_clear()
-        self.is_known_env.cache_clear()
-        self.find_known_env.cache_clear()
-        self.is_same_env.cache_clear()
```

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/gac.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/gac.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import re
 import boto3
 import logging
 from dcicutils.diff_utils import DiffManager
 from dcicutils.env_utils import short_env_name
+from dcicutils.function_cache_decorator import function_cache
 from dcicutils.misc_utils import override_environ, get_error_message
 from dcicutils.obfuscation_utils import obfuscate_dict
 from dcicutils.secrets_utils import get_identity_name, get_identity_secrets
-from .misc_utils import memoize, sort_dictionary_by_case_insensitive_keys
+from .misc_utils import sort_dictionary_by_case_insensitive_keys
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 
 # The main purpose of this is to get the GAC name and to support comparison of two GACs.
 class Gac:
@@ -27,15 +28,15 @@
     @staticmethod
     def get_gac_names() -> list:
         secrets_names = Gac.get_secrets_names()
         pattern = ".*App(lication)?Config(uration)?.*"
         return [secret_name for secret_name in secrets_names if re.match(pattern, secret_name, re.IGNORECASE)]
 
     @staticmethod
-    @memoize
+    @function_cache
     def get_gac_name(env_name: str) -> str:
         gac_names = Gac.get_gac_names()
         env_name_short = short_env_name(env_name)
         pattern = re.compile(".*" + env_name_short.replace('-', '.*').replace('_', '.*') + ".*", re.IGNORECASE)
         matching_gac_names = [gac_name for gac_name in gac_names if pattern.match(gac_name)]
         if len(matching_gac_names) > 0:
             #
@@ -46,15 +47,15 @@
             # OOOH ... Should be getting this just from the IDENTITY. TODO.
             #
             return matching_gac_names[0]
         else:
             return " OR ".join(matching_gac_names)
 
     @staticmethod
-    @memoize
+    @function_cache
     def get_gac_info():
         return {
             "name": get_identity_name(),
             "values": sort_dictionary_by_case_insensitive_keys(obfuscate_dict(get_identity_secrets(), obfuscated="********")),
         }
 
     @staticmethod
@@ -72,12 +73,7 @@
             "gac_compare": sort_dictionary_by_case_insensitive_keys(obfuscate_dict(gac_values_b)),
             "gac_diffs": diffs
         }
 
     @staticmethod
     def get_secret_value(name: str) -> str:
         return get_identity_secrets().get(name)
-
-    @staticmethod
-    def cache_clear() -> None:
-        Gac.get_gac_name.cache_clear()
-        Gac.get_gac_info.cache_clear()
```

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/jwt_utils.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/misc_utils.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/misc_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from chalice.app import Request
-from functools import lru_cache
 import inspect
 import json
 import os
 import pkg_resources
 import sys
 from typing import Callable, Optional, Tuple, Union
 from urllib.parse import urlparse
 
-memoize = lru_cache(100)
-
 
 def sort_dictionary_by_case_insensitive_keys(dictionary: dict) -> dict:
     """
     Returns the given dictionary sorted by (case-insenstivie) key values; yes,
     dictionaries are ordered as of Python 3.7. If the given value is not a
     dictionary it will be coerced to one.
     :param dictionary: Dictionary to sort.
```

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/portal_access_key_utils.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/portal_access_key_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/react_api.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/react_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,43 +12,41 @@
 from typing import Optional
 import urllib.parse
 from itertools import chain
 from dcicutils.env_utils import EnvUtils, get_foursight_bucket, get_foursight_bucket_prefix, full_env_name
 from dcicutils.env_utils import get_portal_url as env_utils_get_portal_url
 from dcicutils.function_cache_decorator import function_cache, function_cache_info, function_cache_clear
 from dcicutils import ff_utils
-from dcicutils.misc_utils import ignored
+from dcicutils.misc_utils import get_error_message, ignored
 from dcicutils.obfuscation_utils import obfuscate_dict
 from dcicutils.redis_tools import RedisSessionToken, SESSION_TOKEN_COOKIE
 from dcicutils.ssl_certificate_utils import get_ssl_certificate_info
 from ...app import app
 from .auth import AUTH_TOKEN_COOKIE
 from .auth import Auth
 from .aws_network import (
     aws_get_network, aws_get_security_groups,
-    aws_get_security_group_rules, aws_get_subnets, aws_get_vpcs, aws_network_cache_clear
+    aws_get_security_group_rules, aws_get_subnets, aws_get_vpcs
 )
 from .aws_s3 import AwsS3
 from .aws_stacks import (
     aws_get_stack, aws_get_stacks,
     aws_get_stack_outputs, aws_get_stack_parameters,
     aws_get_stack_resources, aws_get_stack_template,
-    aws_stacks_cache_clear
 )
 from .checks import Checks
-from .cognito import clear_cognito_cache, get_cognito_oauth_config, handle_cognito_oauth_callback
+from .cognito import get_cognito_oauth_config, handle_cognito_oauth_callback
 from .cookie_utils import create_delete_cookie_string, read_cookie, read_cookie_bool, read_cookie_int
 from .datetime_utils import convert_uptime_to_datetime, convert_utc_datetime_to_useastern_datetime_string
 from .encryption import Encryption
 from .encoding_utils import base64_decode_to_json
 from .gac import Gac
 from .misc_utils import (
     get_base_url,
     is_running_locally,
-    memoize,
     sort_dictionary_by_case_insensitive_keys
 )
 from .portal_access_key_utils import get_portal_access_key_info
 from .react_routes import ReactRoutes
 from .react_api_base import ReactApiBase
 from .react_ui import ReactUi
 
@@ -56,33 +54,24 @@
 # Implementation functions corresponding directly to the routes in react_routes.
 class ReactApi(ReactApiBase, ReactRoutes):
 
     def __init__(self):
         super(ReactApi, self).__init__()
         self._react_ui = ReactUi(self)
         self._checks = Checks(app.core.check_handler.CHECK_SETUP, self._envs)
-        # self._cached_header = {}  # migrating to @function_cache
-        # self._cached_sqs_queue_url = None  # migrating to @function_cache
-        self._cached_accounts = None
-        self._cached_accounts_from_s3 = None
-        self._cached_elasticsearch_server_version = None
 
     @staticmethod
     def _get_stack_name() -> str:
         """
         Returns our AWS defined stack name, as specified by the STACK_NAME environment variable.
         """
         return os.environ.get("STACK_NAME")
 
-    @function_cache(nocache_none=True)
+    @function_cache(nocache=None)
     def _get_sqs_queue_url(self):
-        # Leave just commented of for now short term as migrating to use of @function_cache.
-        # if not self._cached_sqs_queue_url:
-        #     self._cached_sqs_queue_url = app.core.sqs.get_sqs_queue().url
-        # return self._cached_sqs_queue_url
         return app.core.sqs.get_sqs_queue().url
 
     def _get_versions_object(self) -> dict:
         def get_package_version(package_name: str) -> Optional[str]:
             try:
                 return pkg_resources.get_distribution(package_name).version
             except Exception:
@@ -96,26 +85,21 @@
                 "python": platform.python_version(),
                 "chalice": chalice_version,
                 "elasticsearch_server": self._get_elasticsearch_server_version(),
                 "elasticsearch": get_package_version("elasticsearch"),
                 "elasticsearch_dsl": get_package_version("elasticsearch-dsl")
             }
 
+    @function_cache(nokey=True, nocache=None)
     def _get_elasticsearch_server_version(self) -> Optional[str]:
-        if not self._cached_elasticsearch_server_version:
-            try:
-                connection = app.core.init_connection(self._envs.get_default_env())
-                es_info = connection.es_info()
-                elasticsearch_server_version = es_info["version"]["number"]
-                self._cached_elasticsearch_server_version = elasticsearch_server_version
-            except Exception:
-                pass
-        return self._cached_elasticsearch_server_version
+        connection = app.core.init_connection(self._envs.get_default_env())
+        es_info = connection.es_info()
+        return es_info.get("version", {}).get("number")
 
-    @memoize
+    @function_cache
     def _get_user_projects(self, env: str, raw: bool = False) -> list:
         """
         Returns the list of available user projects.
         """
         connection = app.core.init_connection(env)
         projects = ff_utils.search_metadata(f'/search/?type=Project&datastore=database', key=connection.ff_keys)
         if projects and not raw:
@@ -127,15 +111,15 @@
                     "title": project.get("title"),
                     "description": project.get("description")
                 }
                 for project in projects
             ]
         return projects
 
-    @memoize
+    @function_cache
     def _get_user_institutions(self, env: str, raw: bool = False) -> list:
         """
         Returns the list of available user institutions.
         """
         connection = app.core.init_connection(env)
         institutions = ff_utils.search_metadata(f'/search/?type=Institution', key=connection.ff_keys)
 
@@ -152,15 +136,15 @@
                     "title": institution.get("title"),
                     "pi": get_principle_investigator(institution)
                 }
                 for institution in institutions
             ]
         return institutions
 
-    @memoize
+    @function_cache
     def _get_user_roles(self, env: str) -> list:
         ignored(env)
         #
         # The below enumerated user role values where copied from here:
         # https://github.com/dbmi-bgm/cgap-portal/blob/master/src/encoded/schemas/user.json#L69-L106
         #
         roles = [
@@ -171,22 +155,22 @@
             "project_member",
             "patient",
             "other",
             "unknown"
         ]
         return [{"id": role, "name": role, "title": role.replace("_", " ").title()} for role in roles]
 
-    @memoize
+    @function_cache
     def _get_user_schema(self, env: str) -> dict:
         portal_url = get_base_url(app.core.get_portal_url(env))
         user_schema_url = f"{portal_url}/profiles/User.json?format=json"
         user_schema = requests.get(user_schema_url).json()
         return user_schema
 
-    @memoize
+    @function_cache
     def _get_user_statuses(self, env: str) -> list:
         user_schema = self._get_user_schema(env)
         user_schema_properties = user_schema.get("properties") if user_schema else None
         user_schema_status = user_schema_properties.get("status") if user_schema_properties else None
         user_schema_status_enum = user_schema_status.get("enum") if user_schema_status else None
         if not user_schema_status_enum:
             return []
@@ -271,19 +255,14 @@
         """
         Called from react_routes for endpoint: GET /{env}/header
         Note that this in an UNPROTECTED route.
         """
         # Note that this route is not protected but/and we return the results from authorize.
         auth = self._auth.authorize(request, env)
         data = self._reactapi_header_cache(request, env)
-        # Leave just commented of for now short term as migrating to use of @function_cache.
-        # data = self._cached_header.get(env)
-        # if not data:
-        #     data = self._reactapi_header_cache(request, env)
-        #     self._cached_header[env] = data
         data = copy.deepcopy(data)
         data["auth"] = auth
         # 2022-10-18
         # No longer sharing known-envs widely; send only if authenticated;
         # if not authenticated then act as-if the default-env is the only known-env;
         # in this case also include (as an FYI for the UI) the real number of known-envs.
         if auth["authenticated"]:
@@ -298,15 +277,15 @@
         data["auth"]["default_env"] = self._envs.get_default_env()
         # Note that these "test_mode_xyz" cookies are for testing only
         # and if used must be manually set, e.g. via Chrome Developer Tools.
         test_mode_certificate_simulate_error = read_cookie_bool(request, "test_mode_certificate_simulate_error")
         if test_mode_certificate_simulate_error:
             data["portal"]["url"] = None
         # Note that we know that data["portal"]["url"] is explicitly set via _reactapi_header_cache.
-        if not data["portal"]["url"]:
+        if not data["portal"].get("url"):
             # Here we did not get a Portal URL from the to app.core.get_portal_url (via _reactapi_header_cache).
             # That call ends up ultimately calling the Portal health endpoint (via s3Utils.get_synthetic_env_config
             # via environment.get_environment_and_bucket_info). So there may have been a problem with the Portal,
             # e.g. bad SSL certificate; we will get the Portal URL by other means, and from get get its SSL
             # certificate to help diagnose any problem with that. C4-1017 (April 2023).
             try:
                 if test_mode_certificate_simulate_error:
@@ -444,20 +423,26 @@
         response = get_portal_access_key_info(
             env,
             logged_in=logged_in,
             test_mode_access_key_simulate_error=test_mode_access_key_simulate_error,
             test_mode_access_key_expiration_warning_days=test_mode_access_key_expiration_warning_days)
         return self.create_success_response(response)
 
-    @memoize
+    def reactapi_elasticsearch(self) -> Response:
+        try:
+            return self.create_success_response(self._get_elasticsearch_server_version())
+        except Exception as e:
+            return self.create_error_response(get_error_message(e))
+
+    @function_cache
     def _get_env_and_bucket_info(self, env: str, stage_name: str) -> dict:
         return sort_dictionary_by_case_insensitive_keys(
             obfuscate_dict(app.core.environment.get_environment_and_bucket_info(env, stage_name)))
 
-    @memoize
+    @function_cache
     def _get_check_result_bucket_name(self, env: str) -> Optional[str]:
         envs = app.core.init_environments(env=env)
         if not envs:
             return None
         env = envs.get(env)
         return env.get("bucket") if env else None
 
@@ -1195,27 +1180,25 @@
         key = app.core.ACCOUNTS_FILE_NAME
         if not AwsS3.bucket_key_exists(bucket, key):
             return None
         return f"s3://{bucket}/{key}"
 
     def _get_accounts_from_s3(self, request: dict) -> Optional[dict]:
         # Let's not cache this for now, maybe change mind later, thus the OR True clause below.
-        if True or not self._cached_accounts_from_s3:
-            s3_uri = self._get_accounts_file_from_s3()
-            if not s3_uri:
-                return self._get_accounts_only_for_current_account(request)
-            s3_uri = s3_uri.replace("s3://", "")
-            s3_uri_components = s3_uri.split("/")
-            if len(s3_uri_components) != 2:
-                return self._get_accounts_only_for_current_account(request)
-            bucket = s3_uri_components[0]
-            key = s3_uri_components[1]
-            accounts_json_content = AwsS3.get_bucket_key_contents(bucket, key)
-            self._cached_accounts_from_s3 = self._read_accounts_json(accounts_json_content)
-        return self._cached_accounts_from_s3
+        s3_uri = self._get_accounts_file_from_s3()
+        if not s3_uri:
+            return self._get_accounts_only_for_current_account(request)
+        s3_uri = s3_uri.replace("s3://", "")
+        s3_uri_components = s3_uri.split("/")
+        if len(s3_uri_components) != 2:
+            return self._get_accounts_only_for_current_account(request)
+        bucket = s3_uri_components[0]
+        key = s3_uri_components[1]
+        accounts_json_content = AwsS3.get_bucket_key_contents(bucket, key)
+        return self._read_accounts_json(accounts_json_content)
 
     def _get_accounts_only_for_current_account(self, request: dict) -> Optional[list]:
         aws_credentials = self._auth.get_aws_credentials(self._envs.get_default_env())
         if aws_credentials:
             account_name = aws_credentials.get("aws_account_name")
             if account_name:
                 account_stage = app.core.stage.get_stage()
@@ -1239,27 +1222,26 @@
                 account_stage = account.get("stage")
                 if account_stage:
                     account["id"] = account_name + ":" + account_stage
                 else:
                     account["id"] = account_name
         return accounts_json
 
+    @function_cache(nocache=None)
     def _get_accounts(self) -> Optional[dict]:
         accounts_file = self._get_accounts_file()
         if not accounts_file:
             return None
-        if not self._cached_accounts:
-            try:
-                with io.open(self._get_accounts_file(), "r") as accounts_json_f:
-                    accounts_json_content_encrypted = accounts_json_f.read()
-                    accounts_json = self._read_accounts_json(accounts_json_content_encrypted)
-                    self._cached_accounts = accounts_json
-            except Exception:
-                return None
-        return self._cached_accounts
+        try:
+            with io.open(self._get_accounts_file(), "r") as accounts_json_f:
+                accounts_json_content_encrypted = accounts_json_f.read()
+                accounts_json = self._read_accounts_json(accounts_json_content_encrypted)
+                return accounts_json
+        except Exception:
+            return None
 
     def reactapi_accounts(self, request: dict, env: str, from_s3: bool = False) -> Response:
         ignored(env)
         accounts = self._get_accounts() if not from_s3 else self._get_accounts_from_s3(request)
         return self.create_success_response(accounts)
 
     def reactapi_account(self, request: dict, env: str, name: str, from_s3: bool = False) -> Response:
@@ -1573,39 +1555,12 @@
                 if function_cache_clear(name):
                     cache_cleared.append(name)
         else:
             function_cache_clear()
             cache_cleared.append("<all>")
         return self.create_success_response({"cache_cleared": cache_cleared})
 
-    def reactapi_clear_cache(self, request: dict) -> Response:
-        """
-        Called from react_routes for endpoint: GET /__clearcache___
-        Not yet implemented.
-        """
-        ignored(request)
-        app.core.cache_clear()
-        super().cache_clear()
-        self._checks.cache_clear()
-        self._react_ui.cache_clear()
-        Gac.cache_clear()
-        # self._cached_header = {}  # migrating to @function_cache
-        # self._cached_sqs_queue_url = None  # migrating to @function_cache
-        ReactApi._reactapi_header_cache.cache_clear()  # migrating to @function_cache
-        ReactApi._get_sqs_queue_url.cache_clear()  # migrating to @function_cache
-        self._cached_elasticsearch_server_version = None
-        self._cached_accounts = None
-        self._cached_accounts_from_s3 = None
-        self._get_env_and_bucket_info.cache_clear()
-        self._get_check_result_bucket_name.cache_clear()
-        self._get_user_projects.cache_clear()
-        self._get_user_institutions.cache_clear()
-        aws_network_cache_clear()
-        aws_stacks_cache_clear()
-        clear_cognito_cache()
-        return self.create_success_response({"status": "Caches cleared."})
-
     @staticmethod
     def reactapi_testsize(n: int) -> Response:
         n = int(n) - 8  # { "N": "" }
         body = {"N": "X" * n}
         return app.core.create_success_response(body)
```

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/react_api_base.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/react_api_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,12 +226,7 @@
         return app.core.APP_PACKAGE_NAME == "foursight"
 
     def get_site_name(self) -> str:
         return "foursight-cgap" if app.core.APP_PACKAGE_NAME == "foursight-cgap" else "foursight-fourfront"
 
     def get_default_env(self) -> str:
         return self._envs.get_default_env()
-
-    def cache_clear(self) -> None:
-        self._auth.cache_clear()
-        self._auth0_config.cache_clear()
-        self._envs.cache_clear()
```

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/react_route_decorator.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/react_route_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/react_routes.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/react_routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,31 @@
         Note that this in an UNPROTECTED route.
         Returns Portal access key info about this Foursight instance.
         """
         request_dict = app.current_request.to_dict()
         args = get_request_args(request_dict)
         return app.core.reactapi_portal_access_key(request_dict, args)
 
+    @route("/{env}/elasticsearch", authorize=False)
+    def reactapi_route_elasticsearch_noenv(env: str) -> Response:  # noqa: implicit @staticmethod via @route
+        """
+        Note that this in an UNPROTECTED route.
+        Pings the Elasticsearch associated with this Foursight instance and returns related info.
+        """
+        ignored(env)
+        return ReactRoutes.reactapi_route_elasticsearch_noenv()
+
+    @route("/elasticsearch", authorize=False)
+    def reactapi_route_elasticsearch_noenv() -> Response:  # noqa: implicit @staticmethod via @route
+        """
+        Note that this in an UNPROTECTED route.
+        Pings the Elasticsearch associated with this Foursight instance and returns related info.
+        """
+        return app.core.reactapi_elasticsearch()
+
     # ----------------------------------------------------------------------------------------------
     # Foursight React API routes PROTECTED by authorization/authentication.
     # ----------------------------------------------------------------------------------------------
 
     @route("/{env}/info", authorize=True)
     def reactapi_route_info(env: str) -> Response:  # noqa: implicit @staticmethod via @route
         """
@@ -589,21 +606,14 @@
     @route("/__reloadlambda__", authorize=True)
     def reactapi_route_reload_lambda() -> Response:  # noqa: implicit @staticmethod via @route
         """
         For troubleshooting only. Reload the lambda code.
         """
         return app.core.reactapi_reload_lambda(app.current_request.to_dict())
 
-    @route("/__clearcache__", authorize=True)
-    def reactapi_route_clear_cache() -> Response:  # noqa: implicit @staticmethod via @route
-        """
-        For troubleshooting only. Clear any/all internal caches.
-        """
-        return app.core.reactapi_clear_cache(app.current_request.to_dict())
-
     @route("/__testsize__/{n}", authorize=True)
     def reactapi_route_testsize(n: int) -> Response:  # noqa: implicit @staticmethod via @route
         """
         For troubleshooting only. Test response size capabilities of AWS Lamdas.
         """
         return app.core.reactapi_testsize(n)
```

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/react_ui.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/react_ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from chalice import Response
 import io
 import logging
 import os
 from typing import Optional
+from dcicutils.function_cache_decorator import function_cache
 
 logging.basicConfig()
 logger = logging.getLogger(__name__)
 
 _REACT_BASE_DIR = os.path.join(os.path.dirname(__file__), "../../react/ui")
 _REACT_DEFAULT_FILE = "index.html"
 _REACT_STATIC_FILE_TYPES = [
@@ -49,29 +50,26 @@
 
 
 class ReactUi:
 
     def __init__(self, react_api):
         self._react_api = react_api
 
-    _cached_static_files = {}
-
     @staticmethod
     def _is_known_file_suffix(file: str) -> bool:
         return any(file.endswith(file_info["suffix"]) for file_info in _REACT_STATIC_FILE_TYPES)
 
     @staticmethod
     def _get_file_info(file: str) -> Optional[dict]:
         for info in _REACT_STATIC_FILE_TYPES:
             if file.endswith(info["suffix"]):
                 return info
         return None
 
     @staticmethod
-    
     def _is_file_type_whitelisted(file: str) -> bool:
         """
         To be as restrictive as possible we ONLY allow the above whitelisted file types.
         """
         for suffix in _REACT_WHITELISTED_FILE_PATH_SUFFIXES:
             if file.endswith(suffix):
                 return True
@@ -113,23 +111,21 @@
             open_mode = "r"
         file = os.path.normpath(file)
 
         # Restrict to known whitelisted files.
         if not self._is_file_type_whitelisted(file):
             return self._react_api.create_forbidden_response()
 
-        response = ReactUi._cached_static_files.get(file)
-        if not response:
+        try:
+            return self._get_file_content_response(file, open_mode, content_type)
+        except Exception as e:
+            message = f"Exception serving static React file ({file} | {content_type}): {e}"
+            logger.error(message)
+            return self._react_api.create_error_response(message)
+
+    @function_cache
+    def _get_file_content_response(self, file: str, open_mode: str, content_type: str) -> str:
+        with io.open(file, open_mode) as f:
+            content = f.read()
             response = self._react_api.create_success_response(content_type=content_type)
-            try:
-                with io.open(file, open_mode) as f:
-                    response.body = f.read()
-            except Exception as e:
-                message = f"Exception serving static React file ({file} | {content_type}): {e}"
-                logger.error(message)
-                return self._react_api.create_error_response(message)
-            ReactUi._cached_static_files[file] = response = self._react_api.process_response(response)
-        return response
-
-    @staticmethod
-    def cache_clear() -> None:
-        ReactUi._cached_static_files = {}
+            response.body = content
+            return response
```

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/api/yaml_utils.py` & `foursight_core-4.1.0.5b60/foursight_core/react/api/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/ui/index.html` & `foursight_core-4.1.0.5b60/foursight_core/react/ui/index.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/ui/static/css/main.css` & `foursight_core-4.1.0.5b60/foursight_core/react/ui/static/css/main.css`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/react/ui/static/js/main.js` & `foursight_core-4.1.0.5b60/foursight_core/react/ui/static/js/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.a35feec3.js.LICENSE.txt */
+/*! For license information please see main.6d493f41.js.LICENSE.txt */
 (function() {
     var __webpack_modules__ = {
             4189: function(e, t) {
                 "use strict";
                 Object.defineProperty(t, "__esModule", {
                     value: !0
                 })
@@ -51323,65 +51323,93 @@
                 paddingRight: "10pt",
                 whiteSpace: "nowrap"
             },
             ca = Ye(Ye({}, la), {}, {
                 textAlign: "right"
             }),
             da = function(e) {
-                var t = e.cache,
-                    n = ua();
+                var t, n = e.cache,
+                    r = ua();
                 return (0, Kr.jsx)(Kr.Fragment, {
                     children: (0, Kr.jsxs)("tr", {
                         children: [(0, Kr.jsx)("td", {
                             style: la,
-                            children: t.function
+                            children: n.name
                         }), (0, Kr.jsx)("td", {
                             style: ca,
-                            children: t.hits
+                            children: n.hits > 0 ? n.hits : (0, Kr.jsx)(Kr.Fragment, {
+                                children: "\u2013"
+                            })
                         }), (0, Kr.jsx)("td", {
                             style: ca,
-                            children: t.misses
+                            children: n.misses > 0 ? n.misses : (0, Kr.jsx)(Kr.Fragment, {
+                                children: "\u2013"
+                            })
                         }), (0, Kr.jsx)("td", {
                             style: ca,
-                            children: t.size
-                        }), (0, Kr.jsx)("td", {
-                            style: la,
-                            children: t.updated || (0, Kr.jsx)(Kr.Fragment, {
+                            children: n.size > 0 ? n.size : (0, Kr.jsx)(Kr.Fragment, {
                                 children: "\u2013"
                             })
+                        }), (0, Kr.jsxs)("td", {
+                            style: la,
+                            id: "tooltip-updated-".concat(n.name),
+                            children: [(0, Kr.jsx)(Mi, {
+                                id: "tooltip-updated-".concat(n.name),
+                                position: "bottom",
+                                text: "Last time function was actually called."
+                            }), n.updated || (0, Kr.jsx)(Kr.Fragment, {
+                                children: "\u2013"
+                            })]
+                        }), (0, Kr.jsxs)("td", {
+                            style: ca,
+                            id: "tooltip-duration-".concat(n.name),
+                            children: [(0, Kr.jsx)(Mi, {
+                                id: "tooltip-duration-".concat(n.name),
+                                position: "bottom",
+                                text: "Duration of last actual function call."
+                            }), n.duration ? (null === (t = n.duration) || void 0 === t ? void 0 : t.toFixed(1)) + " ms" : (0, Kr.jsx)(Kr.Fragment, {
+                                children: "\u2013"
+                            })]
                         }), (0, Kr.jsx)("td", {
                             style: ca,
-                            children: t.maxsize >= Number.MAX_SAFE_INTEGER ? (0, Kr.jsx)(Kr.Fragment, {
+                            children: n.maxsize >= Number.MAX_SAFE_INTEGER ? (0, Kr.jsx)(Kr.Fragment, {
                                 children: Fr[1 / 0]
                             }) : (0, Kr.jsx)(Kr.Fragment, {
-                                children: t.maxsize
+                                children: n.maxsize
                             })
                         }), (0, Kr.jsx)("td", {
                             style: ca,
-                            children: t.ttl || (0, Kr.jsx)(Kr.Fragment, {
+                            children: n.ttl || (0, Kr.jsx)(Kr.Fragment, {
                                 children: "\u2013"
                             })
                         }), (0, Kr.jsx)("td", {
                             style: ca,
-                            children: t.ttl_none || (0, Kr.jsx)(Kr.Fragment, {
+                            children: n.ttl_none || (0, Kr.jsx)(Kr.Fragment, {
                                 children: "\u2013"
                             })
                         }), (0, Kr.jsx)("td", {
                             style: la,
-                            children: t.nocache_none ? (0, Kr.jsx)(Kr.Fragment, {
-                                children: "No"
+                            children: n.nocache_none ? (0, Kr.jsx)(Kr.Fragment, {
+                                children: "Yes"
                             }) : (0, Kr.jsx)(Kr.Fragment, {
+                                children: "\u2013"
+                            })
+                        }), (0, Kr.jsx)("td", {
+                            style: la,
+                            children: n.nocache_other ? (0, Kr.jsx)(Kr.Fragment, {
                                 children: "Yes"
+                            }) : (0, Kr.jsx)(Kr.Fragment, {
+                                children: "\u2013"
                             })
                         }), (0, Kr.jsx)("td", {
                             style: la,
                             children: (0, Kr.jsx)("span", {
                                 onClick: function() {
-                                    return r = t.function, n("//__functioncacheclear__?name=".concat(r)), void e.refresh();
-                                    var r
+                                    return t = n.name, r("//__functioncacheclear__?name=".concat(t)), void e.refresh();
+                                    var t
                                 },
                                 className: "pointer",
                                 children: "Clear"
                             })
                         })]
                     })
                 })
@@ -51389,14 +51417,15 @@
             fa = function(e) {
                 var n = Xi("//__functioncache__"),
                     r = ua(),
                     o = a((0, t.useState)(!1), 2),
                     i = o[0],
                     s = o[1],
                     u = Ye(Ye({}, la), {}, {
+                        verticalAlign: "bottom",
                         fontWeight: "bold",
                         textDecoration: "underline"
                     });
 
                 function l() {
                     n.refresh()
                 }
@@ -51439,50 +51468,56 @@
                     }), (0, Kr.jsxs)("div", {
                         className: "box margin",
                         children: [(0, Kr.jsxs)("table", {
                             children: [(0, Kr.jsx)("thead", {
                                 children: (0, Kr.jsxs)("tr", {
                                     children: [(0, Kr.jsx)("td", {
                                         style: u,
-                                        children: "Function"
+                                        children: "Name"
                                     }), (0, Kr.jsx)("td", {
                                         style: u,
                                         children: "Hits"
                                     }), (0, Kr.jsx)("td", {
                                         style: u,
                                         children: "Misses"
                                     }), (0, Kr.jsx)("td", {
                                         style: u,
                                         children: "Size"
                                     }), (0, Kr.jsx)("td", {
                                         style: u,
                                         children: "Updated"
                                     }), (0, Kr.jsx)("td", {
                                         style: u,
+                                        children: "Duration"
+                                    }), (0, Kr.jsx)("td", {
+                                        style: u,
                                         children: "Max Size"
                                     }), (0, Kr.jsx)("td", {
                                         style: u,
                                         children: "TTL"
                                     }), (0, Kr.jsx)("td", {
                                         style: u,
                                         children: "TTL None"
-                                    }), (0, Kr.jsx)("td", {
+                                    }), (0, Kr.jsxs)("td", {
+                                        style: u,
+                                        children: ["Null", (0, Kr.jsx)("br", {}), "NoCache"]
+                                    }), (0, Kr.jsxs)("td", {
                                         style: u,
-                                        children: "Cache None"
+                                        children: ["Other", (0, Kr.jsx)("br", {}), "NoCache"]
                                     }), (0, Kr.jsx)("td", {
                                         style: u,
                                         children: "Action"
                                     })]
                                 })
                             }), (0, Kr.jsx)("tbody", {
                                 children: n.map((function(e) {
                                     return (0, Kr.jsx)(da, {
                                         cache: e,
                                         refresh: l
-                                    }, e.function)
+                                    }, e.name)
                                 }))
                             })]
                         }), i && (0, Kr.jsxs)(Kr.Fragment, {
                             children: [(0, Kr.jsx)(ji, {
                                 top: "4pt",
                                 bottom: "4pt"
                             }), (0, Kr.jsx)("pre", {
@@ -59866,15 +59901,15 @@
                                 cursor: "pointer"
                             },
                             children: ["\xa0\xa0", (0, Kr.jsx)("img", {
                                 alt: "Clear Cache",
                                 src: Ut.ClearCache(),
                                 height: "19",
                                 onClick: function() {
-                                    K(zt.Url("/__clearcache__", !1))
+                                    K(zt.Url("/__functioncacheclear__", !1))
                                 }
                             })]
                         }), (0, Kr.jsx)(Mi, {
                             id: "tooltip-info-clear",
                             position: "bottom",
                             size: "small",
                             text: "Click to clear any server-side caches."
```

### Comparing `foursight_core-4.1.0.5b59/foursight_core/route_prefixes.py` & `foursight_core-4.1.0.5b60/foursight_core/route_prefixes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/routes.py` & `foursight_core-4.1.0.5b60/foursight_core/routes.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/run_result.py` & `foursight_core-4.1.0.5b60/foursight_core/run_result.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/s3_connection.py` & `foursight_core-4.1.0.5b60/foursight_core/s3_connection.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/schedule_decorator.py` & `foursight_core-4.1.0.5b60/foursight_core/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/scripts/decrypt_accounts_file.py` & `foursight_core-4.1.0.5b60/foursight_core/scripts/decrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/scripts/encrypt_accounts_file.py` & `foursight_core-4.1.0.5b60/foursight_core/scripts/encrypt_accounts_file.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/sqs_utils.py` & `foursight_core-4.1.0.5b60/foursight_core/sqs_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/stage.py` & `foursight_core-4.1.0.5b60/foursight_core/stage.py`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/templates/base.html` & `foursight_core-4.1.0.5b60/foursight_core/templates/base.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/templates/header.html` & `foursight_core-4.1.0.5b60/foursight_core/templates/header.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/templates/history.html` & `foursight_core-4.1.0.5b60/foursight_core/templates/history.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/templates/info.html` & `foursight_core-4.1.0.5b60/foursight_core/templates/info.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/templates/unused.html` & `foursight_core-4.1.0.5b60/foursight_core/templates/unused.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/templates/user.html` & `foursight_core-4.1.0.5b60/foursight_core/templates/user.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/templates/users.html` & `foursight_core-4.1.0.5b60/foursight_core/templates/users.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/templates/view_checks.html` & `foursight_core-4.1.0.5b60/foursight_core/templates/view_checks.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/foursight_core/templates/view_groups.html` & `foursight_core-4.1.0.5b60/foursight_core/templates/view_groups.html`

 * *Files identical despite different names*

### Comparing `foursight_core-4.1.0.5b59/pyproject.toml` & `foursight_core-4.1.0.5b60/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "foursight-core"
-version = "4.1.0.5b59"
+version = "4.1.0.5b60"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "foursight_core" },
   { include = "checks", from = "foursight_core" },
   { include = "helpers", from = "foursight_core/checks" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.10"
 click = "^7.1.2"
 cron-descriptor = "^1.2.31"
 cryptography = "39.0.2" # Required for AWS Cognito JWT decode (PyJWKClient)
-dcicutils = "7.3.2.1b2"
+dcicutils = "7.4.0"
 elasticsearch = "7.13.4"
 elasticsearch-dsl = "^7.0.0"
 geocoder = "1.38.1"
 gitpython = "^3.1.2"
 google = "^3.0.0"
 google-auth-oauthlib = "^0.7.0"
 google-api-python-client = "^1.12.5"
```

### Comparing `foursight_core-4.1.0.5b59/PKG-INFO` & `foursight_core-4.1.0.5b60/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-core
-Version: 4.1.0.5b59
+Version: 4.1.0.5b60
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: cron-descriptor (>=1.2.31,<2.0.0)
 Requires-Dist: cryptography (==39.0.2)
-Requires-Dist: dcicutils (==7.3.2.1b2)
+Requires-Dist: dcicutils (==7.4.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google (>=3.0.0,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.12.5,<2.0.0)
 Requires-Dist: google-auth-oauthlib (>=0.7.0,<0.8.0)
```

