# Comparing `tmp/simple_openid_connect-0.1.3.tar.gz` & `tmp/simple_openid_connect-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_openid_connect-0.1.3.tar", last modified: Tue Dec  6 21:43:05 2022, max compression
+gzip compressed data, was "simple_openid_connect-0.2.0.tar", last modified: Mon May  1 11:44:44 2023, max compression
```

## Comparing `simple_openid_connect-0.1.3.tar` & `simple_openid_connect-0.2.0.tar`

### file list

```diff
@@ -1,72 +1,76 @@
--rw-r--r--   0        0        0       50 2022-11-30 19:51:24.963258 simple_openid_connect-0.1.3/.gitattributes
--rw-r--r--   0        0        0     1584 2022-12-06 20:47:31.034238 simple_openid_connect-0.1.3/.github/workflows/checks.yml
--rw-r--r--   0        0        0      136 2022-11-30 19:51:24.963258 simple_openid_connect-0.1.3/.gitignore
--rw-r--r--   0        0        0      796 2022-11-15 15:08:25.952456 simple_openid_connect-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      177 2022-11-14 08:52:25.576532 simple_openid_connect-0.1.3/.readthedocs.yaml
--rw-r--r--   0        0        0     1116 2022-11-14 08:52:25.576532 simple_openid_connect-0.1.3/LICENSE
--rw-r--r--   0        0        0     4271 2022-12-06 21:41:09.650967 simple_openid_connect-0.1.3/README.md
--rw-r--r--   0        0        0      679 2022-11-14 08:52:25.576532 simple_openid_connect-0.1.3/docs/Makefile
--rw-r--r--   0        0        0        0 2022-11-14 08:52:25.576532 simple_openid_connect-0.1.3/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2022-11-14 08:52:25.576532 simple_openid_connect-0.1.3/docs/_templates/.gitkeep
--rw-r--r--   0        0        0      320 2022-11-30 20:31:11.336503 simple_openid_connect-0.1.3/docs/api.rst
--rw-r--r--   0        0        0     1790 2022-12-06 20:58:11.090917 simple_openid_connect-0.1.3/docs/conf.py
--rw-r--r--   0        0        0     5429 2022-12-06 21:29:57.730954 simple_openid_connect-0.1.3/docs/django-integration.rst
--rw-r--r--   0        0        0     2615 2022-12-06 21:29:57.730954 simple_openid_connect-0.1.3/docs/drf-integration.rst
--rw-r--r--   0        0        0      708 2022-12-06 21:27:06.240951 simple_openid_connect-0.1.3/docs/index.rst
--rw-r--r--   0        0        0      344 2022-11-30 19:51:24.963258 simple_openid_connect-0.1.3/docs/installation.rst
--rw-r--r--   0        0        0     4868 2022-11-30 19:51:24.963258 simple_openid_connect-0.1.3/docs/usage.rst
--rw-r--r--   0        0        0     2391 2022-12-06 21:41:09.640967 simple_openid_connect-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      211 2022-12-06 20:24:59.410878 simple_openid_connect-0.1.3/requirements.dev.txt
--rw-r--r--   0        0        0      127 2022-12-06 21:42:07.240968 simple_openid_connect-0.1.3/src/simple_openid_connect/__init__.py
--rw-r--r--   0        0        0     4204 2022-12-06 19:55:28.190844 simple_openid_connect-0.1.3/src/simple_openid_connect/base_data.py
--rw-r--r--   0        0        0    10369 2022-12-06 19:54:50.377510 simple_openid_connect-0.1.3/src/simple_openid_connect/client.py
--rw-r--r--   0        0        0     3443 2022-11-15 15:12:28.855780 simple_openid_connect-0.1.3/src/simple_openid_connect/client_authentication.py
--rw-r--r--   0        0        0    56368 2022-12-06 19:54:47.220843 simple_openid_connect-0.1.3/src/simple_openid_connect/data.py
--rw-r--r--   0        0        0     1819 2022-11-30 19:51:24.963258 simple_openid_connect-0.1.3/src/simple_openid_connect/discovery.py
--rw-r--r--   0        0        0     1174 2022-12-06 18:26:48.937407 simple_openid_connect-0.1.3/src/simple_openid_connect/exceptions.py
--rw-r--r--   0        0        0      400 2022-11-14 08:52:25.576532 simple_openid_connect-0.1.3/src/simple_openid_connect/flows/__init__.py
--rw-r--r--   0        0        0     5631 2022-11-15 15:14:46.319109 simple_openid_connect-0.1.3/src/simple_openid_connect/flows/authorization_code_flow/__init__.py
--rw-r--r--   0        0        0     6115 2022-12-06 18:26:48.937407 simple_openid_connect-0.1.3/src/simple_openid_connect/flows/authorization_code_flow/client.py
--rw-r--r--   0        0        0       53 2022-12-06 21:39:15.290965 simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/__init__.py
--rw-r--r--   0        0        0       61 2022-11-30 20:34:02.359830 simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/__init__.py
--rw-r--r--   0        0        0     5468 2022-12-06 18:26:48.937407 simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/apps.py
--rw-r--r--   0        0        0     4555 2022-11-30 22:20:50.619591 simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/decorators.py
--rw-r--r--   0        0        0     2631 2022-11-30 20:23:51.599852 simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-11-17 13:39:34.486695 simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/migrations/__init__.py
--rw-r--r--   0        0        0     5728 2022-12-06 18:26:48.937407 simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/models.py
--rw-r--r--   0        0        0      381 2022-11-30 19:51:24.963258 simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/templates/simple_openid_connect/login_failed.html
--rw-r--r--   0        0        0      729 2022-12-06 19:56:59.000846 simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/urls.py
--rw-r--r--   0        0        0     2338 2022-11-30 21:56:39.196312 simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/user_mapping.py
--rw-r--r--   0        0        0     4177 2022-12-06 20:08:46.087526 simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/views.py
--rw-r--r--   0        0        0      306 2022-12-06 21:33:14.294291 simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/djangorestframework/__init__.py
--rw-r--r--   0        0        0     4648 2022-12-06 21:37:21.100963 simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/djangorestframework/authentication.py
--rw-r--r--   0        0        0      957 2022-12-06 21:38:23.800964 simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py
--rw-r--r--   0        0        0     2531 2022-12-06 21:37:21.094296 simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/djangorestframework/permissions.py
--rw-r--r--   0        0        0      472 2022-11-15 15:12:28.855780 simple_openid_connect-0.1.3/src/simple_openid_connect/jwk.py
--rw-r--r--   0        0        0      621 2022-11-15 15:14:22.569110 simple_openid_connect-0.1.3/src/simple_openid_connect/rp_initiated_logout.py
--rw-r--r--   0        0        0     1509 2022-11-15 13:55:22.862619 simple_openid_connect-0.1.3/src/simple_openid_connect/token_introspection.py
--rw-r--r--   0        0        0     1566 2022-11-15 14:38:56.422522 simple_openid_connect-0.1.3/src/simple_openid_connect/token_refresh.py
--rw-r--r--   0        0        0     1393 2022-11-14 08:52:25.576532 simple_openid_connect-0.1.3/src/simple_openid_connect/userinfo.py
--rw-r--r--   0        0        0      781 2022-11-15 15:12:28.855780 simple_openid_connect-0.1.3/src/simple_openid_connect/utils.py
--rw-r--r--   0        0        0    16938 2022-12-06 19:54:08.124176 simple_openid_connect-0.1.3/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-11-15 16:04:11.782332 simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/__init__.py
--rw-r--r--   0        0        0     2785 2022-11-30 20:03:47.153231 simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/settings.py
--rw-r--r--   0        0        0     2586 2022-12-06 18:35:02.237417 simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/tests/conftest.py
--rw-r--r--   0        0        0     1541 2022-12-06 18:26:49.050741 simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py
--rw-r--r--   0        0        0      633 2022-12-06 19:56:59.000846 simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py
--rw-r--r--   0        0        0     5390 2022-12-06 18:26:49.050741 simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/tests/test_login.py
--rw-r--r--   0        0        0      687 2022-12-06 18:38:00.547420 simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/tests/test_logout.py
--rw-r--r--   0        0        0     1248 2022-11-30 20:03:47.146564 simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/urls.py
--rw-r--r--   0        0        0      639 2022-11-30 20:04:38.756562 simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/views.py
--rw-r--r--   0        0        0      415 2022-11-15 16:27:32.405613 simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/wsgi.py
--rwxr-xr-x   0        0        0      675 2022-11-15 16:27:32.408946 simple_openid_connect-0.1.3/tests/django_test_project/manage.py
--rw-r--r--   0        0        0     1746 2022-11-30 19:51:24.963258 simple_openid_connect-0.1.3/tests/interactive_tests/conftest.py
--rw-r--r--   0        0        0     2001 2022-12-06 18:26:49.050741 simple_openid_connect-0.1.3/tests/interactive_tests/test_google.py
--rw-r--r--   0        0        0     1668 2022-12-06 18:26:49.057407 simple_openid_connect-0.1.3/tests/test_authorization_code_flow.py
--rw-r--r--   0        0        0     5139 2022-12-06 18:26:49.057407 simple_openid_connect-0.1.3/tests/test_client.py
--rw-r--r--   0        0        0      934 2022-12-06 18:26:49.057407 simple_openid_connect-0.1.3/tests/test_client_auth.py
--rw-r--r--   0        0        0     1541 2022-12-06 18:26:49.057407 simple_openid_connect-0.1.3/tests/test_discovery.py
--rw-r--r--   0        0        0      590 2022-12-06 18:26:49.057407 simple_openid_connect-0.1.3/tests/test_jwk.py
--rw-r--r--   0        0        0     2274 2022-11-14 08:52:25.576532 simple_openid_connect-0.1.3/tests/test_message_encoding.py
--rw-r--r--   0        0        0      581 2022-11-14 08:52:25.576532 simple_openid_connect-0.1.3/tests/test_rp_initiated_logout.py
--rw-r--r--   0        0        0     5584 1970-01-01 00:00:00.000000 simple_openid_connect-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       50 2022-11-30 14:49:54.727128 simple_openid_connect-0.2.0/.gitattributes
+-rw-r--r--   0        0        0     1584 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.0/.github/workflows/checks.yml
+-rw-r--r--   0        0        0      136 2022-11-24 12:36:21.336726 simple_openid_connect-0.2.0/.gitignore
+-rw-r--r--   0        0        0      795 2023-05-01 11:17:06.824014 simple_openid_connect-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      177 2022-11-12 20:14:29.642701 simple_openid_connect-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      298 2023-05-01 11:41:49.264155 simple_openid_connect-0.2.0/DEVELOPMENT.md
+-rw-r--r--   0        0        0     1116 2022-11-11 18:16:08.603350 simple_openid_connect-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4447 2023-05-01 11:17:53.814441 simple_openid_connect-0.2.0/README.md
+-rw-r--r--   0        0        0      679 2022-11-13 10:21:55.698024 simple_openid_connect-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0        0 2022-11-11 18:16:08.603350 simple_openid_connect-0.2.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2022-11-11 18:16:08.603350 simple_openid_connect-0.2.0/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0      320 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.0/docs/api.rst
+-rw-r--r--   0        0        0     1790 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0     5429 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.0/docs/django-integration.rst
+-rw-r--r--   0        0        0     2615 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.0/docs/drf-integration.rst
+-rw-r--r--   0        0        0      708 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0     1247 2023-05-01 09:33:59.061101 simple_openid_connect-0.2.0/docs/installation.rst
+-rw-r--r--   0        0        0     4868 2022-11-30 16:29:18.260734 simple_openid_connect-0.2.0/docs/usage.rst
+-rw-r--r--   0        0        0     2391 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      211 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.0/requirements.dev.txt
+-rw-r--r--   0        0        0      127 2023-05-01 11:41:57.694232 simple_openid_connect-0.2.0/src/simple_openid_connect/__init__.py
+-rw-r--r--   0        0        0     4204 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.0/src/simple_openid_connect/base_data.py
+-rw-r--r--   0        0        0    10675 2023-05-01 11:18:29.691434 simple_openid_connect-0.2.0/src/simple_openid_connect/client.py
+-rw-r--r--   0        0        0     3443 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.0/src/simple_openid_connect/client_authentication.py
+-rw-r--r--   0        0        0    57231 2023-05-01 11:33:35.079663 simple_openid_connect-0.2.0/src/simple_openid_connect/data.py
+-rw-r--r--   0        0        0     1819 2022-11-30 12:04:05.293339 simple_openid_connect-0.2.0/src/simple_openid_connect/discovery.py
+-rw-r--r--   0        0        0     1174 2022-12-01 11:36:58.020255 simple_openid_connect-0.2.0/src/simple_openid_connect/exceptions.py
+-rw-r--r--   0        0        0      343 2023-05-01 11:17:53.814441 simple_openid_connect-0.2.0/src/simple_openid_connect/flows/__init__.py
+-rw-r--r--   0        0        0     5631 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.0/src/simple_openid_connect/flows/authorization_code_flow/__init__.py
+-rw-r--r--   0        0        0     6115 2022-12-01 11:36:58.243589 simple_openid_connect-0.2.0/src/simple_openid_connect/flows/authorization_code_flow/client.py
+-rw-r--r--   0        0        0     2208 2023-05-01 11:18:30.258106 simple_openid_connect-0.2.0/src/simple_openid_connect/flows/direct_access_grant/__init__.py
+-rw-r--r--   0        0        0     1583 2023-05-01 11:18:30.258106 simple_openid_connect-0.2.0/src/simple_openid_connect/flows/direct_access_grant/client.py
+-rw-r--r--   0        0        0       53 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/__init__.py
+-rw-r--r--   0        0        0       61 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/__init__.py
+-rw-r--r--   0        0        0     5467 2023-05-01 11:22:04.083382 simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/apps.py
+-rw-r--r--   0        0        0     4555 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/decorators.py
+-rw-r--r--   0        0        0     2630 2023-05-01 11:22:04.076716 simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/migrations/__init__.py
+-rw-r--r--   0        0        0     5728 2022-12-01 11:42:37.006937 simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/models.py
+-rw-r--r--   0        0        0      381 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/templates/simple_openid_connect/login_failed.html
+-rw-r--r--   0        0        0      729 2022-12-08 12:24:29.349860 simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/urls.py
+-rw-r--r--   0        0        0     2338 2022-12-01 10:05:47.886671 simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/user_mapping.py
+-rw-r--r--   0        0        0     4177 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/views.py
+-rw-r--r--   0        0        0      306 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/djangorestframework/__init__.py
+-rw-r--r--   0        0        0     4648 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/djangorestframework/authentication.py
+-rw-r--r--   0        0        0      957 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py
+-rw-r--r--   0        0        0     2531 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/djangorestframework/permissions.py
+-rw-r--r--   0        0        0      472 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.0/src/simple_openid_connect/jwk.py
+-rw-r--r--   0        0        0      621 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.0/src/simple_openid_connect/rp_initiated_logout.py
+-rw-r--r--   0        0        0     1509 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.0/src/simple_openid_connect/token_introspection.py
+-rw-r--r--   0        0        0     1566 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.0/src/simple_openid_connect/token_refresh.py
+-rw-r--r--   0        0        0     1393 2022-11-12 19:48:31.467498 simple_openid_connect-0.2.0/src/simple_openid_connect/userinfo.py
+-rw-r--r--   0        0        0      781 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.0/src/simple_openid_connect/utils.py
+-rw-r--r--   0        0        0    16938 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/__init__.py
+-rw-r--r--   0        0        0     2785 2022-12-01 10:05:47.890004 simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/settings.py
+-rw-r--r--   0        0        0     2586 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/tests/conftest.py
+-rw-r--r--   0        0        0     1541 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py
+-rw-r--r--   0        0        0      633 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py
+-rw-r--r--   0        0        0     5390 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/tests/test_login.py
+-rw-r--r--   0        0        0      687 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/tests/test_logout.py
+-rw-r--r--   0        0        0     1248 2022-12-01 10:05:47.890004 simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/urls.py
+-rw-r--r--   0        0        0      639 2022-12-01 10:05:47.890004 simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/views.py
+-rw-r--r--   0        0        0      415 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/wsgi.py
+-rwxr-xr-x   0        0        0      675 2022-11-16 07:19:49.333600 simple_openid_connect-0.2.0/tests/django_test_project/manage.py
+-rw-r--r--   0        0        0     1746 2022-11-30 13:30:16.836909 simple_openid_connect-0.2.0/tests/interactive_tests/conftest.py
+-rw-r--r--   0        0        0     2001 2022-12-08 12:24:29.353193 simple_openid_connect-0.2.0/tests/interactive_tests/test_google.py
+-rw-r--r--   0        0        0     1668 2022-12-08 12:24:29.366526 simple_openid_connect-0.2.0/tests/test_authorization_code_flow.py
+-rw-r--r--   0        0        0     5139 2022-12-08 12:24:29.366526 simple_openid_connect-0.2.0/tests/test_client.py
+-rw-r--r--   0        0        0      934 2022-12-08 12:24:29.366526 simple_openid_connect-0.2.0/tests/test_client_auth.py
+-rw-r--r--   0        0        0     1378 2023-05-01 11:18:29.554766 simple_openid_connect-0.2.0/tests/test_direct_access_grant.py
+-rw-r--r--   0        0        0     1541 2022-12-08 12:24:29.366526 simple_openid_connect-0.2.0/tests/test_discovery.py
+-rw-r--r--   0        0        0      590 2022-12-08 12:24:29.366526 simple_openid_connect-0.2.0/tests/test_jwk.py
+-rw-r--r--   0        0        0     2274 2022-11-13 10:28:27.455234 simple_openid_connect-0.2.0/tests/test_message_encoding.py
+-rw-r--r--   0        0        0      581 2022-11-12 19:48:31.434164 simple_openid_connect-0.2.0/tests/test_rp_initiated_logout.py
+-rw-r--r--   0        0        0     5760 1970-01-01 00:00:00.000000 simple_openid_connect-0.2.0/PKG-INFO
```

### Comparing `simple_openid_connect-0.1.3/.github/workflows/checks.yml` & `simple_openid_connect-0.2.0/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/.pre-commit-config.yaml` & `simple_openid_connect-0.2.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 exclude: ^.*/secrets.yml$
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v3.2.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
         args:
           - "--profile=black"
   - repo: local
     hooks:
       - id: mypy
```

### Comparing `simple_openid_connect-0.1.3/LICENSE` & `simple_openid_connect-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/README.md` & `simple_openid_connect-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -29,29 +29,30 @@
 
   Tell the user about function requirements clearly but don't try any fancy internal persistence or caching mechanisms that will only fail in different usage scenarios.
   Instead, abstract the underlying OpenID protocol into usable, clear functions but nothing more.
 
 
 ## Framework Integrations
 
-| Name                                                            | Integration Docs                                                                                   | Supported Versions     |
-|-----------------------------------------------------------------|----------------------------------------------------------------------------------------------------|------------------------|
-| [Django](https://www.djangoproject.com/)                        | [Integration Docs](https://simple-openid-connect.readthedocs.io/en/stable/django-integration.html) | `v3.2`, `v4.0`, `v4.1` |
-| [Django-Rest-Framework](https://www.django-rest-framework.org/) | [Integration Docs](https://simple-openid-connect.readthedocs.io/en/stable/drf-integration.html)    | `v3.13`, `v3.14`       |
+| Name                                                            | Package Feature       | Integration Docs                                                                                   | Supported Versions     |
+|-----------------------------------------------------------------|-----------------------|----------------------------------------------------------------------------------------------------|------------------------|
+| [Django](https://www.djangoproject.com/)                        | `django`              | [Integration Docs](https://simple-openid-connect.readthedocs.io/en/stable/django-integration.html) | `v3.2`, `v4.0`, `v4.1` |
+| [Django-Rest-Framework](https://www.django-rest-framework.org/) | `djangorestframework` | [Integration Docs](https://simple-openid-connect.readthedocs.io/en/stable/drf-integration.html)    | `v3.13`, `v3.14`       |
 
 
 
 ## Supported OpenID Specs
 
 The list of [OpenID specifications](https://openid.net/developers/specs/) can be found on the official website.
 
 - (✔️) Partial [OpenID Connect Core 1.0](https://openid.net/specs/openid-connect-core-1_0.html)
 
   Only the following flows and features are implemented:
   - ✔️ Authorization Code Flow
+  - ✔️ Direct Access Grant (or *Resource Owner Password Credentials Grant*)
   - ✔️ `client_secret_basic` client authentication
   - ✔️ `none` client authentication
   - ✔️ Query String serialization and parsing
   - ✔️ ID Token handling (parsing + validation)
   - ✔️ Using refresh tokens
   - ✔️ Retrieving userinfo
   - ❌ Implicit Flow
```

### Comparing `simple_openid_connect-0.1.3/docs/Makefile` & `simple_openid_connect-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/docs/conf.py` & `simple_openid_connect-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/docs/django-integration.rst` & `simple_openid_connect-0.2.0/docs/django-integration.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/docs/drf-integration.rst` & `simple_openid_connect-0.2.0/docs/drf-integration.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/docs/index.rst` & `simple_openid_connect-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/docs/usage.rst` & `simple_openid_connect-0.2.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/pyproject.toml` & `simple_openid_connect-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/base_data.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/base_data.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/client.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
     UserinfoSuccessResponse,
 )
 from simple_openid_connect.discovery import discover_configuration_from_issuer
 from simple_openid_connect.exceptions import UnsupportedByProviderError
 from simple_openid_connect.flows.authorization_code_flow.client import (
     AuthorizationCodeFlowClient,
 )
+from simple_openid_connect.flows.direct_access_grant.client import (
+    DirectAccessGrantClient,
+)
 
 Self = TypeVar("Self", bound="OpenidClient")
 
 
 class OpenidClient:
     """
     A more contiguous client implementation of the Openid-Connect protocol that offers simpler APIs at the cost of losing some flexibility.
@@ -48,26 +51,30 @@
     provider_keys: List[JWK]
     client_auth: ClientAuthenticationMethod
     scope: str
 
     authorization_code_flow: AuthorizationCodeFlowClient
     "*authorization code flow* related functionality"
 
+    direct_access_grant: DirectAccessGrantClient
+    "*Direct Access Grant* (or *Resource Owner Password Credentials Grant*) functionality"
+
     def __init__(
         self,
         provider_config: ProviderMetadata,
         provider_keys: List[JWK],
         authentication_redirect_uri: Optional[str],
         client_id: str,
         client_secret: Optional[str] = None,
         scope: str = "openid",
     ):
         self.provider_config = provider_config
         self.provider_keys = provider_keys
         self.authorization_code_flow = AuthorizationCodeFlowClient(self)
+        self.direct_access_grant = DirectAccessGrantClient(self)
         self.scope = scope
         self.authentication_redirect_uri = authentication_redirect_uri
 
         if client_secret is None:
             self.client_auth = NoneAuth(client_id)
         else:
             if (
```

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/client_authentication.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/client_authentication.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/data.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     auth_time: Optional[int]
     "Time when the End-User authentication occurred Its value is a JSON number representing the number of seconds from 1970-01-01T0:0:0Z as measured in UTC until the date/time When a max_age request is made or when auth_time is requested as an Essential Claim, then this Claim is REQUIRED; otherwise, its inclusion is OPTIONAL (The auth_time Claim semantically corresponds to the OpenID 2.0 PAPE [OpenID.PAPE] auth_time response parameter.)"
 
     nonce: Optional[str]
     "String value used to associate a Client session with an ID Token, and to mitigate replay attacks The value is passed through unmodified from the Authentication Request to the ID Token If present in the ID Token, Clients MUST verify that the nonce Claim Value is equal to the value of the nonce parameter sent in the Authentication Request If present in the Authentication Request, Authorization Servers MUST include a nonce Claim in the ID Token with the Claim Value being the nonce value sent in the Authentication Request Authorization Servers SHOULD perform no other processing on nonce values used The nonce value is a case sensitive string. "
 
     acr: Optional[str]
-    "OPTIONAL. Authentication Context Class Reference String specifying an Authentication Context Class Reference value that identifies the Authentication Context Class that the authentication performed satisfied. " 'The value "0" indicates the End-User authentication did not meet the requirements of ISO/IEC 29115 [ISO29115] level 1. ' 'Authentication using a long-lived browser cookie, for instance, is one example where the use of "level 0" is appropriate. ' "Authentications with level 0 SHOULD NOT be used to authorize access to any resource of any monetary value (This corresponds to the OpenID 2.0 PAPE [OpenID.PAPE] nist_auth_level 0.)  An absolute URI or an RFC 6711 [RFC6711] registered name SHOULD be used as the acr value; registered names MUST NOT be used with a different meaning than that which is registered Parties using this claim will need to agree upon the meanings of the values used, which may be context-specific The acr value is a case sensitive string."
+    "OPTIONAL. Authentication Context Class Reference String specifying an Authentication Context Class Reference value that identifies the Authentication Context Class that the authentication performed satisfied. The value '0' indicates the End-User authentication did not meet the requirements of ISO/IEC 29115 [ISO29115] level 1. Authentication using a long-lived browser cookie, for instance, is one example where the use of 'level 0' is appropriate. Authentications with level 0 SHOULD NOT be used to authorize access to any resource of any monetary value (This corresponds to the OpenID 2.0 PAPE [OpenID.PAPE] nist_auth_level 0.)  An absolute URI or an RFC 6711 [RFC6711] registered name SHOULD be used as the acr value; registered names MUST NOT be used with a different meaning than that which is registered Parties using this claim will need to agree upon the meanings of the values used, which may be context-specific The acr value is a case sensitive string."
 
     amr: Optional[List[str]]
     "OPTIONAL. Authentication Methods References JSON array of strings that are identifiers for authentication methods used in the authentication For instance, values might indicate that both password and OTP authentication methods were used The definition of particular values to be used in the amr Claim is beyond the scope of this specification Parties using this claim will need to agree upon the meanings of the values used, which may be context-specific The amr value is an array of case sensitive strings."
 
     azp: Optional[str]
     "OPTIONAL. Authorized party - the party to which the ID Token was issued If present, it MUST contain the OAuth 2.0 Client ID of this party This Claim is only needed when the ID Token has a single audience value and that audience is different than the authorized party It MAY be included even when the authorized party is the same as the sole audience The azp value is a case sensitive string containing a StringOrURI value."
 
@@ -347,42 +347,42 @@
 
     client_id: str
     "REQUIRED. OAuth 2.0 Client Identifier valid at the Authorization Server."
 
     redirect_uri: str
     "REQUIRED. Redirection URI to which the response will be sent This URI MUST exactly match one of the Redirection URI values for the Client pre-registered at the OpenID Provider When using this flow, the Redirection URI SHOULD use the https scheme; however, it MAY use the http scheme, provided that the Client Type is confidential, as defined in Section 2.1 of OAuth 2.0, and provided the OP allows the use of http Redirection URIs in this case The Redirection URI MAY use an alternate scheme, such as one that is intended to identify a callback into a native application."
 
-    state: Optional[str]
+    state: Optional[str] = None
     "RECOMMENDED. Opaque value used to maintain state between the request and the callback Typically, Cross-Site Request Forgery (CSRF, XSRF) mitigation is done by cryptographically binding the value of this parameter with a browser cookie."
 
-    response_mode: Optional[str]
+    response_mode: Optional[str] = None
     "OPTIONAL. Informs the Authorization Server of the mechanism to be used for returning parameters from the Authorization Endpoint. This use of this parameter is NOT RECOMMENDED when the Response Mode that would be requested is the default mode specified for the Response Type."
 
-    nonce: Optional[str]
+    nonce: Optional[str] = None
     "OPTIONAL. String value used to associate a Client session with an ID Token, and to mitigate replay attacks The value is passed through unmodified from the Authentication Request to the ID Token Sufficient entropy MUST be present in the nonce values used to prevent attackers from guessing values."
 
-    display: Optional[List[str]]
+    display: Optional[List[str]] = None
     'OPTIONAL. Space delimited, case sensitive list of ASCII string values that specifies whether the Authorization Server prompts the End-User for reauthentication and consent. The defined values are: "page", "popup", "touch" and "wap"'
 
-    prompt: Optional[List[str]]
+    prompt: Optional[List[str]] = None
     'OPTIONAL. Space delimited, case sensitive list of ASCII string values that specifies whether the Authorization Server prompts the End-User for reauthentication and consent. The defined values are: "none", "login", "consent" and "select_account".'
 
-    max_age: Optional[int]
+    max_age: Optional[int] = None
     "OPTIONAL. Maximum Authentication Age Specifies the allowable elapsed time in seconds since the last time the End-User was actively authenticated by the OP If the elapsed time is greater than this value, the OP MUST attempt to actively re-authenticate the End-User When max_age is used, the ID Token returned MUST include an auth_time Claim Value."
 
-    ui_locales: Optional[List[str]]
+    ui_locales: Optional[List[str]] = None
     "OPTIONAL. End-User's preferred languages and scripts for the user interface, represented as a space-separated list of BCP47 [RFC5646] language tag values, ordered by preference. " 'For instance, the value "fr-CA fr en" represents a preference for French as spoken in Canada, then French (without a region designation), followed by English (without a region designation). ' "An error SHOULD NOT result if some or all of the requested locales are not supported by the OpenID Provider."
 
-    id_token_hint: Optional[str]
+    id_token_hint: Optional[str] = None
     "OPTIONAL. ID Token previously issued by the Authorization Server being passed as a hint about the End-User's current or past authenticated session with the Client If the End-User identified by the ID Token is logged in or is logged in by the request, then the Authorization Server returns a positive response; otherwise, it SHOULD return an error, such as login_required When possible, an id_token_hint SHOULD be present when prompt=none is used and an invalid_request error MAY be returned if it is not; however, the server SHOULD respond successfully when possible, even if it is not present The Authorization Server need not be listed as an audience of the ID Token when it is used as an id_token_hint value. "
 
-    login_hint: Optional[str]
+    login_hint: Optional[str] = None
     "OPTIONAL. Hint to the Authorization Server about the login identifier the End-User might use to log in (if necessary) This hint can be used by an RP if it first asks the End-User for their e-mail address (or other identifier) and then wants to pass that value as a hint to the discovered authorization service It is RECOMMENDED that the hint value match the value used for discovery (which is not supported by this library) This value MAY also be a phone number in the format specified for the `phone_number` Claim The use of this parameter is left to the OP's discretion."
 
-    acr_values: Optional[List[str]]
+    acr_values: Optional[List[str]] = None
     "OPTIONAL. Requested Authentication Context Class Reference values Space-separated string that specifies the acr values that the Authorization Server is being requested to use for processing this Authentication Request, with the values appearing in order of preference The Authentication Context Class satisfied by the authentication performed is returned as the acr Claim Value, as specified in Section 2 The acr Claim is requested as a Voluntary Claim by this parameter."
 
 
 class AuthenticationSuccessResponse(OpenidBaseModel):
     """
     A response that is sent by the Authorization Server if a previous :class:`.AuthenticationRequest` could successfully
     be parsed and handled.
@@ -488,28 +488,37 @@
 
     This request MUST be sent to the token endpoint using POST with "application/x-www-form-urlencoded" body.
     """
 
     class Config:
         extra = Extra.allow
 
-    grant_type: Union[Literal["authorization_code", "refresh_token"], str]
+    grant_type: Union[Literal["authorization_code", "refresh_token", "password"], str]
     "REQUIRED. Which type of token exchange this request is."
 
-    code: Optional[str]
+    code: Optional[str] = None
     "REQUIRED, if grant type is 'code', otherwise optional. The authorization code received from the authorization server."
 
-    redirect_uri: Optional[str]
+    redirect_uri: Optional[str] = None
     "REQUIRED, if grant_Type is 'code', otherwise not needed. Must be identical to the value that was included in the :data:`AuthenticationRequest <AuthenticationRequest.redirect_uri>`."
 
-    client_id: Optional[str]
+    client_id: Optional[str] = None
     "REQUIRED, if the client is not authenticating with the authorization server. Basically, confidential clients don't need to include it but others do."
 
-    refresh_token: Optional[str]
-    "REQUIRED. The refresh token issued to the client."
+    refresh_token: Optional[str] = None
+    "REQUIRED, if grant type is 'refresh_token'. The refresh token issued to the client."
+
+    username: Optional[str] = None
+    "REQUIRED, if grant type is 'password'"
+
+    password: Optional[str] = None
+    "REQUIRED, if grant type is 'password'"
+
+    scope: Optional[str] = None
+    "REQUIRED, if grant type is 'password'. The scope requested by the application"
 
     @root_validator(skip_on_failure=True)
     def _validate_required_based_on_grant_type(
         cls, values: Mapping[str, Any]
     ) -> Mapping[str, Any]:
         if values["grant_type"] == "authorization_code":
             assert (
@@ -518,14 +527,24 @@
             assert (
                 values["redirect_uri"] is not None
             ), "redirect_uri is required when grant_type is 'authorization_code'"
         elif values["grant_type"] == "refresh_token":
             assert (
                 values["refresh_token"] is not None
             ), "refresh_token is required when grant_type is 'refresh_token'"
+        elif values["grant_type"] == "password":
+            assert (
+                values["username"] is not None
+            ), "username is required when grant_type is 'password'"
+            assert (
+                values["password"] is not None
+            ), "password is required when grant_type is 'password'"
+            assert (
+                values["scope"] is not None
+            ), "scope is required when grant_type is 'password'"
 
         return values
 
 
 class TokenSuccessResponse(OpenidBaseModel):
     """
     After receiving and validating a valid and authorized :class:`TokenRequest <TokenRequest>` from the Client, the Authorization Server returns a successful response that includes an ID Token and an Access Token
```

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/discovery.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/discovery.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/exceptions.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/exceptions.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/flows/authorization_code_flow/__init__.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/flows/authorization_code_flow/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/flows/authorization_code_flow/client.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/flows/authorization_code_flow/client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/apps.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/apps.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,14 @@
             In any case, if the `OPENID_BASE_URI` setting is set, it will be used instead.
 
         :raises ImproperlyConfigured: when no *own_base_uri* is given and the `OPENID_BASE_URI` is also None
         """
         # use a cached client instance if one exists or create a new one if not
         client = cache.get("openid_client")  # type: OpenidClient
         if client is None:
-
             # determine base_uri of this app
             if self.safe_settings.OPENID_REDIRECT_URI is not None:
                 if self.safe_settings.OPENID_BASE_URI is not None:
                     own_base_uri = self.safe_settings.OPENID_BASE_URI
                 else:
                     if own_base_uri is None:
                         raise ImproperlyConfigured(
```

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/decorators.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/decorators.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/migrations/0001_initial.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
 
     operations = [
```

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/models.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/models.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/urls.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/urls.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/user_mapping.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/user_mapping.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/django/views.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/django/views.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/djangorestframework/authentication.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/djangorestframework/authentication.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/integrations/djangorestframework/permissions.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/integrations/djangorestframework/permissions.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/rp_initiated_logout.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/rp_initiated_logout.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/token_introspection.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/token_introspection.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/token_refresh.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/token_refresh.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/userinfo.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/userinfo.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/src/simple_openid_connect/utils.py` & `simple_openid_connect-0.2.0/src/simple_openid_connect/utils.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/conftest.py` & `simple_openid_connect-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/settings.py` & `simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/settings.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/tests/conftest.py` & `simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py` & `simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py` & `simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/tests/test_login.py` & `simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/tests/test_logout.py` & `simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/tests/test_logout.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/urls.py` & `simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/urls.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/django_test_project/django_test_project/views.py` & `simple_openid_connect-0.2.0/tests/django_test_project/django_test_project/views.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/django_test_project/manage.py` & `simple_openid_connect-0.2.0/tests/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/interactive_tests/conftest.py` & `simple_openid_connect-0.2.0/tests/interactive_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/interactive_tests/test_google.py` & `simple_openid_connect-0.2.0/tests/interactive_tests/test_google.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/test_authorization_code_flow.py` & `simple_openid_connect-0.2.0/tests/test_authorization_code_flow.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/test_client.py` & `simple_openid_connect-0.2.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/test_client_auth.py` & `simple_openid_connect-0.2.0/tests/test_client_auth.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/test_discovery.py` & `simple_openid_connect-0.2.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/test_jwk.py` & `simple_openid_connect-0.2.0/tests/test_jwk.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/test_message_encoding.py` & `simple_openid_connect-0.2.0/tests/test_message_encoding.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/tests/test_rp_initiated_logout.py` & `simple_openid_connect-0.2.0/tests/test_rp_initiated_logout.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.1.3/PKG-INFO` & `simple_openid_connect-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_openid_connect
-Version: 0.1.3
+Version: 0.2.0
 Summary: Simple and opinionated OpenID-Connect relying party and resource server implementation
 Author-email: Finn-Thorben Sell <dev@finn-thorben.me>
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
@@ -60,29 +60,30 @@
 
   Tell the user about function requirements clearly but don't try any fancy internal persistence or caching mechanisms that will only fail in different usage scenarios.
   Instead, abstract the underlying OpenID protocol into usable, clear functions but nothing more.
 
 
 ## Framework Integrations
 
-| Name                                                            | Integration Docs                                                                                   | Supported Versions     |
-|-----------------------------------------------------------------|----------------------------------------------------------------------------------------------------|------------------------|
-| [Django](https://www.djangoproject.com/)                        | [Integration Docs](https://simple-openid-connect.readthedocs.io/en/stable/django-integration.html) | `v3.2`, `v4.0`, `v4.1` |
-| [Django-Rest-Framework](https://www.django-rest-framework.org/) | [Integration Docs](https://simple-openid-connect.readthedocs.io/en/stable/drf-integration.html)    | `v3.13`, `v3.14`       |
+| Name                                                            | Package Feature       | Integration Docs                                                                                   | Supported Versions     |
+|-----------------------------------------------------------------|-----------------------|----------------------------------------------------------------------------------------------------|------------------------|
+| [Django](https://www.djangoproject.com/)                        | `django`              | [Integration Docs](https://simple-openid-connect.readthedocs.io/en/stable/django-integration.html) | `v3.2`, `v4.0`, `v4.1` |
+| [Django-Rest-Framework](https://www.django-rest-framework.org/) | `djangorestframework` | [Integration Docs](https://simple-openid-connect.readthedocs.io/en/stable/drf-integration.html)    | `v3.13`, `v3.14`       |
 
 
 
 ## Supported OpenID Specs
 
 The list of [OpenID specifications](https://openid.net/developers/specs/) can be found on the official website.
 
 - (✔️) Partial [OpenID Connect Core 1.0](https://openid.net/specs/openid-connect-core-1_0.html)
 
   Only the following flows and features are implemented:
   - ✔️ Authorization Code Flow
+  - ✔️ Direct Access Grant (or *Resource Owner Password Credentials Grant*)
   - ✔️ `client_secret_basic` client authentication
   - ✔️ `none` client authentication
   - ✔️ Query String serialization and parsing
   - ✔️ ID Token handling (parsing + validation)
   - ✔️ Using refresh tokens
   - ✔️ Retrieving userinfo
   - ❌ Implicit Flow
```

