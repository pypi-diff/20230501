# Comparing `tmp/django-axes-6.0.0b2.tar.gz` & `tmp/django-axes-6.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-axes-6.0.0b2.tar", last modified: Fri Apr 28 11:25:29 2023, max compression
+gzip compressed data, was "django-axes-6.0.0b3.tar", last modified: Mon May  1 18:32:38 2023, max compression
```

## Comparing `django-axes-6.0.0b2.tar` & `django-axes-6.0.0b3.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.720070 django-axes-6.0.0b2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.700070 django-axes-6.0.0b2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.700070 django-axes-6.0.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/.prospector.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    31470 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    35736 2023-04-28 11:25:29.720070 django-axes-6.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.700070 django-axes-6.0.0b2/axes/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.704070 django-axes-6.0.0b2/axes/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/handlers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/handlers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/handlers/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/handlers/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/handlers/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20380 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.692070 django-axes-6.0.0b2/axes/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.692070 django-axes-6.0.0b2/axes/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.704070 django-axes-6.0.0b2/axes/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.692070 django-axes-6.0.0b2/axes/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.708070 django-axes-6.0.0b2/axes/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.692070 django-axes-6.0.0b2/axes/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.708070 django-axes-6.0.0b2/axes/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.692070 django-axes-6.0.0b2/axes/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.708070 django-axes-6.0.0b2/axes/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.692070 django-axes-6.0.0b2/axes/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.708070 django-axes-6.0.0b2/axes/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.708070 django-axes-6.0.0b2/axes/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.708070 django-axes-6.0.0b2/axes/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/commands/axes_list_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/commands/axes_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/commands/axes_reset_failure_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/commands/axes_reset_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/commands/axes_reset_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/management/commands/axes_reset_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.712070 django-axes-6.0.0b2/axes/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0002_auto_20151217_2044.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0003_auto_20160322_0929.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0004_auto_20181024_1538.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0005_remove_accessattempt_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0006_remove_accesslog_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0007_alter_accessattempt_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/0008_accessfailurelog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/axes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.712070 django-axes-6.0.0b2/django_axes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35736 2023-04-28 11:25:29.000000 django-axes-6.0.0b2/django_axes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-28 11:25:29.000000 django-axes-6.0.0b2/django_axes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:25:29.000000 django-axes-6.0.0b2/django_axes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:25:29.000000 django-axes-6.0.0b2/django_axes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-28 11:25:29.000000 django-axes-6.0.0b2/django_axes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 11:25:29.000000 django-axes-6.0.0b2/django_axes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.716070 django-axes-6.0.0b2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/10_changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/1_requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/2_installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/3_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)    63233 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/4_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/5_customization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/6_integration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/7_architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/8_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/9_contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.716070 django-axes-6.0.0b2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/images/flow.png
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/requirements-qa.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:25:29.720070 django-axes-6.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:29.720070 django-axes-6.0.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_failures.py
--rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    31928 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    29839 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 11:25:13.000000 django-axes-6.0.0b2/tests/urls_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.910358 django-axes-6.0.0b3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.878357 django-axes-6.0.0b3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.882357 django-axes-6.0.0b3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/.prospector.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    31599 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    35865 2023-05-01 18:32:38.910358 django-axes-6.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.886357 django-axes-6.0.0b3/axes/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.886357 django-axes-6.0.0b3/axes/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/handlers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/handlers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/handlers/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/handlers/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/handlers/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20418 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.870357 django-axes-6.0.0b3/axes/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.870357 django-axes-6.0.0b3/axes/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.890357 django-axes-6.0.0b3/axes/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.870357 django-axes-6.0.0b3/axes/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.890357 django-axes-6.0.0b3/axes/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.870357 django-axes-6.0.0b3/axes/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.890357 django-axes-6.0.0b3/axes/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.870357 django-axes-6.0.0b3/axes/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.890357 django-axes-6.0.0b3/axes/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.870357 django-axes-6.0.0b3/axes/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.890357 django-axes-6.0.0b3/axes/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.890357 django-axes-6.0.0b3/axes/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.894358 django-axes-6.0.0b3/axes/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/management/commands/axes_list_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/management/commands/axes_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/management/commands/axes_reset_failure_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/management/commands/axes_reset_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/management/commands/axes_reset_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/management/commands/axes_reset_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.898357 django-axes-6.0.0b3/axes/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/migrations/0002_auto_20151217_2044.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/migrations/0003_auto_20160322_0929.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/migrations/0004_auto_20181024_1538.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/migrations/0005_remove_accessattempt_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/migrations/0006_remove_accesslog_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/migrations/0007_alter_accessattempt_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/migrations/0008_accessfailurelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/axes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.898357 django-axes-6.0.0b3/django_axes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35865 2023-05-01 18:32:38.000000 django-axes-6.0.0b3/django_axes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-01 18:32:38.000000 django-axes-6.0.0b3/django_axes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:32:38.000000 django-axes-6.0.0b3/django_axes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:32:38.000000 django-axes-6.0.0b3/django_axes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-01 18:32:38.000000 django-axes-6.0.0b3/django_axes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-01 18:32:38.000000 django-axes-6.0.0b3/django_axes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.902358 django-axes-6.0.0b3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/docs/10_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/docs/1_requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/docs/2_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/docs/3_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    63233 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/docs/4_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/docs/5_customization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/docs/6_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/docs/7_architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/docs/8_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/docs/9_contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.902358 django-axes-6.0.0b3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/docs/images/flow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/requirements-qa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:32:38.910358 django-axes-6.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:38.910358 django-axes-6.0.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/test_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/test_failures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31936 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29839 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 18:32:19.000000 django-axes-6.0.0b3/tests/urls_empty.py
```

### Comparing `django-axes-6.0.0b2/.github/workflows/codeql.yml` & `django-axes-6.0.0b3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/.github/workflows/release.yml` & `django-axes-6.0.0b3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/.github/workflows/test.yml` & `django-axes-6.0.0b3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/CHANGES.rst` & `django-axes-6.0.0b3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 
 Changes
 =======
 
 
+6.0.0b3 (2023-05-01)
+--------------------
+
+- Use Django ``cache.incr`` API for atomic cached failure counting
+  [hirotasoshu, aleksihakli]
+
+
 6.0.0b2 (2023-04-28)
 --------------------
 
 - Make ``django-ipware`` an optional dependency. Install it with e.g. ``pip install django-axes[ipware]`` package and extras specifier. [aleksihakli]
 - Deprecate and rename old configuration flags. Old flags will be removed in or after version ``6.1``. [aleksihakli]
-   * ``AXES_PROXY_ORDER`` is now ``AXES_IPWARE_PROXY_ORDER``, 
-   * ``AXES_PROXY_COUNT`` is now ``AXES_IPWARE_PROXY_COUNT``, 
-   * ``AXES_IPWARE_PROXY_TRUSTED_IPS`` is now ``AXES_PROXY_TRUSTED_IPS``, and 
-   * ``AXES_IPWARE_META_PRECEDENCE_ORDER`` is now ``AXES_META_PRECEDENCE_ORDER``. 
+   * ``AXES_PROXY_ORDER`` is now ``AXES_IPWARE_PROXY_ORDER``,
+   * ``AXES_PROXY_COUNT`` is now ``AXES_IPWARE_PROXY_COUNT``,
+   * ``AXES_PROXY_TRUSTED_IPS`` is now ``AXES_IPWARE_PROXY_TRUSTED_IPS``, and
+   * ``AXES_META_PRECEDENCE_ORDER`` is now ``AXES_IPWARE_META_PRECEDENCE_ORDER``.
 
 
 6.0.0b1 (2023-04-25)
 --------------------
 
 - Set 429 as the default lockout response code. [hirotasoshu]
 
@@ -110,15 +117,15 @@
 - Add support for float or partial hours for ``AXES_COOLOFF_TIME``.
   [hramezani]
 
 
 5.32.0 (2022-04-08)
 -------------------
 
-- Add support for persistent failure logging
+- Add support for persistent logging
   where failed login attempts are persisted in the database
   until a specific threshold is reached.
   [p1-gdd]
 - Add support for not resetting login times when users
   try to login during the lockout cooloff period.
   [antoine-42]
```

### Comparing `django-axes-6.0.0b2/CODE_OF_CONDUCT.md` & `django-axes-6.0.0b3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/CONTRIBUTING.rst` & `django-axes-6.0.0b3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/LICENSE` & `django-axes-6.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/PKG-INFO` & `django-axes-6.0.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.0b2
+Version: 6.0.0b3
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -124,23 +124,30 @@
 See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
 
 Changes
 =======
 
 
+6.0.0b3 (2023-05-01)
+--------------------
+
+- Use Django ``cache.incr`` API for atomic cached failure counting
+  [hirotasoshu, aleksihakli]
+
+
 6.0.0b2 (2023-04-28)
 --------------------
 
 - Make ``django-ipware`` an optional dependency. Install it with e.g. ``pip install django-axes[ipware]`` package and extras specifier. [aleksihakli]
 - Deprecate and rename old configuration flags. Old flags will be removed in or after version ``6.1``. [aleksihakli]
-   * ``AXES_PROXY_ORDER`` is now ``AXES_IPWARE_PROXY_ORDER``, 
-   * ``AXES_PROXY_COUNT`` is now ``AXES_IPWARE_PROXY_COUNT``, 
-   * ``AXES_IPWARE_PROXY_TRUSTED_IPS`` is now ``AXES_PROXY_TRUSTED_IPS``, and 
-   * ``AXES_IPWARE_META_PRECEDENCE_ORDER`` is now ``AXES_META_PRECEDENCE_ORDER``. 
+   * ``AXES_PROXY_ORDER`` is now ``AXES_IPWARE_PROXY_ORDER``,
+   * ``AXES_PROXY_COUNT`` is now ``AXES_IPWARE_PROXY_COUNT``,
+   * ``AXES_PROXY_TRUSTED_IPS`` is now ``AXES_IPWARE_PROXY_TRUSTED_IPS``, and
+   * ``AXES_META_PRECEDENCE_ORDER`` is now ``AXES_IPWARE_META_PRECEDENCE_ORDER``.
 
 
 6.0.0b1 (2023-04-25)
 --------------------
 
 - Set 429 as the default lockout response code. [hirotasoshu]
 
@@ -235,15 +242,15 @@
 - Add support for float or partial hours for ``AXES_COOLOFF_TIME``.
   [hramezani]
 
 
 5.32.0 (2022-04-08)
 -------------------
 
-- Add support for persistent failure logging
+- Add support for persistent logging
   where failed login attempts are persisted in the database
   until a specific threshold is reached.
   [p1-gdd]
 - Add support for not resetting login times when users
   try to login during the lockout cooloff period.
   [antoine-42]
```

### Comparing `django-axes-6.0.0b2/README.rst` & `django-axes-6.0.0b3/README.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/admin.py` & `django-axes-6.0.0b3/axes/admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/apps.py` & `django-axes-6.0.0b3/axes/apps.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/attempts.py` & `django-axes-6.0.0b3/axes/attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/backends.py` & `django-axes-6.0.0b3/axes/backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/checks.py` & `django-axes-6.0.0b3/axes/checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/conf.py` & `django-axes-6.0.0b3/axes/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/decorators.py` & `django-axes-6.0.0b3/axes/decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/handlers/base.py` & `django-axes-6.0.0b3/axes/handlers/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/handlers/cache.py` & `django-axes-6.0.0b3/axes/handlers/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 
 from axes.conf import settings
 from axes.handlers.base import AxesBaseHandler, AbstractAxesHandler
 from axes.helpers import (
     get_cache,
     get_cache_timeout,
-    get_client_cache_key,
+    get_client_cache_keys,
     get_client_str,
     get_client_username,
     get_credentials,
     get_failure_limit,
 )
 from axes.models import AccessAttempt
 from axes.signals import user_locked_out
@@ -40,29 +40,29 @@
             raise NotImplementedError("Cannot clear all entries from cache")
         if ip_or_username:
             raise NotImplementedError(
                 "Due to the cache key ip_or_username=True is not supported"
             )
 
         cache_keys.extend(
-            get_client_cache_key(
+            get_client_cache_keys(
                 AccessAttempt(username=username, ip_address=ip_address)
             )
         )
 
         for cache_key in cache_keys:
             deleted = self.cache.delete(cache_key)
             count += int(deleted) if deleted is not None else 1
 
         log.info("AXES: Reset %d access attempts from database.", count)
 
         return count
 
     def get_failures(self, request, credentials: Optional[dict] = None) -> int:
-        cache_keys = get_client_cache_key(request, credentials)
+        cache_keys = get_client_cache_keys(request, credentials)
         failure_count = max(
             self.cache.get(cache_key, default=0) for cache_key in cache_keys
         )
         return failure_count
 
     def user_login_failed(self, sender, credentials: dict, request=None, **kwargs):
         """
@@ -106,15 +106,26 @@
             request,
         )
 
         if self.is_whitelisted(request, credentials):
             log.info("AXES: Login failed from whitelisted client %s.", client_str)
             return
 
-        failures_since_start = 1 + self.get_failures(request, credentials)
+        cache_keys = get_client_cache_keys(request, credentials)
+        cache_timeout = get_cache_timeout()
+        failures = []
+        for cache_key in cache_keys:
+            added = self.cache.add(key=cache_key, value=1, timeout=cache_timeout)
+            if added:
+                failures.append(1)
+            else:
+                failures.append(self.cache.incr(key=cache_key, delta=1))
+                self.cache.touch(key=cache_key, timeout=cache_timeout)
+
+        failures_since_start = max(failures)
         request.axes_failures_since_start = failures_since_start
 
         if failures_since_start > 1:
             log.warning(
                 "AXES: Repeated login failure by %s. Count = %d of %d. Updating existing record in the cache.",
                 client_str,
                 failures_since_start,
@@ -122,19 +133,14 @@
             )
         else:
             log.warning(
                 "AXES: New login failure by %s. Creating new record in the cache.",
                 client_str,
             )
 
-        cache_keys = get_client_cache_key(request, credentials)
-        for cache_key in cache_keys:
-            failures = self.cache.get(cache_key, default=0)
-            self.cache.set(cache_key, failures + 1, get_cache_timeout())
-
         if (
             settings.AXES_LOCK_OUT_AT_FAILURE
             and failures_since_start >= get_failure_limit(request, credentials)
         ):
             log.warning(
                 "AXES: Locking out %s after repeated login failures.", client_str
             )
@@ -162,15 +168,15 @@
             request.axes_path_info,
             request,
         )
 
         log.info("AXES: Successful login by %s.", client_str)
 
         if settings.AXES_RESET_ON_SUCCESS:
-            cache_keys = get_client_cache_key(request, credentials)
+            cache_keys = get_client_cache_keys(request, credentials)
             for cache_key in cache_keys:
                 failures_since_start = self.cache.get(cache_key, default=0)
                 self.cache.delete(cache_key)
                 log.info(
                     "AXES: Deleted %d failed login attempts by %s from cache.",
                     failures_since_start,
                     client_str,
```

### Comparing `django-axes-6.0.0b2/axes/handlers/database.py` & `django-axes-6.0.0b3/axes/handlers/database.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/handlers/dummy.py` & `django-axes-6.0.0b3/axes/handlers/dummy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/handlers/proxy.py` & `django-axes-6.0.0b3/axes/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/handlers/test.py` & `django-axes-6.0.0b3/axes/handlers/test.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/helpers.py` & `django-axes-6.0.0b3/axes/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import timedelta
 from hashlib import sha256
 from logging import getLogger
 from string import Template
-from typing import Callable, Optional, Type, Union
+from typing import Callable, Optional, Type, Union, List
 from urllib.parse import urlencode
 
 from django.core.cache import BaseCache, caches
 from django.http import HttpRequest, HttpResponse, JsonResponse, QueryDict
 from django.shortcuts import redirect, render
 from django.utils.module_loading import import_string
 
@@ -244,29 +244,29 @@
         if settings.AXES_USE_USER_AGENT:
             # 4. The HTTP User-Agent can be used to track e.g. one browser
             filter_query[0]["user_agent"] = user_agent
 
     return filter_query
 
 
-def make_cache_key_list(filter_kwargs_list):
+def make_cache_key_list(filter_kwargs_list: List[dict]) -> List[str]:
     cache_keys = []
     for filter_kwargs in filter_kwargs_list:
         cache_key_components = "".join(
             value for value in filter_kwargs.values() if value
         )
         cache_key_digest = sha256(cache_key_components.encode()).hexdigest()
         cache_keys.append(f"axes-{cache_key_digest}")
     return cache_keys
 
 
-def get_client_cache_key(
+def get_client_cache_keys(
     request_or_attempt: Union[HttpRequest, AccessBase],
     credentials: Optional[dict] = None,
-) -> str:
+) -> List[str]:
     """
     Build cache key name from request or AccessAttempt object.
 
     :param request_or_attempt: HttpRequest or AccessAttempt object
     :param credentials: credentials containing user information
     :return cache_key: Hash key that is usable for Django cache backends
     """
```

### Comparing `django-axes-6.0.0b2/axes/locale/ar/LC_MESSAGES/django.mo` & `django-axes-6.0.0b3/axes/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/locale/ar/LC_MESSAGES/django.po` & `django-axes-6.0.0b3/axes/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/locale/de/LC_MESSAGES/django.mo` & `django-axes-6.0.0b3/axes/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/locale/de/LC_MESSAGES/django.po` & `django-axes-6.0.0b3/axes/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/locale/pl/LC_MESSAGES/django.mo` & `django-axes-6.0.0b3/axes/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/locale/pl/LC_MESSAGES/django.po` & `django-axes-6.0.0b3/axes/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/locale/ru/LC_MESSAGES/django.mo` & `django-axes-6.0.0b3/axes/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/locale/ru/LC_MESSAGES/django.po` & `django-axes-6.0.0b3/axes/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/locale/tr/LC_MESSAGES/django.mo` & `django-axes-6.0.0b3/axes/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/locale/tr/LC_MESSAGES/django.po` & `django-axes-6.0.0b3/axes/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/management/commands/axes_reset_failure_logs.py` & `django-axes-6.0.0b3/axes/management/commands/axes_reset_failure_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/management/commands/axes_reset_ip.py` & `django-axes-6.0.0b3/axes/management/commands/axes_reset_ip.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/management/commands/axes_reset_logs.py` & `django-axes-6.0.0b3/axes/management/commands/axes_reset_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/management/commands/axes_reset_username.py` & `django-axes-6.0.0b3/axes/management/commands/axes_reset_username.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/middleware.py` & `django-axes-6.0.0b3/axes/middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/migrations/0001_initial.py` & `django-axes-6.0.0b3/axes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/migrations/0002_auto_20151217_2044.py` & `django-axes-6.0.0b3/axes/migrations/0002_auto_20151217_2044.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/migrations/0003_auto_20160322_0929.py` & `django-axes-6.0.0b3/axes/migrations/0003_auto_20160322_0929.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/migrations/0004_auto_20181024_1538.py` & `django-axes-6.0.0b3/axes/migrations/0004_auto_20181024_1538.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/migrations/0007_alter_accessattempt_unique_together.py` & `django-axes-6.0.0b3/axes/migrations/0007_alter_accessattempt_unique_together.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/migrations/0008_accessfailurelog.py` & `django-axes-6.0.0b3/axes/migrations/0008_accessfailurelog.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/models.py` & `django-axes-6.0.0b3/axes/models.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/signals.py` & `django-axes-6.0.0b3/axes/signals.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/axes/utils.py` & `django-axes-6.0.0b3/axes/utils.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/django_axes.egg-info/PKG-INFO` & `django-axes-6.0.0b3/django_axes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.0b2
+Version: 6.0.0b3
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -124,23 +124,30 @@
 See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
 
 Changes
 =======
 
 
+6.0.0b3 (2023-05-01)
+--------------------
+
+- Use Django ``cache.incr`` API for atomic cached failure counting
+  [hirotasoshu, aleksihakli]
+
+
 6.0.0b2 (2023-04-28)
 --------------------
 
 - Make ``django-ipware`` an optional dependency. Install it with e.g. ``pip install django-axes[ipware]`` package and extras specifier. [aleksihakli]
 - Deprecate and rename old configuration flags. Old flags will be removed in or after version ``6.1``. [aleksihakli]
-   * ``AXES_PROXY_ORDER`` is now ``AXES_IPWARE_PROXY_ORDER``, 
-   * ``AXES_PROXY_COUNT`` is now ``AXES_IPWARE_PROXY_COUNT``, 
-   * ``AXES_IPWARE_PROXY_TRUSTED_IPS`` is now ``AXES_PROXY_TRUSTED_IPS``, and 
-   * ``AXES_IPWARE_META_PRECEDENCE_ORDER`` is now ``AXES_META_PRECEDENCE_ORDER``. 
+   * ``AXES_PROXY_ORDER`` is now ``AXES_IPWARE_PROXY_ORDER``,
+   * ``AXES_PROXY_COUNT`` is now ``AXES_IPWARE_PROXY_COUNT``,
+   * ``AXES_PROXY_TRUSTED_IPS`` is now ``AXES_IPWARE_PROXY_TRUSTED_IPS``, and
+   * ``AXES_META_PRECEDENCE_ORDER`` is now ``AXES_IPWARE_META_PRECEDENCE_ORDER``.
 
 
 6.0.0b1 (2023-04-25)
 --------------------
 
 - Set 429 as the default lockout response code. [hirotasoshu]
 
@@ -235,15 +242,15 @@
 - Add support for float or partial hours for ``AXES_COOLOFF_TIME``.
   [hramezani]
 
 
 5.32.0 (2022-04-08)
 -------------------
 
-- Add support for persistent failure logging
+- Add support for persistent logging
   where failed login attempts are persisted in the database
   until a specific threshold is reached.
   [p1-gdd]
 - Add support for not resetting login times when users
   try to login during the lockout cooloff period.
   [antoine-42]
```

### Comparing `django-axes-6.0.0b2/django_axes.egg-info/SOURCES.txt` & `django-axes-6.0.0b3/django_axes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/docs/1_requirements.rst` & `django-axes-6.0.0b3/docs/1_requirements.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/docs/2_installation.rst` & `django-axes-6.0.0b3/docs/2_installation.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/docs/3_usage.rst` & `django-axes-6.0.0b3/docs/3_usage.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/docs/4_configuration.rst` & `django-axes-6.0.0b3/docs/4_configuration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/docs/5_customization.rst` & `django-axes-6.0.0b3/docs/5_customization.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/docs/6_integration.rst` & `django-axes-6.0.0b3/docs/6_integration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/docs/7_architecture.rst` & `django-axes-6.0.0b3/docs/7_architecture.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/docs/Makefile` & `django-axes-6.0.0b3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/docs/conf.py` & `django-axes-6.0.0b3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/docs/images/flow.png` & `django-axes-6.0.0b3/docs/images/flow.png`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/pyproject.toml` & `django-axes-6.0.0b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/setup.py` & `django-axes-6.0.0b3/setup.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/tests/base.py` & `django-axes-6.0.0b3/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/tests/settings.py` & `django-axes-6.0.0b3/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/tests/test_admin.py` & `django-axes-6.0.0b3/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/tests/test_attempts.py` & `django-axes-6.0.0b3/tests/test_attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/tests/test_backends.py` & `django-axes-6.0.0b3/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/tests/test_checks.py` & `django-axes-6.0.0b3/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/tests/test_decorators.py` & `django-axes-6.0.0b3/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/tests/test_failures.py` & `django-axes-6.0.0b3/tests/test_failures.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/tests/test_handlers.py` & `django-axes-6.0.0b3/tests/test_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -492,20 +492,20 @@
         sender = MagicMock()
         AxesProxyHandler.user_login_failed(sender, credentials, self.request)
         self.assertFalse(cache_set.called)
         log.warning.assert_called_with(
             "AXES: Username is None and AXES_ONLY_USER_FAILURES is enabled, new record will NOT be created."
         )
 
-    @patch.object(cache, "set")
-    def test_user_login_failed_with_none_username(self, cache_set):
+    @patch.object(cache, "add")
+    def test_user_login_failed_with_none_username(self, cache_add):
         credentials = {"username": None, "password": "test"}
         sender = MagicMock()
         AxesProxyHandler.user_login_failed(sender, credentials, self.request)
-        self.assertTrue(cache_set.called)
+        self.assertTrue(cache_add.called)
 
 
 @override_settings(AXES_HANDLER="axes.handlers.dummy.AxesDummyHandler")
 class AxesDummyHandlerTestCase(AxesHandlerBaseTestCase):
     def test_handler(self):
         for _ in range(settings.AXES_FAILURE_LIMIT):
             self.login()
```

### Comparing `django-axes-6.0.0b2/tests/test_helpers.py` & `django-axes-6.0.0b3/tests/test_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from django.http import HttpRequest, HttpResponse, HttpResponseRedirect, JsonResponse
 from django.test import RequestFactory, override_settings
 
 from axes.apps import AppConfig
 from axes.helpers import (
     cleanse_parameters,
     get_cache_timeout,
-    get_client_cache_key,
+    get_client_cache_keys,
     get_client_ip_address,
     get_client_parameters,
     get_client_str,
     get_client_username,
     get_cool_off,
     get_cool_off_iso8601,
     get_lockout_response,
@@ -368,43 +368,43 @@
                     "user_agent": self.user_agent,
                 },
             ],
         )
 
 
 class ClientCacheKeyTestCase(AxesTestCase):
-    def test_get_cache_key(self):
+    def test_get_cache_keys(self):
         """
         Test the cache key format.
         """
 
         cache_hash_digest = sha256(self.ip_address.encode()).hexdigest()
         cache_hash_key = f"axes-{cache_hash_digest}"
 
         # Getting cache key from request
         request_factory = RequestFactory()
         request = request_factory.post(
             "/admin/login/", data={"username": self.username, "password": "test"}
         )
 
-        self.assertEqual([cache_hash_key], get_client_cache_key(request))
+        self.assertEqual([cache_hash_key], get_client_cache_keys(request))
 
         # Getting cache key from AccessAttempt Object
         attempt = AccessAttempt(
             user_agent="<unknown>",
             ip_address=self.ip_address,
             username=self.username,
             get_data="",
             post_data="",
             http_accept=request.META.get("HTTP_ACCEPT", "<unknown>"),
             path_info=request.META.get("PATH_INFO", "<unknown>"),
             failures_since_start=0,
         )
 
-        self.assertEqual([cache_hash_key], get_client_cache_key(attempt))
+        self.assertEqual([cache_hash_key], get_client_cache_keys(attempt))
 
     def test_get_cache_key_empty_ip_address(self):
         """
         Simulate an empty IP address in the request.
         """
 
         empty_ip_address = ""
@@ -416,29 +416,29 @@
         request_factory = RequestFactory()
         request = request_factory.post(
             "/admin/login/",
             data={"username": self.username, "password": "test"},
             REMOTE_ADDR=empty_ip_address,
         )
 
-        self.assertEqual([cache_hash_key], get_client_cache_key(request))
+        self.assertEqual([cache_hash_key], get_client_cache_keys(request))
 
         # Getting cache key from AccessAttempt Object
         attempt = AccessAttempt(
             user_agent="<unknown>",
             ip_address=empty_ip_address,
             username=self.username,
             get_data="",
             post_data="",
             http_accept=request.META.get("HTTP_ACCEPT", "<unknown>"),
             path_info=request.META.get("PATH_INFO", "<unknown>"),
             failures_since_start=0,
         )
 
-        self.assertEqual([cache_hash_key], get_client_cache_key(attempt))
+        self.assertEqual([cache_hash_key], get_client_cache_keys(attempt))
 
     def test_get_cache_key_credentials(self):
         """
         Test the cache key format.
         """
 
         ip_address = self.ip_address
@@ -450,28 +450,28 @@
         request = request_factory.post(
             "/admin/login/", data={"username": self.username, "password": "test"}
         )
 
         # Difference between the upper test: new call signature with credentials
         credentials = {"username": self.username}
 
-        self.assertEqual([cache_hash_key], get_client_cache_key(request, credentials))
+        self.assertEqual([cache_hash_key], get_client_cache_keys(request, credentials))
 
         # Getting cache key from AccessAttempt Object
         attempt = AccessAttempt(
             user_agent="<unknown>",
             ip_address=ip_address,
             username=self.username,
             get_data="",
             post_data="",
             http_accept=request.META.get("HTTP_ACCEPT", "<unknown>"),
             path_info=request.META.get("PATH_INFO", "<unknown>"),
             failures_since_start=0,
         )
-        self.assertEqual([cache_hash_key], get_client_cache_key(attempt))
+        self.assertEqual([cache_hash_key], get_client_cache_keys(attempt))
 
 
 class UsernameTestCase(AxesTestCase):
     @override_settings(AXES_USERNAME_FORM_FIELD="username")
     def test_default_get_client_username(self):
         expected = "test-username"
```

### Comparing `django-axes-6.0.0b2/tests/test_logging.py` & `django-axes-6.0.0b3/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/tests/test_login.py` & `django-axes-6.0.0b3/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/tests/test_management.py` & `django-axes-6.0.0b3/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/tests/test_middleware.py` & `django-axes-6.0.0b3/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.0b2/tests/test_models.py` & `django-axes-6.0.0b3/tests/test_models.py`

 * *Files identical despite different names*

